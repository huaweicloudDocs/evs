# 查询租户的详细配额<a name="ZH-CN_TOPIC_0102649601"></a>

## 功能介绍<a name="section9502070"></a>

查询租户的详细配额。

## URI<a name="section18409771"></a>

-   URI格式

    GET /v3/\{project\_id\}/os-quota-sets/\{project\_id\}?usage=True

-   参数说明

    <a name="table117163"></a>
    <table><thead align="left"><tr id="row55762700"><th class="cellrowborder" valign="top" width="33.33%" id="mcps1.1.4.1.1"><p id="p20484818"><a name="p20484818"></a><a name="p20484818"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.3%" id="mcps1.1.4.1.2"><p id="p48657561"><a name="p48657561"></a><a name="p48657561"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.370000000000005%" id="mcps1.1.4.1.3"><p id="p48948360"><a name="p48948360"></a><a name="p48948360"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5394248"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p34280961"><a name="p34280961"></a><a name="p34280961"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.3%" headers="mcps1.1.4.1.2 "><p id="p25294426"><a name="p25294426"></a><a name="p25294426"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.370000000000005%" headers="mcps1.1.4.1.3 "><p id="p35582587"><a name="p35582587"></a><a name="p35582587"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section31470215"></a>

无

## 响应<a name="section14796483"></a>

