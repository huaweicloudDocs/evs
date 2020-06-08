# API版本选择建议<a name="evs_04_0007"></a>

## API风格说明<a name="section1092352712223"></a>

当前EVS服务对外的API存在以下两种风格：

-   EVS服务自定义规范的API，以下简称为EVS自定义API。
-   顺从OpenStack社区标准原生规范的API，以下简称为OpenStack Cinder API。

两者风格不同，功能相近。OpenStack Cinder API主要用于满足您在开源生态工具方面的对接需求。针对某些功能，EVS自定义API在OpenStack Cinder API基础上，做了功能增强。

-   支持创建包周期的云硬盘
-   支持扩容包周期的云硬盘
-   支持企业项目管理

## 版本号介绍<a name="section23345249250"></a>

EVS自定义API提供v2和v3版本。在接口功能相同的情况下，推荐您优先使用v3接口。

同时，针对创建、扩容云硬盘，还提供了v2.1接口，可以针对包周期云硬盘执行相关操作。

-   [创建云硬盘](创建云硬盘-API-v2.md)
-   [扩容云硬盘](扩容云硬盘-API-v2.md)

OpenStack Cinder API提供v2和v3版本，其中v3支持微版本号。在接口功能相同的情况下，推荐您优先使用v3接口。

