(https://deepwiki.com/badge.svg)]# # GeoIP 简介 [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/Loyalsoldier/geoip) ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/Loyalsoldier/geoip/total?logo=github) ![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/Loyalsoldier/geoip/latest/total?logo=github) [![jsdelivr stats](https://data.jsdelivr.com/v1/package/gh/Loyalsoldier/geoip/badge?style=rounded)](https://www.jsdelivr.com/package/gh/Loyalsoldier/geoip)


本项目是 [Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip) 的修改版本。

### 项目初衷
主要针对 Box4Magisk、Box for Root 等代理模块的 ipset 功能，提供**区分 IPv4 与 IPv6** 的中国大陆 IP 列表（TXT 格式）。

### 核心特性
* **自动更新**：每日凌晨自动生成 sing-box (`SRS`)、mihomo (`MRS`) 及 `TXT` 格式文件。
* **数据增强**：在原项目基础上，额外整合了以下中国大陆（CN）数据源：
  * [苍狼山庄](https://ispip.clang.cn/)、[纯真IP](https://github.com/metowolf/iplist)、[misakaio](https://github.com/misakaio/chnroutes2)
* **逻辑优化**：对所有数据源进行去重和合并（merge），确保生成的 CIDR 格式严谨、无重叠。

---

## 下载地址与使用方法

本项目发布的所有文件均可在 [Latest Release](https://github.com/X-Shelby/geoip/releases/tag/latest) 中找到。

**常用文件固定链接：**
* **IPv4 (TXT)**: [cn_v4.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v4.txt)
* **IPv6 (TXT)**: [cn_v6.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn_v6.txt)
* **混合 (TXT)**: [cn.txt](https://github.com/X-Shelby/geoip/releases/download/latest/cn.txt)
* **sing-box (SRS)**: [cn.srs](https://github.com/X-Shelby/geoip/releases/download/latest/cn.srs)
* **Mihomo (MRS)**: [cn.mrs](https://github.com/X-Shelby/geoip/releases/download/latest/cn.mrs)

> **注意**：如果无法访问 `raw.githubusercontent.com`，可以尝试使用 `cdn.jsdelivr.net` 或 `fastly.jsdelivr.net` 进行加速。

---

## 声明与致谢
本项目默认使用 [MaxMind GeoLite2 Country CSV 数据](https://github.com/Loyalsoldier/geoip/blob/release/GeoLite2-Country-CSV.zip)。
更多关于原项目的设计逻辑，请参考原作者 [Loyalsoldier](https://github.com/Loyalsoldier/geoip) 的仓库。

## License

[CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/) and [GPL-3.0](https://github.com/Loyalsoldier/geoip/blob/master/LICENSE-GPL)

This product includes GeoLite2 data created by MaxMind, available from [MaxMind](https://www.maxmind.com).