-   响应参数

    <a name="zh-cn_topic_0020235133_table42676787201620"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235133_row15715964201620"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235133_p65033611201620"><a name="zh-cn_topic_0020235133_p65033611201620"></a><a name="zh-cn_topic_0020235133_p65033611201620"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235133_p5090379315311"><a name="zh-cn_topic_0020235133_p5090379315311"></a><a name="zh-cn_topic_0020235133_p5090379315311"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235133_p1989612244512"><a name="zh-cn_topic_0020235133_p1989612244512"></a><a name="zh-cn_topic_0020235133_p1989612244512"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235133_row5954204616447"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p5817645816447"><a name="zh-cn_topic_0020235133_p5817645816447"></a><a name="zh-cn_topic_0020235133_p5817645816447"></a>quota_set</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p1467262516447"><a name="zh-cn_topic_0020235133_p1467262516447"></a><a name="zh-cn_topic_0020235133_p1467262516447"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p3298658216447"><a name="zh-cn_topic_0020235133_p3298658216447"></a><a name="zh-cn_topic_0020235133_p3298658216447"></a>查询请求返回的配额信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row60124619201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p38255980201620"><a name="zh-cn_topic_0020235133_p38255980201620"></a><a name="zh-cn_topic_0020235133_p38255980201620"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p2956653915311"><a name="zh-cn_topic_0020235133_p2956653915311"></a><a name="zh-cn_topic_0020235133_p2956653915311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p10336815201620"><a name="zh-cn_topic_0020235133_p10336815201620"></a><a name="zh-cn_topic_0020235133_p10336815201620"></a>云硬盘数量，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row25922478201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p19345972201620"><a name="zh-cn_topic_0020235133_p19345972201620"></a><a name="zh-cn_topic_0020235133_p19345972201620"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p4607944115311"><a name="zh-cn_topic_0020235133_p4607944115311"></a><a name="zh-cn_topic_0020235133_p4607944115311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p26061300201620"><a name="zh-cn_topic_0020235133_p26061300201620"></a><a name="zh-cn_topic_0020235133_p26061300201620"></a>快照数量，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row33225116201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p6879872201620"><a name="zh-cn_topic_0020235133_p6879872201620"></a><a name="zh-cn_topic_0020235133_p6879872201620"></a>gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p4144727715311"><a name="zh-cn_topic_0020235133_p4144727715311"></a><a name="zh-cn_topic_0020235133_p4144727715311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p41689235201620"><a name="zh-cn_topic_0020235133_p41689235201620"></a><a name="zh-cn_topic_0020235133_p41689235201620"></a>总大小（快照+云硬盘），单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row39658796201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p58245913201620"><a name="zh-cn_topic_0020235133_p58245913201620"></a><a name="zh-cn_topic_0020235133_p58245913201620"></a>volumes_TYPE</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p178624415311"><a name="zh-cn_topic_0020235133_p178624415311"></a><a name="zh-cn_topic_0020235133_p178624415311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p33568305201620"><a name="zh-cn_topic_0020235133_p33568305201620"></a><a name="zh-cn_topic_0020235133_p33568305201620"></a>为某个volume_type预留的云硬盘个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row33679293201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p43668237201620"><a name="zh-cn_topic_0020235133_p43668237201620"></a><a name="zh-cn_topic_0020235133_p43668237201620"></a>snapshots_TYPE</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p1046809615311"><a name="zh-cn_topic_0020235133_p1046809615311"></a><a name="zh-cn_topic_0020235133_p1046809615311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p19567167201620"><a name="zh-cn_topic_0020235133_p19567167201620"></a><a name="zh-cn_topic_0020235133_p19567167201620"></a>为某个volume_type预留快照个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row41886775201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p37385587201620"><a name="zh-cn_topic_0020235133_p37385587201620"></a><a name="zh-cn_topic_0020235133_p37385587201620"></a>gigabytes_TYPE</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p4260948115311"><a name="zh-cn_topic_0020235133_p4260948115311"></a><a name="zh-cn_topic_0020235133_p4260948115311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p3943730201620"><a name="zh-cn_topic_0020235133_p3943730201620"></a><a name="zh-cn_topic_0020235133_p3943730201620"></a>为某个volume_type预留的size大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row35493575201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p56407339201620"><a name="zh-cn_topic_0020235133_p56407339201620"></a><a name="zh-cn_topic_0020235133_p56407339201620"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p2881594215311"><a name="zh-cn_topic_0020235133_p2881594215311"></a><a name="zh-cn_topic_0020235133_p2881594215311"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p50275403201620"><a name="zh-cn_topic_0020235133_p50275403201620"></a><a name="zh-cn_topic_0020235133_p50275403201620"></a>租户id。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row49825446201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p9329306201620"><a name="zh-cn_topic_0020235133_p9329306201620"></a><a name="zh-cn_topic_0020235133_p9329306201620"></a>backups</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p5238998415311"><a name="zh-cn_topic_0020235133_p5238998415311"></a><a name="zh-cn_topic_0020235133_p5238998415311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p6295376201620"><a name="zh-cn_topic_0020235133_p6295376201620"></a><a name="zh-cn_topic_0020235133_p6295376201620"></a>备份个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row56658385201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p25926512201620"><a name="zh-cn_topic_0020235133_p25926512201620"></a><a name="zh-cn_topic_0020235133_p25926512201620"></a>backup_gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p1573030215311"><a name="zh-cn_topic_0020235133_p1573030215311"></a><a name="zh-cn_topic_0020235133_p1573030215311"></a>map&lt;string, int&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p49989712201620"><a name="zh-cn_topic_0020235133_p49989712201620"></a><a name="zh-cn_topic_0020235133_p49989712201620"></a>备份大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row47254225201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p2387045201620"><a name="zh-cn_topic_0020235133_p2387045201620"></a><a name="zh-cn_topic_0020235133_p2387045201620"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p6619495315311"><a name="zh-cn_topic_0020235133_p6619495315311"></a><a name="zh-cn_topic_0020235133_p6619495315311"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p25040226201620"><a name="zh-cn_topic_0020235133_p25040226201620"></a><a name="zh-cn_topic_0020235133_p25040226201620"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235133_row24035444201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235133_p713975201620"><a name="zh-cn_topic_0020235133_p713975201620"></a><a name="zh-cn_topic_0020235133_p713975201620"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235133_p6019095215311"><a name="zh-cn_topic_0020235133_p6019095215311"></a><a name="zh-cn_topic_0020235133_p6019095215311"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235133_p53879909201620"><a name="zh-cn_topic_0020235133_p53879909201620"></a><a name="zh-cn_topic_0020235133_p53879909201620"></a>出现错误时，返回的错误码，具体含义参考下面的返回值列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果返回值中limit为-1，表示没有限制配额。  

-   响应样例

    ```
    {
        "quota_set": {
            "gigabytes_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 21
            }, 
            "volumes_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 8
            }, 
            "gigabytes": {
                "reserved": 0, 
                "limit": 42790, 
                "in_use": 2792
            }, 
            "backup_gigabytes": {
                "reserved": 0, 
                "limit": 5120, 
                "in_use": 51
            }, 
            "snapshots_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 28
            }, 
            "snapshots": {
                "reserved": 0, 
                "limit": 10, 
                "in_use": 6
            }, 
            "id": "cd631140887d4b6e9c786b67a6dd4c02", 
            "volumes_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 2
            }, 
            "snapshots_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 108
            }, 
            "gigabytes_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 168
            }, 
            "backups": {
                "reserved": 0, 
                "limit": 100, 
                "in_use": 10
            }, 
            "gigabytes_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 1085
            }, 
            "snapshots_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }
        }
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

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错为：

    ```
    {
        "badrequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 返回值<a name="section66059488"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

