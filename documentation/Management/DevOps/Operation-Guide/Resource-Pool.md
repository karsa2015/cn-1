# 资源池

主机资源包括京东云主机、其他第三方主机（包括物理机、虚机）。如您的账户已经关联京东云控制台账户，可使用快速导入的方式直接勾选控制台中的云主机至DevOps平台中用于部署。

**术语定义**

资源池

为了更好地管理主机，分配主机，引入了资源池的概念。资源池功能主要的作用是进行主机归属分配，即将主机资源从外部（京东云控制台或者手工）导入到产品线，再将主机从产品线分配到具体的应用。

**导入主机资源到资源池**

菜单栏-->配置管理-->资源池

![Alt text](https://github.com/jdcloudcom/cn/blob/DevOps/image/DevOps/Operation11.png)

1.京东云主机

提供两种资源池导入方式：

1）快速导入：在服务树中选择需要导入的产品线，点击“快速导入”按钮，在导入页面选择云主机所属地域，点击“查询”按钮，勾选相应云主机后，点击“导入”，即可将选中的云主机导入到左侧服务树指定产品线的备机池中。

2）批量导入：服务树中选择需要导入的产品线，根据提供的导入模板正确填写主机信息，点击“导入”，即可将文件中的云主机导入到左侧服务树指定产品线的备机池中。

2.其他

仅支持批量导入的方式。
