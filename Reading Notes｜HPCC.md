#congestioncontrol
#网络监控测量
*sigcomm 2019*
HPCC是阿里推出的针对RDMA的拥塞控制协议，借助INT提供的详细信息来精确速率控制，具有快速收敛，保持接近zero-queue的优点。
## Motivation
目前高速网络存在三种问题：
- 收敛慢
- 
2.3 RDMA CC trade-off：
1. Throughput vs. Stability
2. Bandwidth vs. Latency
关键思想：
使用精确的链路负载信息精确控制流量

## Design
重要部分
1. Senders limit inflight bytes with sending windows.
发送方通过发送窗口限制字节数，
3. Congestion signal and control law based on inflight bytes.
4. Fast reaction without overreaction.
过度反应，