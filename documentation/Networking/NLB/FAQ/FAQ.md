# 常见问题

**Q：单用户的负载均衡配额？**

A：现支持单用户同一地域下最多创建5个LB，如需提升配额请提交工单或联系客服人员。


**Q：网络负载均衡相关资源的配额限制？**

A：一个负载均衡实例下最多可创建20个监听器、20个后端服务、20个虚拟服务器组，每个虚拟服务器组最多可添加100台后端服务器。


**Q：网络负载均衡无法与后端服务器实例进行通信？**

A：后端云主机/容器实例的安全组、ACL必须显示的允许负载均衡和服务器实例之间的通信，注意ACL为无状态规则，需要分别配置流入、流出负载均衡的策略。

**Q：网络负载均衡TCP协议监听如何获取客户端真实IP？**

A：网络负载均衡后端服务挂接高可用组或者实例类型（添加虚机或者容器对象）的虚拟服务器组时，IP报文头缺省就能够直接透传客户端真实源IP，不需任何特殊配置或者操作。
   
**Q：多可用区是怎样保障高可用的？**

A：只能将负载均衡所在可用区内的云主机/容器添加为后端服务，按照设置的调度算法进行流量转发，当一个可用区出现故障时，流量将自动切换至其他可用区服务器。

   
**Q：负载均衡后端服务如何选择关联虚拟服务器组还是高可用组？**

A：虚拟服务器组可以由用户手动或者通过与AS关联自动增删云主机实例，手动配置方式使用简单；虚拟服务器组可以与AS（弹性伸缩）关联使用，实现跨可用区的高可用，但不保证同可用区内跨机架的高可用。高可用组自动实现了主机实例跨AZ、跨机架的高可用分配与按照规则弹性伸缩，提供比虚拟服务器组更灵活、更自动的主机分配服务。因此用户需要简单使用、快速上手时，可选择关联虚拟服务器组；用户需要自动的高可用服务，建议选择关联高可用组。

   
**Q：一个负载均衡实例占用的内网ip资源？**

A：负载均衡在每个可用区采用高可用架构，默认启用两个实例资源，除去vip还需要占用两个所在子网的ip资源，因此单可用区一共会占用3个内网ip，双可用区会占用5个内网ip，每多支持一个可用区需多占用两个所在子网的ip资源，以此类推。
另外当网络负载均衡进行横向弹性扩展的时候，将占用更多内网ip资源，用户需要尽量为网络负载均衡预留足够的内网ip、以备支持足够的弹性扩展能力，目前建议至少预留10个内网ip。
