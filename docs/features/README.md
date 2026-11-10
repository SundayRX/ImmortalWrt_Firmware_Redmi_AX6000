# 功能使用指南

[返回首页](../../README.md) · [安装、升级与恢复](../flashing.md)

从设备接入局域网，到路由器查询域名，按下面的顺序了解网络如何工作。每篇教程都包含原理图、设置步骤和常见问题处理。

| 想了解或完成什么 | 阅读 |
|---|---|
| IP、网关、DHCP 分别有什么用，设备怎样获得网络参数 | [LAN 与地址分配](lan.md#lan-basics) |
| 给打印机、NAS 或电脑固定地址，区分静态租约与 ARP 绑定 | [固定地址的选择与设置](lan.md#fixed-address) |
| 修改路由器的局域网网段，重新连接管理页面 | [修改 LAN 网段](lan.md#change-subnet) |
| 一次域名查询怎样经过缓存、规则与上游服务器 | [DNS 工作原理](dns.md#query-flow) |
| 修改 PPPoE / DHCP 获取的普通 DNS，检查 WAN/WAN6 | [普通 DNS 设置](dns.md#ordinary-dns) |
| 加密路由器的 DNS 查询，选择故障时是否回退 | [25.12 加密 DNS（DoH）](dns.md#doh) |
| 理解 OpenClash、浏览器安全 DNS 与系统设置的关系 | [其他解析服务与实际查询路径](dns.md#other-services) |

初次设置建议先读 **LAN → DNS**；已经能正常上网时，可以直接打开需要的章节。系统版本、下载与修复清单见 [25.12](../systems/25.12-6.12.md)、[24.10](../systems/24.10-6.6.md)、[21.02](../systems/21.02-5.4.md)。
