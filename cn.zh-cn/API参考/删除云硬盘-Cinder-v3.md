# 删除云硬盘<a name="zh-cn_topic_0102643091"></a>

## 功能介绍<a name="section10932885"></a>

删除一个云硬盘。

## URI<a name="section31287108"></a>

-   URI格式

    DELETE /v3/\{project\_id\}/volumes/\{volume\_id\}

-   参数说明

    <a name="table44522499"></a>
    <table><thead align="left"><tr id="row39474480"><th class="cellrowborder" valign="top" width="33.33%" id="mcps1.1.4.1.1"><p id="p43316293"><a name="p43316293"></a><a name="p43316293"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.549999999999997%" id="mcps1.1.4.1.2"><p id="p18958859"><a name="p18958859"></a><a name="p18958859"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.12%" id="mcps1.1.4.1.3"><p id="p59272617"><a name="p59272617"></a><a name="p59272617"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row36352712"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p194149447576"><a name="p194149447576"></a><a name="p194149447576"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.1.4.1.2 "><p id="p5246632"><a name="p5246632"></a><a name="p5246632"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.1.4.1.3 "><p id="p22324024"><a name="p22324024"></a><a name="p22324024"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row66698493"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p33868853"><a name="p33868853"></a><a name="p33868853"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.1.4.1.2 "><p id="p59022586"><a name="p59022586"></a><a name="p59022586"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.12%" headers="mcps1.1.4.1.3 "><p id="p16100147"><a name="p16100147"></a><a name="p16100147"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="zh-cn_topic_0058762428_table114096539515"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762428_row64913538519"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058762428_p14491115311514"><a name="zh-cn_topic_0058762428_p14491115311514"></a><a name="zh-cn_topic_0058762428_p14491115311514"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058762428_p54911753125116"><a name="zh-cn_topic_0058762428_p54911753125116"></a><a name="zh-cn_topic_0058762428_p54911753125116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.191919191919194%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058762428_p10491105315113"><a name="zh-cn_topic_0058762428_p10491105315113"></a><a name="zh-cn_topic_0058762428_p10491105315113"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.45454545454546%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058762428_p16491553125110"><a name="zh-cn_topic_0058762428_p16491553125110"></a><a name="zh-cn_topic_0058762428_p16491553125110"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762428_row64916530515"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762428_p14491953135112"><a name="zh-cn_topic_0058762428_p14491953135112"></a><a name="zh-cn_topic_0058762428_p14491953135112"></a>cascade</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762428_p15491185365111"><a name="zh-cn_topic_0058762428_p15491185365111"></a><a name="zh-cn_topic_0058762428_p15491185365111"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762428_p349155345117"><a name="zh-cn_topic_0058762428_p349155345117"></a><a name="zh-cn_topic_0058762428_p349155345117"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.45454545454546%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762428_p1941233905911"><a name="zh-cn_topic_0058762428_p1941233905911"></a><a name="zh-cn_topic_0058762428_p1941233905911"></a>删除云硬盘关联的所有快照，默认值为false。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section4146219482"></a>

以将云硬盘关联的快照一起删除为例。

-   请求样例

    ```
    DELETE https://{endpoint}/v3/{project_id}/volumes/{volume_id}?cascade=true
    ```


## 响应消息<a name="section51227795"></a>

-   响应参数

    <a name="zh-cn_topic_0058762428_table46654279102454"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762428_row6664264102454"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762428_p2934472102454"><a name="zh-cn_topic_0058762428_p2934472102454"></a><a name="zh-cn_topic_0058762428_p2934472102454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762428_p1338569102927"><a name="zh-cn_topic_0058762428_p1338569102927"></a><a name="zh-cn_topic_0058762428_p1338569102927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762428_p23036595102454"><a name="zh-cn_topic_0058762428_p23036595102454"></a><a name="zh-cn_topic_0058762428_p23036595102454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762428_row12419334102454"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762428_p129522216412"><a name="zh-cn_topic_0058762428_p129522216412"></a><a name="zh-cn_topic_0058762428_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762428_p1595262111415"><a name="zh-cn_topic_0058762428_p1595262111415"></a><a name="zh-cn_topic_0058762428_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762428_p109527215417"><a name="zh-cn_topic_0058762428_p109527215417"></a><a name="zh-cn_topic_0058762428_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#zh-cn_topic_0058762428_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058762428_li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0058762428_zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    无

    或

    ```
    {
        "error": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错：

    ```
    {
        "itemNotFound": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section58396974"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

