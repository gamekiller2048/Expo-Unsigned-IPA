example usage:
```
name: Build iOS IPA

on:
  push:
    branches:
      - master
jobs:
  build-ios:
    runs-on: macos-15

    steps:
      - name: Checkout Code
        uses: actions/checkout@v3

      - name: Expo Build Unsigned IPA
        uses: gamekiller2048/expo-unsigned-ipa@main
        with:
          PROJECT_NAME: '[MY EXPO PROJECT NAME]'

```
