# 查询单个云硬盘类型的详细信息<a name="ZH-CN_TOPIC_0102648469"></a>

## 功能介绍<a name="section48630964"></a>

查询单个云硬盘类型的详细信息。

## URI<a name="section35025494"></a>

-   URI格式

    GET /v3/\{project\_id\}/types/\{type\_id\}

-   参数说明

    <a name="table3865173"></a>
    <table><thead align="left"><tr id="row43603258"><th class="cellrowborder" valign="top" width="29.25%" id="mcps1.1.4.1.1"><p id="p42202994"><a name="p42202994"></a><a name="p42202994"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="25.009999999999998%" id="mcps1.1.4.1.2"><p id="p62999330"><a name="p62999330"></a><a name="p62999330"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.739999999999995%" id="mcps1.1.4.1.3"><p id="p2672115"><a name="p2672115"></a><a name="p2672115"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15114764"><td class="cellrowborder" valign="top" width="29.25%" headers="mcps1.1.4.1.1 "><p id="p16336406"><a name="p16336406"></a><a name="p16336406"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.009999999999998%" headers="mcps1.1.4.1.2 "><p id="p48180537"><a name="p48180537"></a><a name="p48180537"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.739999999999995%" headers="mcps1.1.4.1.3 "><p id="p10309404"><a name="p10309404"></a><a name="p10309404"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row25675773"><td class="cellrowborder" valign="top" width="29.25%" headers="mcps1.1.4.1.1 "><p id="p66471715"><a name="p66471715"></a><a name="p66471715"></a>type_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="25.009999999999998%" headers="mcps1.1.4.1.2 "><p id="p15499871"><a name="p15499871"></a><a name="p15499871"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.739999999999995%" headers="mcps1.1.4.1.3 "><p id="p47530006"><a name="p47530006"></a><a name="p47530006"></a>云硬盘类型ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section46793998"></a>

无

## 响应<a name="section18492804"></a>

