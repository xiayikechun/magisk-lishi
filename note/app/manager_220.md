## 2020.2.23 Magisk v22.0

### RESTORE THE EXISTING MAGISK MANAGER BACK TO NORMAL BEFORE UPGRADING IF HIDDEN!

Another major Magisk release! This time our focus is not the core Magisk implementation, but rather on improving the whole Magisk user experience.

### Magisk Manager is dead.<br>Long live the Magisk app!

Ever since the first Magisk release, Magisk (the core components) and Magisk Manager (the companion app) are released separately and isn't necessarily always in sync. This leads to some confusion and a lot of complexity when downloading/installing Magisk through the app. Starting from v22.0, the Magisk app (renamed from Magisk Manager) includes everything it needs within the APK itself, making installation a 100% offline process.

Custom recovery lovers, no worries! The Magisk app APK *itself* is a custom recovery flashable zip, just like MAGIC鈩煂�. Check out the updated [installation guide](https://topjohnwu.github.io/Magisk/install.html) for more info.

### App Hiding

Another major breakthrough in this release is that devices lower than Android 9.0 can now also use the advanced app hiding technique to hide the Magisk app. Due to this incompatible change, **RESTORE THE EXISTING MAGISK MANAGER BACK TO NORMAL BEFORE UPGRADING IF HIDDEN!**

### Bug Fixes

- [MagiskHide] Fix a bug when stopping MagiskHide does not take effect
- [MagiskBoot] Fix bug when unpacking `lz4_lg` compressed boot images
- [MagiskInit] Support Galaxy S21 series
- [MagiskSU] Fix incorrect APEX paths that caused `libsqlite.so` fail to load

### Full Changelog: [here](https://topjohnwu.github.io/Magisk/changes.html)

## Mintimate's Blog (English)
- 21.02.24 Update This.
- Offical Web:https://www.mintimate.cn
- Donate: https://www.mintimate.cn/about
- Offical QQ Group:1051948568

## Mintimate's Blog (中文)
- 最后更新时间:21.02.24
- 如果有问题:https://www.mintimate.cn
- 如果先捐赠:https://www.mintimate.cn/about
- 本自定义源反馈QQ群:1051948568

## 统计
- 01月份，本源累计被调取12291次
- 01月份，服务器累计消耗流量140G
