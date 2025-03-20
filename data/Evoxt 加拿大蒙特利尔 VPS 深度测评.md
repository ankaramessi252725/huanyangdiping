# Evoxt 加拿大蒙特利尔 VPS 深度测评

## 测评套餐详情

以下是本次测评所使用的 Evoxt 加拿大蒙特利尔 VPS 套餐配置：

- **型号**: VM-0.5  
- **核心数**: 1 个核心  
- **内存**: 512MB  
- **存储空间**: 5GB  
- **备份**: 每周备份  
- **价格**: 2.99 美元/月  

这款套餐适合轻量级应用或初次尝试 VPS 的用户，性价比颇高。

## 测试 IP 与 Looking Glass

测试使用的 IP 地址如下：  
- **IPv4**: 38.95.173.112  
- **IPv6**: 2400:8d60:0012:0000:0000:0000:b628:b2d7  
- **地理位置**: 加拿大 蒙特利尔  

这些 IP 可用于 ping 测试或 traceroute，方便用户验证网络连通性。

## 流媒体解锁表现

Evoxt 蒙特利尔 VPS 在流媒体解锁方面表现出色，以下是测试结果：

============[ 多国家流媒体解锁测试 ]============
Dazn:                  是 (地区: 加拿大)
Disney+:               即将支持 [Disney+ 马来西亚]
Netflix:               是 (地区: 马来西亚)
YouTube Premium:       是 (地区: 加拿大)
Amazon Prime Video:    是 (地区: 加拿大)
TVBAnywhere+:          是
Spotify 注册:          是 (地区: 加拿大)
iQyi 海外地区:         加拿大
Bing 地区:             加拿大 (可能有风险)
YouTube CDN:           蒙特利尔, 魁北克
Netflix 首选 CDN:      法兰克福
ChatGPT:               是
Google Gemini:         是 (地区: 加拿大)
Claude:                是
Wikipedia 可编辑性:    是
Google Play 商店:      加拿大
Google 搜索免验证码:   是
Steam 货币:            加拿大元 (CAD)
Reddit:                是
=======================================

从结果来看，该 VPS 支持多款主流流媒体服务，如 Netflix、YouTube Premium 和 Amazon Prime Video，特别适合需要跨区域访问内容的用户。

👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## TCP 回程路由分析

以下是针对不同网络运营商的回程路由测试数据，展示了从蒙特利尔 VPS 到中国各地的网络路径和延迟表现：

### 上海 CN2 / 广东东莞 CN2

1   *  
2   10.255.4.10     RFC1918                    0.32 ms  
3   67.215.0.66     加拿大 蒙特利尔 globo.tech  1.56 ms  
5   154.24.95.57    加拿大 蒙特利尔 cogentco.com 1.24 ms  
9   154.54.72.42    德国 法兰克福 cogentco.com  87.83 ms  
15  59.43.159.17    中国 上海 chinatelecom.cn   268.18 ms  
18  58.32.32.1      中国 上海 chinatelecom.cn   263.76 ms  

### 上海电信

3   67.215.0.68     加拿大 蒙特利尔 globo.tech  0.34 ms  
5   154.24.95.57    加拿大 蒙特利尔 cogentco.com 1.55 ms  
15  61.152.71.66    中国 上海 chinatelecom.cn   224.72 ms  
16  101.95.52.34    中国 上海 chinatelecom.cn   226.23 ms  

### 上海联通 9929

3   67.215.0.66     加拿大 蒙特利尔 globo.tech  0.65 ms  
14  154.54.44.86    美国 洛杉矶 cogentco.com    75.68 ms  
18  218.105.2.150   中国 上海 chinaunicom.cn   197.71 ms  

### 广州移动

3   67.215.0.68     加拿大 蒙特利尔 globo.tech  0.87 ms  
8   64.125.23.239   美国 洛杉矶 zayo.com       58.85 ms  
17  120.241.55.26   中国 深圳 gd.10086.cn      240.14 ms  

### 教育网

3   67.215.0.66     加拿大 蒙特利尔 globo.tech  0.41 ms  
10  184.105.64.129  中国 香港 he.net           188.39 ms  
23  101.6.15.130    中国 北京 edu.cn          226.87 ms  

路由测试表明，Evoxt 蒙特利尔 VPS 通过 Cogent 和 GloboTech 等骨干网络，延迟表现因目标地区和运营商而异，整体适合需要连接北美和欧洲的用户。

## 带宽速度测试

以下是不同地区的上传和下载速度测试结果：

节点名称         上传速度     下载速度     延迟  
Speedtest.net   928.27 Mbps  913.46 Mbps  0.64 ms  
新加坡 SG      367.53 Mbps  904.37 Mbps  205.84 ms  
东京 JP        438.35 Mbps  300.02 Mbps  165.18 ms  
美国 US        877.63 Mbps  906.61 Mbps  59.59 ms  
德国 DE        772.77 Mbps  917.84 Mbps  90.45 ms  
南京 CT        64.91 Mbps   682.76 Mbps  231.65 ms  
上海 CU        347.91 Mbps  381.62 Mbps  253.01 ms  

测试显示，蒙特利尔 VPS 在北美和欧洲拥有优异的带宽表现，亚洲地区速度稍有下降但仍可满足大部分需求。

## YABS 性能测试

以下是 VPS 的硬件性能测试结果：

CPU 型号:         AMD EPYC-Genoa 处理器  
CPU 核心:         1  
CPU 主频:         4491.480 MHz  
磁盘容量:         4.9 GB (已用 1.3 GB)  
内存:            457 MB (已用 76 MB)  
系统运行时间:      1 天 6 小时 28 分  
操作系统:         Debian GNU/Linux 12  
架构:            x86_64 (64 位)  
虚拟化技术:       KVM  
I/O 速度(平均):    621.0 MB/s  

YABS 测试表明，该 VPS 的 I/O 性能稳定，适合运行小型网站或轻量级应用。