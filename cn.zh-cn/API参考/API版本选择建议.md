# API版本选择建议<a name="ZH-CN_TOPIC_0174575298"></a>

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

## 微版本号介绍及使用说明<a name="section1373175211"></a>

微版本说明：当使用v3版本的OpenStack Cinder API时，您可以指定微版本号以此获取服务支持的最新API微版本，通过版本信息查询接口，可以查询当前支持的主版本、支持的最大与最小的微版本。

当前OpenStack Cinder API的版本号默认为3.0，最大版本号为3.50。v3版本的OpenStack Cinder API中有个别参数依赖微版本号，详细信息已在参数说明中介绍。

微版本使用方法：用户想要使用微版本特性，需要在请求OpenStack Cinder API时，在请求头中加入微版本头：Openstack-API-Version。

例如使用微版本3.50时，需要在https的请求头中加入：OpenStack-API-Version:volume 3.50

## 微版本请求样例<a name="section953273282314"></a>

假设使用云硬盘详情API查询“count”字段。

-   使用v3接口，不加微版本号
    -   GET: https://_\{endpoint\}_/v3/ba546eb46e7247c9aadb566ed7a1d31f/volumes/detail?with\_count=true

        \{endpoint\}信息请参见[终端节点](终端节点.md)获取。

    -   Headers:

        <a name="table19387710"></a>
        <table><tbody><tr id="row14795382"><td class="cellrowborder" valign="top" width="50%"><p id="p57575265"><a name="p57575265"></a><a name="p57575265"></a>Content-Type</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%"><p id="p33084893"><a name="p33084893"></a><a name="p33084893"></a>application/json</p>
        </td>
        </tr>
        <tr id="row29328585"><td class="cellrowborder" valign="top" width="50%"><p id="p26805152"><a name="p26805152"></a><a name="p26805152"></a>X-Auth-Token</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%"><p id="p23733724"><a name="p23733724"></a><a name="p23733724"></a>${token}</p>
        </td>
        </tr>
        </tbody>
        </table>

    -   响应消息体：

        ```
        {
            "volumes": [
                {
                    "attachments": [ ], 
                    "availability_zone": "az-dc-1", 
                    "bootable": "false", 
                    "consistencygroup_id": null, 
                    "created_at": "2016-05-25T02:42:10.856332", 
                    "description": null, 
                    "encrypted": false, 
                    "id": "b104b8db-170d-441b-897a-3c8ba9c5a214", 
                    "links": [
                        {
                            "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                            "rel": "self"
                        }, 
                        {
                            "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                            "rel": "bookmark"
                        }
                    ], 
                    "metadata": {}, 
                    "name": "zjb_u25_test", 
                    "os-vol-host-attr:host": "pod01.xxx#SATA", 
                    "volume_image_metadata": { }, 
                    "os-vol-mig-status-attr:migstat": null, 
                    "os-vol-mig-status-attr:name_id": null, 
                    "os-vol-tenant-attr:tenant_id": "dd14c6ac581f40059e27f5320b60bf2f",  
                    "replication_status": "disabled", 
                    "multiattach": false, 
                    "size": 1, 
                    "snapshot_id": null, 
                    "source_volid": null, 
                    "status": "available", 
                    "updated_at": "2016-05-25T02:42:22.341984", 
                    "user_id": "b0524e8342084ef5b74f158f78fc3049", 
                    "volume_type": "SATA"
                }
            ], 
            "volumes_links": [
                {
                    "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/detail?limit=1&marker=b104b8db-170d-441b-897a-3c8ba9c5a214", 
                    "rel": "next"
                }
            ]
        }
        ```

    -   结论：响应消息体中没有“count”字段。


-   使用v3接口，加微版本号
    -   GET: https://_\{endpoint\}_/v3/ba546eb46e7247c9aadb566ed7a1d31f/volumes/detail?with\_count=true

        \{endpoint\}信息请参见[终端节点](终端节点.md)获取。

    -   Headers:

        <a name="table072614264116"></a>
        <table><tbody><tr id="row117861542194113"><td class="cellrowborder" valign="top" width="50%"><p id="p1178764217417"><a name="p1178764217417"></a><a name="p1178764217417"></a>Content-Type</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%"><p id="p107871542134119"><a name="p107871542134119"></a><a name="p107871542134119"></a>application/json</p>
        </td>
        </tr>
        <tr id="row57879428414"><td class="cellrowborder" valign="top" width="50%"><p id="p57871342134116"><a name="p57871342134116"></a><a name="p57871342134116"></a>X-Auth-Token</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%"><p id="p978711422417"><a name="p978711422417"></a><a name="p978711422417"></a>${token}</p>
        </td>
        </tr>
        <tr id="row678714427416"><td class="cellrowborder" valign="top" width="50%"><p id="p478734284119"><a name="p478734284119"></a><a name="p478734284119"></a>Openstack-Api-Version</p>
        </td>
        <td class="cellrowborder" valign="top" width="50%"><p id="p167874425416"><a name="p167874425416"></a><a name="p167874425416"></a>volume 3.45</p>
        </td>
        </tr>
        </tbody>
        </table>

    -   响应消息体：

        ```
        {
            "count": 1, 
            "volumes": [
                {
                    "attachments": [ ], 
                    "availability_zone": "az-dc-1", 
                    "bootable": "false", 
                    "consistencygroup_id": null, 
                    "created_at": "2016-05-25T02:42:10.856332", 
                    "description": null, 
                    "encrypted": false, 
                    "id": "b104b8db-170d-441b-897a-3c8ba9c5a214", 
                    "links": [
                        {
                            "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                            "rel": "self"
                        }, 
                        {
                            "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                            "rel": "bookmark"
                        }
                    ], 
                    "metadata": {}, 
                    "name": "zjb_u25_test", 
                    "os-vol-host-attr:host": "pod01.xxx#SATA", 
                    "volume_image_metadata": { }, 
                    "os-vol-mig-status-attr:migstat": null, 
                    "os-vol-mig-status-attr:name_id": null, 
                    "os-vol-tenant-attr:tenant_id": "dd14c6ac581f40059e27f5320b60bf2f", 
                    "os-volume-replication:driver_data": null, 
                    "replication_status": "disabled", 
                    "multiattach": false, 
                    "size": 1, 
                    "snapshot_id": null, 
                    "source_volid": null, 
                    "status": "available", 
                    "updated_at": "2016-05-25T02:42:22.341984", 
                    "user_id": "b0524e8342084ef5b74f158f78fc3049", 
                    "volume_type": "SATA"
                }
            ], 
            "volumes_links": [
                {
                    "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/detail?limit=1&marker=b104b8db-170d-441b-897a-3c8ba9c5a214", 
                    "rel": "next"
                }
            ]
        }
        ```

    -   结论：响应消息体中有“count”字段。


