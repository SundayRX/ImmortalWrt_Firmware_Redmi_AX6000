# Redmi AX6000 固件

面向 **Redmi AX6000 / RB06、普通 110m 布局**的 ImmortalWrt 固件，提供双频 Wi-Fi、网页管理、网络加速和插件扩展。先按插件兼容性选择系统，再下载对应的固件包。

**仅适用于 RB06 普通 110m。** 小米 AX6000 / RA72、原厂分区和其他布局不能直接刷入。第一次安装请先看[设备与布局要求](docs/flashing.md#layout-comparison)。

[选择版本](#选择版本) · [下载固件](#下载) · [安装与升级](docs/flashing.md) · [安装插件](docs/flashing.md#package-install) · [功能指南](docs/features/README.md) · [LAN 与固定 IP](docs/features/lan.md) · [DNS 设置](docs/features/dns.md)

## 选择版本

**从安全维护角度，优先推荐使用 25.12。** 该系列采用 Linux 6.12 和 [OpenSSL 3.5 LTS](https://openssl-library.org/policies/releasestrat/) 等较新的基础组件；选择前请确认常用插件有适配的 APK 版本，使用中及时安装固件更新。

| 系统系列 | 适合谁 | 防火墙与插件 | 管理界面 |
|---|---|---|---|
| [25.12 / Linux 6.12](docs/systems/25.12-6.12.md) | ⭐️ **重视安全维护、新功能与新版界面** | FW4 / nftables；APK 软件包 | LuCI 25.12，Argon 3.0.0 |
| [24.10 / Linux 6.6](docs/systems/24.10-6.6.md) | **需要 FW4，并继续使用适配的 IPK 插件** | FW4 / nftables；OPKG 安装 IPK | LuCI 24.10，Argon 2.4.3 |
| [21.02 / Linux 5.4](docs/systems/21.02-5.4.md) | ☆ **需要旧版 FW3 / IPK 插件兼容** | FW3 / iptables；OPKG 安装 IPK | LuCI 21.02，Argon 2.3.1 |

25.12 使用 APK，不能直接安装 IPK；需要保留 FW4 + IPK 插件组合时选择 24.10；依赖旧版 FW3 插件时可选 21.02，其系统与插件生态较旧。跨系列升级前，请先确认常用插件有对应版本。

三套系统均采用 MediaTek 厂商 Wi-Fi 驱动。下载区列出各系列可用版本及组件信息，发行页标明 `SNAPSHOT` 或预发布状态。

## 下载

### 25.12 / Linux 6.12

<!-- AX6000:25.12-6.12:START -->
- [下载最新版本与查看说明](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases/tag/ImmortalWrt-25.12-Kernel-6.12-41187c9-20261109T151844Z) · 编译时间：2026-11-09 15:18:44 UTC
- [全部版本与历史固件](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases?q=%2225.12-6.12%22)

| 项目 | 此固件版本 |
| --- | --- |
| 系统 | ImmortalWrt 25.12-SNAPSHOT `r0-41187c9` |
| 内核 | Linux `6.12.112` |
| 布局 | 普通 110m（`immortalwrt-110m`） |
| Wi-Fi 驱动 | MediaTek `mt_wifi` `7.6.7.3` |
| LuCI | `26.289.10016~36e3f0d` |
| Argon | `3.0.0-r20261016` |
<!-- AX6000:25.12-6.12:END -->

[功能与使用说明](docs/systems/25.12-6.12.md) · [修复与改进](docs/systems/25.12-6.12.md#fixes)

### 24.10 / Linux 6.6

<!-- AX6000:24.10-6.6:START -->
- [下载最新版本与查看说明](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases/tag/ImmortalWrt-24.10-Kernel-6.6-571cef0-20261104T144745Z) · 编译时间：2026-11-04 14:47:45 UTC
- [全部版本与历史固件](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases?q=%2224.10-6.6%22)

| 项目 | 此固件版本 |
| --- | --- |
| 系统 | ImmortalWrt 24.10-SNAPSHOT `r0-571cef0` |
| 内核 | Linux `6.6.133` |
| 布局 | 普通 110m（`immortalwrt-110m`） |
| Wi-Fi 驱动 | MediaTek `mt_wifi` `7.6.7.3` |
| LuCI | `26.246.30525~80ed8a4` |
| Argon | `2.4.3-r20250722.1` |
<!-- AX6000:24.10-6.6:END -->

[功能与使用说明](docs/systems/24.10-6.6.md) · [修复与改进](docs/systems/24.10-6.6.md#fixes)

### 21.02 / Linux 5.4

<!-- AX6000:21.02-5.4:START -->
- [下载最新版本与查看说明](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases/tag/ImmortalWrt-21.02-Kernel-5.4-7503e41-20261105T030120Z) · 编译时间：2026-11-05 03:01:20 UTC
- [全部版本与历史固件](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/releases?q=%2221.02-5.4%22)

| 项目 | 此固件版本 |
| --- | --- |
| 系统 | ImmortalWrt 21.02-SNAPSHOT `r0-7503e41` |
| 内核 | Linux `5.4.284` |
| 布局 | 普通 110m（`immortalwrt-110m`） |
| Wi-Fi 驱动 | MediaTek `mt_wifi` `7.6.7.3` |
| LuCI | `git-23.360.32803-5829eab` |
| Argon | `2.3.1` |
<!-- AX6000:21.02-5.4:END -->

[功能与使用说明](docs/systems/21.02-5.4.md) · [修复与改进](docs/systems/21.02-5.4.md#fixes)

打开发行页，核对系统、布局和插件版本，再下载 **Assets 中的固件 ZIP**。GitHub 自动生成的 `Source code (zip/tar.gz)` 不能刷机。

ZIP 名称包含系统、内核、设备、布局和编译时间，末尾 `Z` 表示 UTC 时间。解压后按用途选择文件：

| 文件 | 用途 |
|---|---|
| `firmware/*squashfs-sysupgrade.bin` | 已有系统内更新或回退 |
| `firmware/*squashfs-factory.bin` | 配套 U-Boot 网页安装或恢复 |
| `bootloader/*-fip-fixed-parts.bin` | RB06 普通 110m 引导文件；初次安装或明确需要更新引导时使用 |
| `release-notes.md` / `packages.txt` | 本次固件说明 / 软件包版本清单 |
| `SHA256SUMS` | 核对包内文件完整性 |

刷写前完成[下载校验](docs/flashing.md#verify-download)。sysupgrade 和 factory 按入口选择其一，无需依次刷入；FIP 是独立引导文件，日常升级无需重刷。使用旧发行包时，先按其文件清单确认安装和恢复所需文件齐全。

## 功能与改进

各系列说明列出无线连接、管理操作和系统升级的改进；预装软件清单见固件包内的 `packages.txt`。

| 使用环节 | 改进重点 |
|---|---|
| 安全维护 | 更新证书信任和相关系统组件，修复特定网页请求、上传及防火墙规则处理问题；具体适用项目见各系列说明 |
| 无线连接 | 关联兼容、密钥更新、无线配置保存及双频状态显示 |
| 管理页面 | 改善概览加载、配置保存、静态租约管理和手机布局；25.12 增加日志倒序与软件包安装结果提示 |
| 网络与服务 | 完善加速设置生效、限速与访问控制配合，以及服务异常后的恢复；25.12 提供加密 DNS（DoH）设置和当前上游列表，可选择是否允许故障时回退到普通 DNS |
| 升级与恢复 | 完善备份与写入失败提示，提供跨系列配置保护、安装与恢复镜像；25.12 减少未改动的内置 OpenClash 数据库重复备份 |

查看完整清单：[25.12](docs/systems/25.12-6.12.md#fixes) · [24.10](docs/systems/24.10-6.6.md#fixes) · [21.02](docs/systems/21.02-5.4.md#fixes)。

## 默认设置

| 项目 | 默认值 |
|---|---|
| 管理地址 | `192.168.31.1` |
| 用户名 / 密码 | `root`；未预设密码，首次登录后设置 |
| 主机名 | `Redmi_AX6000` |
| 时区 | `Asia/Singapore`，UTC+8 |
| LAN IPv6 | 默认关闭；WAN IPv6 可独立配置 |
| 局域网 DNS | 默认向设备提供路由器地址 `192.168.31.1` |
| 上游 DNS | WAN 自动获取；手动设置见[修改 DNS](#dns-settings) |
| 加密 DNS | 25.12 提供 DoH，默认关闭；设置方法见[加密 DNS](docs/systems/25.12-6.12.md#dns-over-https) |

以上为出厂默认设置。保留配置升级时，继续使用原有的管理地址、密码和网络设置。

首次使用按以下顺序设置：

1. 电脑用网线连接 LAN，自动获取 IP，打开 `http://192.168.31.1` 并设置管理员密码。
2. 根据接入方式配置 WAN：宽带拨号填写运营商提供的 PPPoE 账号密码，上级路由器分配地址时选择 DHCP。
3. 设置 Wi-Fi 名称与密码，确认有线和无线均能上网后，再按需启用插件。OpenClash 需要另行下载代理核心并导入自己的配置。

<a id="dns-settings"></a>
<a id="pppoe-宽带拨号"></a>
<a id="dhcp-自动获取地址上网"></a>

### LAN 与 DNS 设置

设备接入局域网后，通过 DHCP 获得 IP、网关和 DNS 地址。默认由路由器为设备提供域名解析，再按设置查询上游 DNS。

- [LAN 与地址分配](docs/features/lan.md)：理解 IP、网关与 DHCP，给设备固定地址，修改局域网网段。
- [普通 DNS 设置](docs/features/dns.md#ordinary-dns)：查看 PPPoE / DHCP 的 DNS 来源，设置 WAN/WAN6 上游或恢复自动获取。
- [25.12 加密 DNS](docs/features/dns.md#doh)：理解 DoH、引导 IP 和故障回退，按需要启用加密查询。

<a id="安装与使用"></a>

## 更新与回退

已有本仓库普通 110m 固件且管理页面可用时，优先从“系统 → 备份/升级”上传 `*squashfs-sysupgrade.bin`。**在 25.12、24.10、21.02 之间升级或回退，都取消保留配置**，安装后重新设置网络并安装匹配插件。不能整包恢复另一系列的备份。

系统无法启动时，使用同布局的 factory 镜像从配套 U-Boot 恢复。多布局引导请选择 **`immortalwrt-110m`**；`default` 是另一种布局。完整步骤、备份范围和旧版升级页面的处理办法见[安装、升级与恢复](docs/flashing.md)。

<a id="查看周边-wi-fi"></a>

## 常见使用问题

| 需求 | 操作与注意事项 |
|---|---|
| 给设备固定 IP | 25.12 在“网络 → DHCP”管理静态租约；21.02、24.10 在“网络 → DHCP/DNS → 静态租约”管理。离线设备也能编辑；选择与步骤见[固定地址](docs/features/lan.md#fixed-address) |
| 某些设备没有主机名 | 未上报名称的设备显示 IP 或 MAC，可在静态租约中为该设备填写名称 |
| 查看周边 Wi-Fi | 在“状态 → 信道分析”选择频段，需要新结果时重新扫描。查看结果不自动更改工作信道；扫描会短暂占用无线资源 |
| 传输文件 | 使用“系统 → 文件传输”，或在 SFTP 客户端中填写路由器地址、SSH 端口（默认 22）和登录凭据；网页可执行操作取决于账号权限 |
| 升级后恢复插件 | 自行安装的插件程序通常需要重装；先确认 IPK/APK、防火墙和内核依赖，另行恢复插件数据 |
| 手动上传软件包 | 在“系统 → 软件包”上传匹配本系列的安装包；25.12 的单次安装选项与结果说明见[软件包安装](docs/flashing.md#package-install) |
| 保留配置后可用空间变少 | 检查恢复的数据和外装插件；OpenClash 数据库的备份与空间处理见[备份与空间](docs/flashing.md#backup-space) |
| 平均负载如何理解 | 三个数分别对应最近 1、5、15 分钟的平均负载，不是 CPU 使用率百分比；CPU 使用率请看概览中的独立项目 |
| 升级后仍显示旧页面 | 按 `Ctrl+F5`，必要时清除管理地址的站点缓存并重新登录，无需因此恢复路由器出厂设置 |
| 限速或统计与预期不同 | 检查硬件加速和代理是否影响该功能，再按所选系统的使用说明调整 |
| 对照固件新旧 | 在“状态 → 概览”查看版本及编译时间。下载页使用 UTC，路由器按设置的时区显示 |

21.02 的信道图支持 HT20/40 显示；需要查看 80/160 MHz 带宽时，可选择 24.10 或 25.12。

<a id="反馈"></a>

## 来源与反馈

系统及组件来源与许可见[来源与许可](docs/sources-and-licenses.md)。

遇到问题可提交 [Issue](https://github.com/SundayRX/ImmortalWrt_Firmware_Redmi_AX6000/issues)，附完整 Release Tag 或固件版本、升级方式、是否保留配置，以及复现步骤。截图和日志请先去除密码、订阅地址、令牌等私密信息。

<!-- AX6000:DOCUMENTS:{"build":{"commit":"0c4bd82c28dd1e99d469571527490180db793f42","run_attempt":"1","run_id":"42756680640"},"schema":1,"templates_sha256":"8d642a4fb680e837fc86c143744458028e735facaad79291412e6dd50c042fe9"} -->
