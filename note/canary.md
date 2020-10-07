## v8.0.1
- Fix `vbmeta.img` patching for Samsung `AP.tar` files. This fixes bootloops on devices like Galaxy S10 after flashing updated AP files.
- Properly truncate existing files before writing to prevent corrupted files
- Prevent a possible UI loop when device ran into very low memory
- Switch to use JSDelivr CDN for several files

## Magisk v21.0
Long time no see! v21.0 is the largest release in Magisk’s history. It comes with full Android 11 support (tons of stuff had to be rewritten from scratch!), and a completely redesigned Magisk Manager. These are the reasons why this particular public release took me over half a year to wrap up.

To the end user, not much has changed other than the fact that Magisk Manager has completely changed its appearance. However developers should pay some attention to some changes due to adjustments for Android 11. Full changelogs are too massive to fit, so here I’ll point out the main changes and links to updated documentations.

## Highlights
- Android 11 support 🎉
- Completely redesigned Magisk Manager
- Safe Mode detection: if you installed a module that bootloops your device, reboot into Safe Mode and all modules will be disabled. More instructions on how to deal with broken modules is linked here.
- The following are for advanced users/developer:

- On Android 8.0+, Magisk now uses a new SELinux setup that keeps Android sandbox less compromised. This provides better security to rooted users, and also separates Magisk rules from original rules. Details here.
- On Android 11, /sbin may no longer exist. For developers, this means the Magisk’s internal tmpfs directory is no longer always /sbin, and instead randomly created every boot. To get the tmpfs path, use the command magisk --path (more details here). For custom kernel developers that uses overlay.d, updated docs are here.
- magiskpolicy gained more features and some minor syntax changes, details here.


## Mintimate's Blog (English)
- 10.02 Add This.
- Offical Web:https://www.mintimate.cn
- Offical QQ Group:1051948568
- WeChat Official Accounts:MintimateBlog

## Mintimate's Blog (中文)
- 最后更新时间:10.02
- 如果有问题:https://www.mintimate.cn/about
- 本自定义源反馈QQ群:1051948568
- 微信公众号:MintimateBlog

## 统计
- 9月份，本源累计被调取9063次
- 9月份，服务器累计消耗流量52G

## 黑名单
- QQ用户：397105900 在QQ群内恶意对线，态度蛮狠；望大家小心。
