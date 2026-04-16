# 计算机网络

## 应用层

- **HTTP / HTTPS**：请求方法（GET/POST/PUT/DELETE）、状态码、Cookie/Session、HTTPS 握手流程、TLS 原理
- **DNS**：域名解析流程（递归/迭代）、A/CNAME/MX 记录、DNS 缓存
- **CDN**：内容分发原理、回源机制、边缘节点缓存策略

## 传输层

- **TCP 三次握手**：SYN → SYN-ACK → ACK，为什么不是两次/四次
- **TCP 四次挥手**：FIN → ACK → FIN → ACK，TIME_WAIT 状态及意义
- **流量控制**：滑动窗口机制
- **拥塞控制**：慢启动、拥塞避免、快重传、快恢复
- **UDP**：无连接、不可靠、低延迟场景（DNS、视频流）

## 网络层

- **IP 协议**：IPv4/IPv6、分片与重组
- **路由**：静态路由、动态路由（OSPF、BGP）
- **NAT**：地址转换原理，私有地址段

## 链路层

- **以太网**：帧格式、MTU
- **ARP**：IP → MAC 地址解析流程，ARP 缓存，ARP 欺骗
