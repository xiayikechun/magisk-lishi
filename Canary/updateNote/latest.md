### Guide
It has been a while since the last public release, long time no see! A personal update for those unaware: I am now working at Google on the Android Platform Security team. Without further ado, let's jump right into it!

### MagiskHide Removal

I have lost interest in fighting this battle for quite a while; plus, the existing MagiskHide implementation is flawed in so many ways. Decoupling Magisk from root hiding is, in my opinion, beneficial to the community. Ever since my announcement on Twitter months ago, highly effective "root hiding" modules (much **MUCH** better than MagiskHide) has been flourishing, which again shows that people are way more capable than I am on this subject. So why not give those determined their time to shine, and let me focus on improving Magisk instead of drowning in the everlasting cat-and-mouse game 😉.

### Sunsetting Magisk-Modules-Repo

Due to lack of time and maintenance, the centralized Magisk-Modules-Repo was frozen, and the functionality to download modules from the repo is removed in v24.0. As a supplement, module developers can now specify an `updateJson` URL in their modules. The Magisk app will use that to check, download, and install module updates.

### Introducing Zygisk

Zygisk is **Magisk in Zygote**, the next big thing for Magisk! When this feature is enabled, a part of Magisk will run in the `Zygote` daemon process, allowing module developers to run code directly in every Android apps' processes. If you've heard of [Riru](https://github.com/RikkaApps/Riru), then Zygisk is inspired by that project and is functionally similar, though the implementation is quite different internally. I cannot wait to see what module developers can achieve using Zygisk!

### Documentation

For developers, details about `updateJson` and building Zygisk modules can all be found in the updated [documentation](https://topjohnwu.github.io/Magisk/guides.html#magisk-modules).

### v24.0 Full Changelog

- [General] MagiskHide is removed from Magisk
- [General] Support 64-bit only systems
- [General] Support Android 12
- [General] Update BusyBox to 1.34.1
- [Zygisk] Introduce new feature: Zygisk
- [Zygisk] Introduce DenyList feature to revert Magisk features in user selected processes
- [MagiskBoot] Support patching 32-bit kernel zImages
- [MagiskBoot] Support boot image header v4
- [MagiskBoot] Support patching out `skip_initramfs` from dtb bootargs
- [MagiskBoot] Add new env variable `PATCHVBMETAFLAG` to configure whether vbmeta flags should be patched
- [MagiskInit] Support loading fstab from `/system/etc` (required for Pixel 6)
- [MagiskInit] Support `/proc/bootconfig` for loading boot configurations
- [MagiskInit] Better support for some Meizu devices
- [MagiskInit] Better support for some OnePlus/Oppo/Realme devices
- [MagiskInit] Support `init.real` on some Sony devices
- [MagiskInit] Skip loading Magisk when detecting DSU
- [MagiskPolicy] Load `*_compat_cil_file` from system_ext
- [MagiskSU] Use isolated devpts if the kernel supports it
- [MagiskSU] Fix root shell if isolated mount namespace is set
- [resetprop] Deleted properties are now wiped from memory instead of just unlinking
- [App] Build a single APK for all ABIs
- [App] Switch to use standard bottom navigation bar
- [App] Downloading modules from the centralized Magisk-Modules-Repo is removed
- [App] Support user configuration of boot image vbmeta patching
- [App] Restore the ability to install Magisk on the other slot on some A/B devices
- [App] Allow modules to specify an update URL for in-app update + install

## Mintimate's Blog (English)
- 01.20 Update This.
- Offical Web:https://www.mintimate.cn
- Donate: https://www.mintimate.cn/about
- Offical QQ Group:1051948568

## Mintimate's Blog (中文)
- 最后更新时间:01.20
- 如果有问题:https://www.mintimate.cn
- 如果先捐赠:https://www.mintimate.cn/about
- 本自定义源反馈QQ群:1051948568
