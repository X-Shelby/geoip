# GeoIP 简介 [![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/Loyalsoldier/geoip) ![GitHub Downloads (all assets, all releases)](https://img.shields.io/github/downloads/Loyalsoldier/geoip/total?logo=github) ![GitHub Downloads (all assets, latest release)](https://img.shields.io/github/downloads/Loyalsoldier/geoip/latest/total?logo=github) [![jsdelivr stats](https://data.jsdelivr.com/v1/package/gh/Loyalsoldier/geoip/badge?style=rounded)](https://www.jsdelivr.com/package/gh/Loyalsoldier/geoip)

### 去重和合并 IP 与 CIDR（`merge`）
根据提供的所有数据源，去重，将其转换为目标格式，并输出到文件。

本项目为原项目的修改版，主要用于Box4Magisk、Box for Root等代理模块的ipset功能提供区分ipv4跟ipv6的cn_ip｀TXT`文件。每日凌晨自动生成包括sing-box `SRS` 、mihomo `MRS` 、TXT的格式文件。更详细内容请查看原作者[Loyalsoldier](https://github.com/Loyalsoldier/geoip)的项目！
此fork与原项目的相比，增加了
- 中国大陆（CN）IPv4、IPv6地址 [苍狼山庄](https://ispip.clang.cn/)、[纯真IP](https://github.com/metowolf/iplist)、[misakaio](https://github.com/misakaio/chnroutes2/blob/master/chnroutes.txt) 的数据源
## 与 MaxMind 官方 GeoIP 数据的区别

本项目默认使用 [MaxMind GeoLite2 Country CSV 数据](https://github.com/Loyalsoldier/geoip/blob/release/GeoLite2-Country-CSV.zip)生成各个国家和地区的 GeoIP 文件。所有可供使用的国家和地区 geoip 类别（如 `geoip:cn`，两位英文字母表示国家和地区），请查看：[https://www.iban.com/country-codes](https://www.iban.com/country-codes)。

另外，本项目对 MaxMind 官方 GeoIP 数据做了修改和新增：

- 中国大陆 IPv4 地址数据融合了 [IPIP.net](https://github.com/17mon/china_ip_list/blob/master/china_ip_list.txt) 和 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china.txt)
- 中国大陆 IPv6 地址数据使用 [@gaoyifan/china-operator-ip](https://github.com/gaoyifan/china-operator-ip/blob/ip-lists/china6.txt)
-

## 下载地址与使用方法

本项目发布的所有 GeoIP 文件，请查看 [release](https://github.com/X-Shelby/geoip/releases/tag/latest)。以下是部分格式GeoIP 文件的下载地址：

固定下载链接：
- IPv4 (TXT): https://github.com/X-Shelby/geoip/releases/download/latest/cn_v4.txt
- IPv6 (TXT): https://github.com/X-Shelby/geoip/releases/download/latest/cn_v6.txt
- 合并 (TXT): https://github.com/X-Shelby/geoip/releases/download/latest/cn.txt
- sing-box (SRS): https://github.com/X-Shelby/geoip/releases/download/latest/cn.srs
- Mihomo (MRS): https://github.com/X-Shelby/geoip/releases/download/latest/cn.mrs
> 如果无法访问域名 `raw.githubusercontent.com`，可以使用第二个地址 `cdn.jsdelivr.net`。
> 如果无法访问域名 `cdn.jsdelivr.net`，可以将其替换为 `fastly.jsdelivr.net`。
>。

## License

[CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/) and [GPL-3.0](https://github.com/Loyalsoldier/geoip/blob/master/LICENSE-GPL)

This product includes GeoLite2 data created by MaxMind, available from [MaxMind](https://www.maxmind.com).
