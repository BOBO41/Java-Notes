企业级分布式应用服务（Enterprise Distributed Application Service, 简称 EDAS）是阿里巴巴中间件团队研发的 PaaS 平台，为企业提供高可用和分布式的互联网架构解决方案。

HSF为EDAS应用开发提供一套分布式服务框架的解决方案，从应用层面为大家提供统一的服务发布/调用支持，让开发者很容易的开发分布式的应用，不用考虑分布式领域中的各种技术细节（远程通讯，性能损耗、调用的透明化、同步/异步调用方法的实现等等问题）

资源
云服务器ECS
负载均衡SLB
专有网络VPC

EDAS agent ps -ef|grep agent

应用
  必须有agent的机器上
  部署
  启用
  停止

服务列表

应用回滚 回滚到之前部署的版本
应用扩容 添加机器 多机器
应用删除 应用必须停止

EDAS 日志查看

应用监控
  cpu 内存 磁盘 网络 rpc 。。。

弹性伸缩 通过cpu 服务器的增减 资源控制

应用诊断 分析内存 类加载 对象内存

通知报警 机器的硬件的使用率 来判断

限流 QPS thread 超过阈值 不服务

降级 RT 调用的服务超过时间 不使用

监控
响应时间(RT)
　　响应时间是指系统对请求作出响应的时间。
吞吐量(TPS)
    吞吐量是指系统在单位时间内处理请求的数量。
QPS 每秒查询率(Query Per Second)
　　每秒查询率QPS是对一个特定的查询服务器在规定时间内所处理流量多少的衡量标准，在因特网上，作为域名系统服务器的机器的性能经常用每秒查询率来衡量。对应fetches/sec，即每秒的响应请求数，也即是最大吞吐能力。 （看来是类似于TPS，只是应用于特定场景的吞吐量）
