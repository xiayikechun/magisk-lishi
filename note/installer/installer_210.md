## v21.0
- [General] Support Android 11 🎉
- [General] Add Safe Mode detection. Disable all modules when the device is booting into Safe Mode.
- [General] Increase post-fs-data mode timeout from 10 seconds to 40 seconds
- [MagiskInit] Rewritten 2SI support from scratch
- [MagiskInit] Support when no /sbin folder exists (Android 11)
- [MagiskInit] Dump fstab from device-tree to rootfs and force init to use it for 2SI devices
- [MagiskInit] Strip out AVB for 2SI as it may cause bootloop
- [Modules] Rewritten module mounting logic from scratch
- [MagiskSU] For Android 8.0+, a completely new policy setup is used. This reduces compromises in Android’s sandbox, providing more policy isolation and better security for root users.
- [MagiskSU] Isolated mount namespace will now first inherit from parent process, then isolate itself from the world
- [MagiskSU] Update communication protocol with Magisk Manager to work with the hardened SELinux setup
- [MagiskPolicy] Optimize match all rules. This will significantly reduce policy binary size and save memory and improve general kernel performance.
- [MagiskPolicy] Support declaring new types and attributes
- [MagiskPolicy] Make policy statement closer to stock *.te format. Please check updated documentation or magiskpolicy --help for more details.
- [MagiskBoot] Support compressed extra blobs
- [MagiskBoot] Pad boot images to original size with zeros
- [MagiskHide] Manipulate additional vendor properties

## Mintimate's Blog (English)
- 11.14 Update This.
- Offical Web:https://www.mintimate.cn
- Donate: https://www.mintimate.cn/about
- Offical QQ Group:1051948568

## Mintimate's Blog (中文)
- 最后更新时间:11.14
- 如果有问题:https://www.mintimate.cn
- 如果先捐赠:https://www.mintimate.cn/about
- 本自定义源反馈QQ群:1051948568

## 统计
- 10月份，本源累计被调取12718次
- 10月份，服务器累计消耗流量58G

## 黑名单
- QQ用户：397105900 在QQ群内恶意对线，态度蛮狠；望大家小心。
