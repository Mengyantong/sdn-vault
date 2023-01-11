#TE
#IWQoS
## Motivation
随着网络快速发展，网络架构正在演变成complex interconnection of circuit-switched domains and layers, 划分受到地理、管理、客户需求和经济成本的影响，而
1. centralized controller不足以处理高频率的流量请求
2. 如果设计distributed controllers来提高控制器性能，需要在所有控制器上保存一个network-wide view的copy， keeping them consistent is expensive. hierarchical controllers不需要copy但是由于根控制器keeping a global view，需要计算全部cross-domain的flows，导致provide limited improvements on scalability。而且如果处于保密的考虑在控制器上维护一个全局状态是不可行的。
## 挑战
- Description of the network view：在不泄露网络信息的情况下支持te
- Collaboration among controllers: 控制器之间如何协作实现最佳带宽分配
- TE optimization algorithm: te寻找路径为流量分配带宽，目的是最大限度提高网络利用率和满足Qos要求。算法必须实现max-min fairness,

