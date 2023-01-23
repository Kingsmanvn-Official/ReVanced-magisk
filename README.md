#### ⚠️ Do not download modules from 3rd party sources like random websites you found on Google. Only use this repository. I am not responsible for anything they may contain.

# ReVanced Magisk Module
[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/revanced_kingsmanvn)
[![Build Modules](https://github.com/j-hc/revanced-magisk-module/actions/workflows/build.yml/badge.svg)](https://github.com/Kingsmanvn-Official/ReVanced-Magisk/actions/workflows/build.yml)
[![CI](https://github.com/Kingsmanvn-Official/ReVanced-Magisk/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/Kingsmanvn-Official/ReVanced-Magisk/actions/workflows/ci.yml)
[![Latest release](https://img.shields.io/github/v/release/Kingsmanvn-Official/ReVanced-Magisk?style=flat-square)](https://github.com/Kingsmanvn-Official/ReVanced-Magisk/releases/latest)

Get the [latest CI release](https://github.com/Kingsmanvn-Official/ReVanced-Magisk/releases).

[**mindetach module**](https://github.com/j-hc/mindetach-magisk) in the releases section detaches YouTube and YouTube Music from Play Store and blocks it from updating them.

## Features
 * Support all present and future ReVanced and [ReVanced Extended](https://github.com//inotia00/revanced-patches) apps
 * Can build Magisk modules and non-root APKs
 * Updated daily with the latest versions of apps and patches in accordance with your configuration
 * Cleans APKs from unneeded libs to make them smaller
 * Fully open-source, every binary or APK is compiled without human intervention
 * Modules
     * recompile invalidated odex for YouTube and Music apps for faster usage
     * receive updates from Magisk app
     * do not break safetynet or trigger root detections used by certain apps
     * handle installation of the correct version of the stock app and all that
     * mount the patched app immediately without needing to reboot

#### **Note that the [CI workflow](../../actions/workflows/ci.yml) is scheduled to build the modules and APKs every 6 hours using GitHub Actions if there is a change. You may want to disable it.**
#### **Fix next video not autoplay (error from upstream)**

## To include/exclude patches or patch more ReVanced Apps
[**See the list of patches**](https://github.com/revanced/revanced-patches#-list-of-available-patches)

 * Star the repo :eyes:
 * [Fork the repo](https://github.com/j-hc/revanced-magisk-module/fork) or use it as a template
 * Edit the options in [`config.toml`](./config.toml)
 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

To add more Revanced apps or know more about `config.toml`, read here [`CONFIG.md`](./CONFIG.md)

To be able to use non-root variants of YouTube and YT Music, install [inotia00 MicroG](https://github.com/inotia00/VancedMicroG/releases).

# Building Locally
Make sure you have JDK 17 installed. Then run:

```console
$ git clone --recurse-submodules https://github.com/j-hc/revanced-magisk-module
$ cd revanced-magisk-module
$ ./build.sh
```
