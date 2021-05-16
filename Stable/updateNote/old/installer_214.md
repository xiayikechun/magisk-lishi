## 2021.1.17 Magisk v21.4

**Update**: v21.4 adds more regression hot fixes.

Happy 2021! v21.3 adds a workaround for devices with buggy F2FS Linux kernel drivers. This F2FS bug may cause bootloops on many devices. Checkout the full [v21.0 release notes](https://gitee.com/mintimate/magick_custom_update_source/raw/master/note/installer/installer_210.md) if coming from older releases.

### v21.4

- [MagiskSU] Fix `su -c` behavior that broke many root apps
- [General] Properly handle read/write over sockets (the `broken pipe` issue)

### v21.3

- [MagiskInit] Avoid mounting `f2fs` userdata as it may result in kernel crashes. This shall fix a lot of bootloops
- [MagiskBoot] Fix a minor header checksum bug for `DHTB` header and ASUS `blob` image formats
- [MagiskHide] Allowing hiding isolated processes if the mount namespace is separated


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

## 统计
- 12月份，本源累计被调取9283次
- 12月份，服务器累计消耗流量40G

