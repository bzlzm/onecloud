
# 玩客云openwrt自动编译

旁路由：此版本缺失了snmpd，其它完美。
更改opkg列表
src/gz openwrt_core https://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/targets/amlogic/meson8b/packages
src/gz openwrt_base http://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/base/
# src/gz openwrt_kenzo https://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/kenzo
src/gz openwrt_luci http://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/luci/
src/gz openwrt_packages http://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/packages/
src/gz openwrt_routing http://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/routing/
# src/gz openwrt_small https://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/small
src/gz openwrt_telephony http://mirrors.tencent.com/lede/releases/24.10-SNAPSHOT/packages/arm_cortex-a5_vfpv4/telephony/
然后在线安装snmpd即可。

## 使用方法

文件名包含burn的为线刷固件，解压后使用[Amlogic_USB_Burning_Tool](https://androiddatahost.com/khfj4)烧录。\
红灯闪是在启动中，启动完成后蓝灯常亮。首次启动时间可能会长一些(五分钟左右)。

- 登录ip: 10.0.0.188
- 用户名: root
- 密码: password

## 感谢
- 自动编译工作流改自 https://github.com/P3TERX/Actions-OpenWrt
- 玩客云u-boot https://github.com/hzyitc/u-boot-onecloud
- openwrt源码 https://github.com/coolsnowwolf/lede
- 线刷包打包工具 https://github.com/hzyitc/AmlImg
- 打包脚本改自 https://github.com/shiyu1314/openwrt-onecloud
- 所有为openwrt做出贡献的人
