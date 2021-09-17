# 查询扩展接口<a name="evs_04_3044"></a>

## 功能介绍<a name="section19390540"></a>

查询扩展接口。

## URI<a name="section40297137"></a>

-   URI格式

    GET /v3/\{project\_id\}/extensions

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="28.49%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.5%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="28.49%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.5%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section27129916"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v3/{project_id}/extensions
    ```


## 响应消息<a name="section42842654"></a>

-   响应参数

    <a name="evs_04_2080_table11977025201856"></a>
    <table><thead align="left"><tr id="evs_04_2080_row8102228201856"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2080_p52300707201856"><a name="evs_04_2080_p52300707201856"></a><a name="evs_04_2080_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_2080_p3642697315541"><a name="evs_04_2080_p3642697315541"></a><a name="evs_04_2080_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2080_p17319263201856"><a name="evs_04_2080_p17319263201856"></a><a name="evs_04_2080_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2080_row60683035201856"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p16378828201856"><a name="evs_04_2080_p16378828201856"></a><a name="evs_04_2080_p16378828201856"></a>extensions</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p6490369115541"><a name="evs_04_2080_p6490369115541"></a><a name="evs_04_2080_p6490369115541"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p20205612201856"><a name="evs_04_2080_p20205612201856"></a><a name="evs_04_2080_p20205612201856"></a>扩展接口列表，请参见<a href="#evs_04_2080_li35330737222812">•extensions参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2080_row18487163602815"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p129522216412"><a name="evs_04_2080_p129522216412"></a><a name="evs_04_2080_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p1595262111415"><a name="evs_04_2080_p1595262111415"></a><a name="evs_04_2080_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p109527215417"><a name="evs_04_2080_p109527215417"></a><a name="evs_04_2080_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2080_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2080_li35330737222812"></a>extensions参数说明

    <a name="evs_04_2080_table49541177222812"></a>
    <table><thead align="left"><tr id="evs_04_2080_row31307356222812"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.1.4.1.1"><p id="evs_04_2080_p52867918222812"><a name="evs_04_2080_p52867918222812"></a><a name="evs_04_2080_p52867918222812"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.66%" id="mcps1.1.4.1.2"><p id="evs_04_2080_p54442989222812"><a name="evs_04_2080_p54442989222812"></a><a name="evs_04_2080_p54442989222812"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2080_p47079504222812"><a name="evs_04_2080_p47079504222812"></a><a name="evs_04_2080_p47079504222812"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2080_row55343460222812"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p66542884171033"><a name="evs_04_2080_p66542884171033"></a><a name="evs_04_2080_p66542884171033"></a>updated</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p21264523171033"><a name="evs_04_2080_p21264523171033"></a><a name="evs_04_2080_p21264523171033"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p172841210852"><a name="evs_04_2080_p172841210852"></a><a name="evs_04_2080_p172841210852"></a>最后的更新时间。</p>
    <p id="evs_04_2080_p64318586171033"><a name="evs_04_2080_p64318586171033"></a><a name="evs_04_2080_p64318586171033"></a><span id="evs_04_2080_text15197123457"><a name="evs_04_2080_text15197123457"></a><a name="evs_04_2080_text15197123457"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.+XX.XX，其中+XX.XX表示时区。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2080_row49897554222812"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p46262636171033"><a name="evs_04_2080_p46262636171033"></a><a name="evs_04_2080_p46262636171033"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p56285996171033"><a name="evs_04_2080_p56285996171033"></a><a name="evs_04_2080_p56285996171033"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p59451065171033"><a name="evs_04_2080_p59451065171033"></a><a name="evs_04_2080_p59451065171033"></a>描述。</p>
    </td>
    </tr>
    <tr id="evs_04_2080_row15692876222812"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p54609812171033"><a name="evs_04_2080_p54609812171033"></a><a name="evs_04_2080_p54609812171033"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p44048737191438"><a name="evs_04_2080_p44048737191438"></a><a name="evs_04_2080_p44048737191438"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p61224008171033"><a name="evs_04_2080_p61224008171033"></a><a name="evs_04_2080_p61224008171033"></a><span id="evs_04_2080_text658942018365"><a name="evs_04_2080_text658942018365"></a><a name="evs_04_2080_text658942018365"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2080_row23073040222812"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p19600405171033"><a name="evs_04_2080_p19600405171033"></a><a name="evs_04_2080_p19600405171033"></a>alias</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p44128957171033"><a name="evs_04_2080_p44128957171033"></a><a name="evs_04_2080_p44128957171033"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p22448926171033"><a name="evs_04_2080_p22448926171033"></a><a name="evs_04_2080_p22448926171033"></a>云硬盘扩展参数的别名。</p>
    </td>
    </tr>
    <tr id="evs_04_2080_row52652485222812"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_p57813479171033"><a name="evs_04_2080_p57813479171033"></a><a name="evs_04_2080_p57813479171033"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.66%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_p52380208171033"><a name="evs_04_2080_p52380208171033"></a><a name="evs_04_2080_p52380208171033"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_p2055232171033"><a name="evs_04_2080_p2055232171033"></a><a name="evs_04_2080_p2055232171033"></a>云硬盘扩展参数的名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2080_li0419202382514"></a>error参数说明

    <a name="evs_04_2080_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2080_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2080_evs_04_2013_p19541716103019"><a name="evs_04_2080_evs_04_2013_p19541716103019"></a><a name="evs_04_2080_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2080_evs_04_2013_p39375186103019"><a name="evs_04_2080_evs_04_2013_p39375186103019"></a><a name="evs_04_2080_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2080_evs_04_2013_p38578950103019"><a name="evs_04_2080_evs_04_2013_p38578950103019"></a><a name="evs_04_2080_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2080_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_evs_04_2013_p46815658103019"><a name="evs_04_2080_evs_04_2013_p46815658103019"></a><a name="evs_04_2080_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_evs_04_2013_p33971979103019"><a name="evs_04_2080_evs_04_2013_p33971979103019"></a><a name="evs_04_2080_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_evs_04_2013_p21623243103019"><a name="evs_04_2080_evs_04_2013_p21623243103019"></a><a name="evs_04_2080_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2080_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2080_evs_04_2013_p59870541103019"><a name="evs_04_2080_evs_04_2013_p59870541103019"></a><a name="evs_04_2080_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2080_evs_04_2013_p17675690103019"><a name="evs_04_2080_evs_04_2013_p17675690103019"></a><a name="evs_04_2080_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2080_evs_04_2013_p6087468103019"><a name="evs_04_2080_evs_04_2013_p6087468103019"></a><a name="evs_04_2080_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2080_evs_04_2013_p54787218103019"><a name="evs_04_2080_evs_04_2013_p54787218103019"></a><a name="evs_04_2080_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "extensions": [
            {
                "updated": "2013-04-18T00:00:00+00:00", 
                "name": "SchedulerHints", 
                "links": [ ], 
                "alias": "OS-SCH-HNT", 
                "description": "Pass arbitrary key/value pairs to the scheduler."
            }, 
            {
                "updated": "2011-06-29T00:00:00+00:00", 
                "name": "Hosts", 
                "links": [ ], 
                "alias": "os-hosts", 
                "description": "Admin-only host administration."
            }, 
            {
                "updated": "2011-11-03T00:00:00+00:00", 
                "name": "VolumeTenantAttribute", 
                "links": [ ], 
                "alias": "os-vol-tenant-attr", 
                "description": "Expose the internal project_id as an attribute of a volume."
            }, 
            {
                "updated": "2011-08-08T00:00:00+00:00", 
                "name": "Quotas", 
                "links": [ ], 
                "alias": "os-quota-sets", 
                "description": "Quota management support."
            }, 
            {
                "updated": "2011-08-24T00:00:00+00:00", 
                "name": "TypesManage", 
                "links": [ ], 
                "alias": "os-types-manage", 
                "description": "Types manage support."
            }, 
            {
                "updated": "2013-07-10T00:00:00+00:00", 
                "name": "VolumeEncryptionMetadata", 
                "links": [ ], 
                "alias": "os-volume-encryption-metadata", 
                "description": "Volume encryption metadata retrieval support."
            }, 
            {
                "updated": "2012-12-12T00:00:00+00:00", 
                "name": "Backups", 
                "links": [ ], 
                "alias": "backups", 
                "description": "Backups support."
            }, 
            {
                "updated": "2013-07-16T00:00:00+00:00", 
                "name": "SnapshotActions", 
                "links": [ ], 
                "alias": "os-snapshot-actions", 
                "description": "Enable snapshot manager actions."
            }, 
            {
                "updated": "2012-05-31T00:00:00+00:00", 
                "name": "VolumeActions", 
                "links": [ ], 
                "alias": "os-volume-actions", 
                "description": "Enable volume actions
        "
            }, 
            {
                "updated": "2013-10-03T00:00:00+00:00", 
                "name": "UsedLimits", 
                "links": [ ], 
                "alias": "os-used-limits", 
                "description": "Provide data on limited resources that are being used."
            }, 
            {
                "updated": "2012-05-31T00:00:00+00:00", 
                "name": "VolumeUnmanage", 
                "links": [ ], 
                "alias": "os-volume-unmanage", 
                "description": "Enable volume unmanage operation."
            }, 
            {
                "updated": "2011-11-03T00:00:00+00:00", 
                "name": "VolumeHostAttribute", 
                "links": [ ], 
                "alias": "os-vol-host-attr", 
                "description": "Expose host as an attribute of a volume."
            }, 
            {
                "updated": "2013-07-01T00:00:00+00:00", 
                "name": "VolumeTypeEncryption", 
                "links": [ ], 
                "alias": "encryption", 
                "description": "Encryption support for volume types."
            }, 
            {
                "updated": "2013-06-27T00:00:00+00:00", 
                "name": "AvailabilityZones", 
                "links": [ ], 
                "alias": "os-availability-zone", 
                "description": "Describe Availability Zones."
            }, 
            {
                "updated": "2013-08-02T00:00:00+00:00", 
                "name": "Qos_specs_manage", 
                "links": [ ], 
                "alias": "qos-specs", 
                "description": "QoS specs support."
            }, 
            {
                "updated": "2011-08-24T00:00:00+00:00", 
                "name": "TypesExtraSpecs", 
                "links": [ ], 
                "alias": "os-types-extra-specs", 
                "description": "Type extra specs support."
            }, 
            {
                "updated": "2013-08-08T00:00:00+00:00", 
                "name": "VolumeMigStatusAttribute", 
                "links": [ ],  
                "alias": "os-vol-mig-status-attr", 
                "description": "Expose migration_status as an attribute of a volume."
            }, 
            {
                "updated": "2012-08-13T00:00:00+00:00", 
                "name": "CreateVolumeExtension", 
                "links": [ ], 
                "alias": "os-image-create", 
                "description": "Allow creating a volume from an image in the Create Volume v1 API."
            }, 
            {
                "updated": "2014-01-10T00:00:00-00:00", 
                "name": "ExtendedServices", 
                "links": [ ],  
                "alias": "os-extended-services", 
                "description": "Extended services support."
            }, 
            {
                "updated": "2012-06-19T00:00:00+00:00", 
                "name": "ExtendedSnapshotAttributes", 
                "links": [ ], 
                "alias": "os-extended-snapshot-attributes", 
                "description": "Extended SnapshotAttributes support."
            }, 
            {
                "updated": "2012-12-07T00:00:00+00:00", 
                "name": "VolumeImageMetadata", 
                "links": [ ], 
                "alias": "os-vol-image-meta", 
                "description": "Show image metadata associated with the volume."
            }, 
            {
                "updated": "2012-03-12T00:00:00+00:00", 
                "name": "QuotaClasses", 
                "links": [ ], 
                "alias": "os-quota-class-sets", 
                "description": "Quota classes management support."
            }, 
            {
                "updated": "2013-05-29T00:00:00+00:00", 
                "name": "VolumeTransfer", 
                "links": [ ], 
                "alias": "os-volume-transfer", 
                "description": "Volume transfer management support."
            }, 
            {
                "updated": "2014-02-10T00:00:00+00:00", 
                "name": "VolumeManage", 
                "links": [ ],  
                "alias": "os-volume-manage", 
                "description": "Allows existing backend storage to be 'managed' by Cinder."
            }, 
            {
                "updated": "2012-08-25T00:00:00+00:00", 
                "name": "AdminActions", 
                "links": [ ],  
                "alias": "os-admin-actions", 
                "description": "Enable admin actions."
            }, 
            {
                "updated": "2012-10-28T00:00:00-00:00", 
                "name": "Services", 
                "links": [ ],  
                "alias": "os-services", 
                "description": "Services support."
            }
        ]
    }
    ```

    或

    ```
    {
        "error": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

    ```
    {
        "badRequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section50039568"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

