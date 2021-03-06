# 步骤 2：创建ECS实例 {#task_zjx_p1f_5db .task}

本文以入门级实例规格族为例，介绍如何使用控制台快速创建一个实例。详细的创建信息和更多创建方式，请参见 [创建实例](../../../../intl.zh-CN/用户指南/实例/创建实例/购买相同配置实例.md#) 章节。使用API创建实例，请 参见 [RunInstances](../../../../intl.zh-CN/API 参考/实例/RunInstances.md#)。

1.   登录 [云服务器ECS管理控制台](https://ecs.console.aliyun.com/#/home)。 
2.  在左侧导航栏，单击 **实例**。 
3.  在 实例列表 页面，单击 **创建实例**，进入 创建 页面。 
4.  完成 基础配置。 
    1.  选择 **计费方式**。本示例中，选择 **按量付费**。 
    2.  选择地域和可用区，如华东 1，可用区默认选择随机分配。 

        **说明：** 实例创建完成后，不可更改地域和可用区。

    3.  选择实例规格并设置实例数量。 可供选择的[实例规格族](../../../../intl.zh-CN/产品简介/实例规格族.md#)由您所选择的地域决定。本示例中，选择 **所有代** \> **x86计算** \> **入门级（共享）** \> **共享基本型xn4**。
    4.  选择镜像。本示例中，选择系统镜像。 
    5.  选择存储。本示例中，仅使用系统盘，默认选择40 GiB高效云盘。 
5.  单击 **下一步：网络和安全组**，完成网络和安全组设置。 
    1.  选择网络类型为 **专有网络**。本示例中，选择默认专有网络和默认交换机。 
    2.  设置公网带宽。 本示例中，选择 **分配公网IP地址** 为实例分配一个公网IP地址，并选择 **按使用流量** 对公网带宽计费。
    3.  选择安全组。如果您没有创建安全组，可以使用默认安全组。 
    4.  添加弹性网卡。如果所选实例规格不支持弹性网卡，跳过这一步。 
6.  单击 **下一步：系统配置**。 您可以选填此页面中的选项，建议您设置 **登录凭证** 和 **实例名称**。本示例中，选择**自定义密码**，并将实例名称设为ecs-01。
7.  单击 **下一步：分组设置**。您可以选填此页面中的选项，有多台实例时，建议添加标签方便管理。 
8.  单击 **下一步：确认订单**。确认所选配置，您也可以单击编辑图标返回修改配置。 
9.  阅读和确认 **云服务器ECS服务条款**，然后单击 **创建实例**。 

单击 **管理控制台** 回到控制台，一般需要1~5分钟完成实例创建。单击刷新按钮，新建的ECS实例状态变为 **运行中**，表示实例创建成功。