-   响应参数

    <a name="zh-cn_topic_0020235132_table6170753515253"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235132_row4217445215253"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235132_p6068742915253"><a name="zh-cn_topic_0020235132_p6068742915253"></a><a name="zh-cn_topic_0020235132_p6068742915253"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235132_p1673474815253"><a name="zh-cn_topic_0020235132_p1673474815253"></a><a name="zh-cn_topic_0020235132_p1673474815253"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235132_p658034115253"><a name="zh-cn_topic_0020235132_p658034115253"></a><a name="zh-cn_topic_0020235132_p658034115253"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235132_row5525086316333"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p4613490816333"><a name="zh-cn_topic_0020235132_p4613490816333"></a><a name="zh-cn_topic_0020235132_p4613490816333"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p4594004916333"><a name="zh-cn_topic_0020235132_p4594004916333"></a><a name="zh-cn_topic_0020235132_p4594004916333"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p2675768516333"><a name="zh-cn_topic_0020235132_p2675768516333"></a><a name="zh-cn_topic_0020235132_p2675768516333"></a>查询请求返回的云硬盘类型。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row6324564115253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p2262329715253"><a name="zh-cn_topic_0020235132_p2262329715253"></a><a name="zh-cn_topic_0020235132_p2262329715253"></a>extra_specs</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p2054778215253"><a name="zh-cn_topic_0020235132_p2054778215253"></a><a name="zh-cn_topic_0020235132_p2054778215253"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p5940085315253"><a name="zh-cn_topic_0020235132_p5940085315253"></a><a name="zh-cn_topic_0020235132_p5940085315253"></a>云硬盘类型的规格。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row6484563015253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p1800464915253"><a name="zh-cn_topic_0020235132_p1800464915253"></a><a name="zh-cn_topic_0020235132_p1800464915253"></a>volume_backend_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p4909046915253"><a name="zh-cn_topic_0020235132_p4909046915253"></a><a name="zh-cn_topic_0020235132_p4909046915253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p2713175815253"><a name="zh-cn_topic_0020235132_p2713175815253"></a><a name="zh-cn_topic_0020235132_p2713175815253"></a>Cinder后端的云硬盘类型名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row4285923615253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p4904612515253"><a name="zh-cn_topic_0020235132_p4904612515253"></a><a name="zh-cn_topic_0020235132_p4904612515253"></a>availability-zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p1331319415253"><a name="zh-cn_topic_0020235132_p1331319415253"></a><a name="zh-cn_topic_0020235132_p1331319415253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p3923849815253"><a name="zh-cn_topic_0020235132_p3923849815253"></a><a name="zh-cn_topic_0020235132_p3923849815253"></a>可用分区。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row1760216615253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p1648936615253"><a name="zh-cn_topic_0020235132_p1648936615253"></a><a name="zh-cn_topic_0020235132_p1648936615253"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p6057028715253"><a name="zh-cn_topic_0020235132_p6057028715253"></a><a name="zh-cn_topic_0020235132_p6057028715253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p5006999315253"><a name="zh-cn_topic_0020235132_p5006999315253"></a><a name="zh-cn_topic_0020235132_p5006999315253"></a>云硬盘类型名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row4797675615253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p6091205315253"><a name="zh-cn_topic_0020235132_p6091205315253"></a><a name="zh-cn_topic_0020235132_p6091205315253"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p3492929915253"><a name="zh-cn_topic_0020235132_p3492929915253"></a><a name="zh-cn_topic_0020235132_p3492929915253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p6147315615253"><a name="zh-cn_topic_0020235132_p6147315615253"></a><a name="zh-cn_topic_0020235132_p6147315615253"></a>云硬盘类型的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row29065010162354"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p42044028162413"><a name="zh-cn_topic_0020235132_p42044028162413"></a><a name="zh-cn_topic_0020235132_p42044028162413"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p50123125162413"><a name="zh-cn_topic_0020235132_p50123125162413"></a><a name="zh-cn_topic_0020235132_p50123125162413"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p24390255162413"><a name="zh-cn_topic_0020235132_p24390255162413"></a><a name="zh-cn_topic_0020235132_p24390255162413"></a>云硬盘类型的描述信息</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row18405511162410"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p63756107162413"><a name="zh-cn_topic_0020235132_p63756107162413"></a><a name="zh-cn_topic_0020235132_p63756107162413"></a>qos_specs_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p63971081162413"><a name="zh-cn_topic_0020235132_p63971081162413"></a><a name="zh-cn_topic_0020235132_p63971081162413"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p15431098162413"><a name="zh-cn_topic_0020235132_p15431098162413"></a><a name="zh-cn_topic_0020235132_p15431098162413"></a>云硬盘类型对应的qos的id</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row4485204316243"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p42090474162413"><a name="zh-cn_topic_0020235132_p42090474162413"></a><a name="zh-cn_topic_0020235132_p42090474162413"></a>is_public</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p53885223162413"><a name="zh-cn_topic_0020235132_p53885223162413"></a><a name="zh-cn_topic_0020235132_p53885223162413"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p11454306162413"><a name="zh-cn_topic_0020235132_p11454306162413"></a><a name="zh-cn_topic_0020235132_p11454306162413"></a>是否是public类型</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row1638749515253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p5231875615253"><a name="zh-cn_topic_0020235132_p5231875615253"></a><a name="zh-cn_topic_0020235132_p5231875615253"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p996083315253"><a name="zh-cn_topic_0020235132_p996083315253"></a><a name="zh-cn_topic_0020235132_p996083315253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p5610239615253"><a name="zh-cn_topic_0020235132_p5610239615253"></a><a name="zh-cn_topic_0020235132_p5610239615253"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row3515952115253"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p2934893015253"><a name="zh-cn_topic_0020235132_p2934893015253"></a><a name="zh-cn_topic_0020235132_p2934893015253"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p2845316115253"><a name="zh-cn_topic_0020235132_p2845316115253"></a><a name="zh-cn_topic_0020235132_p2845316115253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p5143875415253"><a name="zh-cn_topic_0020235132_p5143875415253"></a><a name="zh-cn_topic_0020235132_p5143875415253"></a>出现错误时，返回的错误码，具体含义参考下面的返回值列表。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row7784432195610"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p1295213583815"><a name="zh-cn_topic_0020235132_p1295213583815"></a><a name="zh-cn_topic_0020235132_p1295213583815"></a>RESKEY:availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p8568345124512"><a name="zh-cn_topic_0020235132_p8568345124512"></a><a name="zh-cn_topic_0020235132_p8568345124512"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p795218533813"><a name="zh-cn_topic_0020235132_p795218533813"></a><a name="zh-cn_topic_0020235132_p795218533813"></a>支持当前云硬盘类型的AZ列表</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235132_row735762912563"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235132_p763817813812"><a name="zh-cn_topic_0020235132_p763817813812"></a><a name="zh-cn_topic_0020235132_p763817813812"></a>os-vendor-extended:sold_out_availability_zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235132_p1921554784510"><a name="zh-cn_topic_0020235132_p1921554784510"></a><a name="zh-cn_topic_0020235132_p1921554784510"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235132_p927131553911"><a name="zh-cn_topic_0020235132_p927131553911"></a><a name="zh-cn_topic_0020235132_p927131553911"></a>当前云硬盘类型售罄的AZ列表</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
        "volume_type": { 
            "extra_specs": { 
                "volume_backend_name": "SATA",  
                "availability-zone": "az1.dc1",  
                "RESKEY:availability_zone": "az1.dc1,az2.dc2",  
                "os-vendor-extended:sold_out_availability_zones": "az2.dc2"
            },  
            "name": "SATA",  
            "qos_specs_id": null,  
            "is_public": true,  
            "id": "ea6e3c13-aac5-46e0-b280-745ed272e662",  
            "description": null 
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


## 返回值<a name="section32217513"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

