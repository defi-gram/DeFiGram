## Telegram messenger for Android

[DeFiGram](https://www.defigram.net) is a messaging app with a focus on speed and security. It’s superfast, simple and free.
This repo contains the official source code for [DeFiGram App for Android](https://www.defigram.net/app).

### Compilation Guide

You will require Android Studio 3.4, Android NDK rev. 20 and Android SDK 8.1

1. Download the DeFiGram source code
2. Copy your release.keystore into TMessagesProj/config
3. Fill out RELEASE_KEY_PASSWORD, RELEASE_KEY_ALIAS, RELEASE_STORE_PASSWORD in gradle.properties to access your  release.keystore
4. Go to https://console.firebase.google.com/, create two android apps with application IDs org.telegram.messenger and org.telegram.messenger.beta, turn on firebase messaging and download google-services.json, which should be copied to the same folder as TMessagesProj.
5. Open the project in the Studio (note that it should be opened, NOT imported).
6. Fill out values in TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java – there’s a link for each of the variables showing where and which data to obtain.
7. You are ready to compile Telegram.
