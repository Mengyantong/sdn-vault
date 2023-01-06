#拥塞控制
#网络监控测量
2.3 RDMA CC trade-off：
1. Throughput vs. Stability
2. Bandwidth vs. Latency
关键思想：
使用精确的链路负载信息精确控制流量

## design
重要部分
1. Senders limit inflight bytes with sending windows.
发送方通过发送窗口限制字节数，
3. Congestion signal and control law based on inflight bytes.
4. Fast reaction without overreaction.
过度反应，