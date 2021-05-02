## 2021.4.9 Magisk v22.1

This release is focused on fixing regressions and bugs. Check the [v22.0 release notes](https://topjohnwu.github.io/Magisk/releases/22000.html) if coming from older releases.

Note: Magisk v22 is the last major version to support Jellybean and Kitkat. Magisk v23 will only support Android 5.0 and higher.
注意：从该版本开始，不再支持5.1以前的Android版本！！！

### Bug Fixes

- [App] Prevent multiple installation sessions running in parallel
- [App] Prevent OutOfMemory crashes when checking boot signature on PXA boot images
- [General] Proper cgroup migration implementation
- [General] Rewrite log writer from scratch, should resolve any crashes and deadlocks
- [General] Many scripts updates fixing regressions
- [MagiskHide] Prevent possible deadlock when signal arrives
- [MagiskHide] Partial match process names if necessary
- [MagiskBoot] Preserve and patch AVB 2.0 structures/headers in boot images
- [MagiskBoot] Properly strip out data encryption flags
- [MagiskBoot] Prevent possible integer overflow
- [MagiskInit] Fix `sepolicy.rule` mounting strategy
- [resetprop] Always delete existing `ro.` props before updating. This will fix bootloops that could be caused by modifying device fingerprint properties.

### Full Changelog: [here](https://topjohnwu.github.io/Magisk/changes.html)

## Mintimate's Blog (English)
- 21.04.11 Update This.
- Offical Web:https://www.mintimate.cn
- Donate: https://www.mintimate.cn/about
- Offical QQ Group:1051948568

## Mintimate's Blog (中文)
- 最后更新时间:21.04.11
- 如果有问题:https://www.mintimate.cn
- 如果想捐赠:https://www.mintimate.cn/about
- 本自定义源反馈QQ群:1051948568

## 警告⚠️
- 为节约服务器成本，拟定6月份关闭本更新源
- 20.03--21.06 感谢1年的陪伴

## 统计
- 04月份，本源被调取6255次
- 04月份，服务器消耗流量32.11G
