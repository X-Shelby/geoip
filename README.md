# GeoIP 简介 [![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/X-Shelby/geoip/total?logo=github)](https://github.com/X-Shelby/geoip) ![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/X-Shelby/geoip/latest/total?logo=github) [![jsdelivr stats](https://data.jsdelivr.com/v1/package/gh/X-Shelby/geoip/badge?style=rounded)](https://www.jsdelivr.com/package/gh/X-Shelby/geoip)

**本项目是 [Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip) 的修改版本。**

### 项目初衷
主要针对 Box4Magisk、Box for Root 等代理模块的 ipset 功能，提供**区分 IPv4 与 IPv6** 的中国大陆 IP 列表（TXT 格式）。

### 核心特性
* **自动更新**：每日凌晨自动生成 sing-box (`SRS`)、mihomo (`MRS`) 及 `TXT` 格式文件。
* **数据增强**：在原项目基础上，
 - 中国大陆 IPv4 地址数据融合了 [IPIP.net](https://github.com/17mon/china_ip_list/blob/master/china_ip_list.txt) 和 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china.txt)
 - 中国大陆 IPv6 地址数据使用 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china6.txt)
* **额外整合了以下中国大陆（CN）数据源：**
 [苍狼山庄](https://ispip.clang.cn/)、[纯真IP](https://github.com/metowolf/iplist)、[BGP-misakaio](https://github.com/misakaio/chnroutes2)、[APNIC-mayaxcn](https://raw.githubusercontent.com/mayaxcn/china-ip-list/master/chnroute.txt)、[ASN-missuo](https://raw.githubusercontent.com/missuo/ASN-China/refs/heads/main/IPv4.China.list)、[MetaCubeX-V4](https://raw.githubusercontent.com/MetaCubeX/meta-rules-dat/refs/heads/meta/geo/geoip/cn.list)
* **逻辑优化**：对所有数据源进行去重和合并（merge），确保生成的 CIDR 格式严谨、无重叠。

---

## 下载地址与使用方法

本项目发布的所有文件均可在 [Latest Release](https://github.com/X-Shelby/geoip/releases/tag/latest) 中找到。

**常用文件固定链接：**
* **IPv4 (TXT)**: [cn_v4.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v4.txt)
* **IPv6 (TXT)**: [cn_v6.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v6.txt)
* **混合 (TXT)**: [cn.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn.txt)
* **sing-box IPv4 (SRS)**: [cn_v4.srs](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v4.srs)
* **sing-box IPv6 (SRS)**: [cn_v6.srs](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v6.srs)
* **sing-box cnip混合新链接 (SRS)**: [cnip_all.srs](https://github.com/X-Shelby/geoip/releases/download/latest/cnip_all.srs)
* **Mihomo IPv4 (MRS)**: [cn_v4.mrs](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v4.mrs)
* **Mihomo IPv6 (MRS)**: [cn_v6.mrs](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v6.mrs)
* **Mihomo cnip混合新链接 (MRS)**: [cnip_all.mrs](https://github.com/X-Shelby/geoip/releases/download/latest/cnip_all.mrs)


> **注意**：如果无法访问 `raw.githubusercontent.com`，可以尝试使用 `cdn.jsdelivr.net` 或 `fastly.jsdelivr.net` 进行加速。

---

## 声明与致谢
本项目默认使用 [MaxMind GeoLite2 Country CSV 数据](https://github.com/Loyalsoldier/geoip/blob/release/GeoLite2-Country-CSV.zip)。

更多关于原项目的设计逻辑，请参考原作者 [Loyalsoldier](https://github.com/Loyalsoldier/geoip) 的仓库。

## License

[CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/) and [GPL-3.0](https://github.com/Loyalsoldier/geoip/blob/master/LICENSE-GPL)

This product includes GeoLite2 data created by MaxMind, available from [MaxMind](https://www.maxmind.com).
