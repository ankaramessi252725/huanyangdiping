# Evoxt 香港 VPS 最新测评报告

## 香港 VPS 上游更换概况

Evoxt 近期对其香港 VPS 的上游服务商进行了调整，目前已全面切换至 XTOM。这一变化对网络性能和用户体验带来了显著影响。本文将通过详细的路由追踪和性能测试数据，为您呈现最新的香港 VPS 使用体验。

## 网络路由表现分析

Evoxt 香港 VPS 的网络路由因运营商不同而有所差异。以下是从上海地区三大主流运营商（电信、联通、移动）的去程路由测试结果：

### 上海电信 (163 AS4134)
去程路由显示，电信用户的数据通过移动 CMI 网络传输，部分节点绕行日本 NTT。以下是详细的 traceroute 数据：

traceroute to 202.101.21.178, 30 hops max, 32 byte packets
1   103.193.131.153  中国 香港  xtom.com.hk  18.35 ms / 16.73 ms / 9.08 ms
2   103.193.131.90   中国 香港  xtom.com.hk  0.79 ms / 0.91 ms / 2.56 ms
3   103.193.131.76   中国 香港  xtom.com.hk  1.90 ms / 0.76 ms / 1.59 ms
4   103.193.131.87   中国 香港  xtom.com.hk  37.47 ms / 4.71 ms / 7.14 ms
5   223.119.81.186   中国 香港  cmi.chinamobile.com  0.77 ms / 0.41 ms / 0.88 ms
...
18  202.101.21.178   中国 上海市  chinatelecom.cn  69.97 ms / 66.95 ms / 65.59 ms

### 上海联通 (169 AS4837)
联通用户的去程同样通过移动 CMI 网络，延迟表现稳定：

traceroute to 139.226.206.150, 30 hops max, 32 byte packets
1   103.193.131.153  中国 香港  xtom.com.hk  17.40 ms / 18.52 ms / 17.03 ms
2   103.193.131.92   中国 香港  xtom.com.hk  4.24 ms / 104.79 ms / 6.35 ms
...
15  139.226.227.38   中国 上海市  chinaunicom.cn  60.14 ms / * ms / * ms

### 上海移动 (骨干网 AS9808)
移动用户直接接入骨干网，延迟较低，整体表现优异：

traceroute to 120.204.34.85, 30 hops max, 32 byte packets
1   103.193.131.153  中国 香港  xtom.com.hk  11.93 ms / 68.68 ms / 17.86 ms
...
13  120.204.34.85    中国 上海市  chinamobile.com  30.84 ms / 32.01 ms / 31.87 ms

从数据来看，Evoxt 香港 VPS 的路由优化较为合理，尤其是移动用户的网络体验更为流畅。

## 系统性能与磁盘速度测试

通过 YABS (Yet-Another-Bench-Script) 测试，我们对 Evoxt 香港 VPS 的硬件性能进行了全面评估。以下是关键数据：

### 基本系统信息
- **操作系统**: Debian GNU/Linux 11 (bullseye)
- **处理器**: QEMU Virtual CPU @ 3593.250 MHz（单核）
- **内存**: 473.1 MiB
- **磁盘**: 4.8 GiB
- **虚拟化类型**: KVM
- **网络支持**: IPv4 和 IPv6 双栈在线

### 磁盘速度 (fio 测试)
磁盘读写性能表现均衡，尤其在较大块大小下表现出色：
- **4k 读写**: 178.25 MB/s (44.5k IOPS)
- **64k 读写**: 1.90 GB/s (29.7k IOPS)
- **512k 读写**: 2.38 GB/s (4.6k IOPS)
- **1m 读写**: 1.75 GB/s (1.7k IOPS)

对于需要高吞吐量的应用场景，这款 VPS 的磁盘性能完全能够胜任。

👉 [2025年最新 Evoxt 优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## 网络速度测试 (iperf3)

### IPv4 网络表现
- **伦敦, UK**: 发送 542 Mbits/sec，接收 178 Mbits/sec，延迟 232 ms
- **巴黎, FR**: 发送 554 Mbits/sec，接收 207 Mbits/sec，延迟 179 ms
- **洛杉矶, US**: 发送 576 Mbits/sec，接收 116 Mbits/sec，延迟 157 ms

### IPv6 网络表现
- **伦敦, UK**: 发送 460 Mbits/sec，接收 193 Mbits/sec，延迟 233 ms
- **巴黎, FR**: 发送 589 Mbits/sec，接收 214 Mbits/sec，延迟 183 ms
- **洛杉矶, US**: 发送 655 Mbits/sec，接收 240 Mbits/sec，延迟 168 ms

测试结果表明，Evoxt 香港 VPS 在全球范围内的网络速度较为稳定，尤其在亚太地区表现出色，适合跨境业务或需要低延迟的用户。

## 总结

Evoxt 香港 VPS 在更换上游至 XTOM 后，网络路由和性能表现均有提升。无论是移动、联通还是电信用户，都能获得较为稳定的连接体验。同时，其磁盘和网络速度测试数据也显示出较高的性价比。对于追求高性能香港 VPS 的用户来说，这款产品值得一试。