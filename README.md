# Manat Bölgüsü (Money Sorter)

Android app that works out how many banknotes are needed for each payment.

## Install on your phone

1. On your Android phone open **https://github.com/yusifqocali/Money-Sorter/releases/latest**
2. Tap **ManatBolgusu.apk** to download it.
3. Open the downloaded file. If Android asks, allow *Install unknown apps* for your browser, then tap **Install**.

## How the APK is built

Every push to `main` runs the **Build APK** workflow (`.github/workflows/build-apk.yml`).
It builds a signed APK and publishes it as a new Release. A newer build installs over the old one.

## Changing the app

The whole app is one page: `app/src/main/assets/index.html`. Edit it, commit, and a new APK appears in Releases a few minutes later.

The signing key in `keystore/` is committed so every build can update the installed app. The repository is public, so anyone could sign an app with this key. That is fine for a personal tool, but don't publish this app to Google Play with it.
