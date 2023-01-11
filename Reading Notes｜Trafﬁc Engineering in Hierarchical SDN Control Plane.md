## Motivation

随着网络快速发展，网络架构正在演变成complex interconnection of circuit-switched domains and layers, 划分受到地理、管理、客户需求和经济成本的影响，而
1. centralized controller不足以处理高频率的流量请求
2. 如果设计distributed controllers来提高控制器性能，需要在所有控制器上保存一个network-wide view的copy， keeping them consistent is expensive. hierarchical controllers不需要copy但是由于根控制器keeping a global view，需要计算全部cross-domain的flows，导致provide limited improvements on scalability。而且如果处于保密的考虑在控制器上维护一个全局状态是不可行的。
tiao zhatiao z

