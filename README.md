# OpenWrt-Tsubasa-Mod

## 项目特色

- 项目基于 [immortalwrt/immortalwrt](https://github.com/immortalwrt/immortalwrt) openwrt-18.06-k5.4 分支，内核版本为 5.4.x，LuCI 版本为 LuCI 18.06。
- 项目是参考 xuanwumen/openwrt-project 的基础编译模板修改的。
- 项目加入了个人的爱好，可能不通用于大多数的人。

## 设备/平台支持情况

|   支持设备 / 平台    |                         下载链接                          |         Platform         |  Target  | Subtarget |
| :------------------: | :-------------------------------------------------------: | :----------------------: | :------: | :-------: |
|    Rockchip 33xx     | [🔗](http://openwrt.cc/snapshots/targets/rockchip/armv8/)  |     aarch64_generic      | rockchip |   armv8   |
|    x86_64 (64位)     |     [🔗](http://openwrt.cc/snapshots/targets/x86/64/)      |          x86_64          |   x86    |    64     |

Rockchip 33xx： 要晚些时间再加入。
目前仅支持 x86 系统的 64 位平台，32 位不考虑支持。


## 软件包安装指南

更新软件包索引:

```
opkg update
```

列出可安装的所有 LuCI APP :

```
opkg list | grep luci-app | grep -v Translation
```

此时可以得到该软件包的中文翻译包为 `luci-i18n-ssr-plus-zh-cn`，使用 `opkg install` 命令安装此翻译包即可:

```
opkg install luci-i18n-ssr-plus-zh-cn
```

可安装的 LuCI APP 列表:

<https://github.com/SuLingGG/OpenWrt-Mini/blob/main/doc/LuCI-App-List.md>

更多 opkg 使用方法请参考 OpenWrt Guide:

<https://openwrt.org/docs/guide-user/additional-software/opkg>

## 鸣谢

特别感谢以下项目：

Openwrt 官方项目：

https://github.com/openwrt/openwrt

Lean 大的 Openwrt 项目：

https://github.com/coolsnowwolf/lede

Project ImmortalWrt 的 ImmortalWrt 项目：

https://github.com/immortalwrt/immortalwrt

P3TERX 大佬的 Actions-OpenWrt 项目：

https://github.com/P3TERX/Actions-OpenWrt

除这些项目之外，也特别感谢所有为 OpenWrt 项目及社区作出贡献的朋友们～