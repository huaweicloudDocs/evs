# 更新云硬盘快照的元数据<a name="zh-cn_topic_0102722795"></a>

## 功能介绍<a name="section4805694511340"></a>

更新云硬盘快照的元数据。

## URI<a name="section268627411340"></a>

-   URI格式

    PUT /v3/\{project\_id\}/snapshots/\{snapshot\_id\}/metadata

-   参数说明

    <a name="table5655293911340"></a>
    <table><thead align="left"><tr id="row4718979611340"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p6427715211340"><a name="p6427715211340"></a><a name="p6427715211340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p3906685711340"><a name="p3906685711340"></a><a name="p3906685711340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1029885411340"><a name="p1029885411340"></a><a name="p1029885411340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2890086411340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p5926863811340"><a name="p5926863811340"></a><a name="p5926863811340"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3603037711340"><a name="p3603037711340"></a><a name="p3603037711340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p3277940011340"><a name="p3277940011340"></a><a name="p3277940011340"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row2657914711340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p542726811340"><a name="p542726811340"></a><a name="p542726811340"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3695552511340"><a name="p3695552511340"></a><a name="p3695552511340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4060754311340"><a name="p4060754311340"></a><a name="p4060754311340"></a>快照ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section87667311340"></a>

-   请求参数

    <a name="zh-cn_topic_0058626635_table31588048"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626635_row57330849"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626635_p13287175"><a name="zh-cn_topic_0058626635_p13287175"></a><a name="zh-cn_topic_0058626635_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626635_p2519427"><a name="zh-cn_topic_0058626635_p2519427"></a><a name="zh-cn_topic_0058626635_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626635_p2747002"><a name="zh-cn_topic_0058626635_p2747002"></a><a name="zh-cn_topic_0058626635_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626635_p21180630"><a name="zh-cn_topic_0058626635_p21180630"></a><a name="zh-cn_topic_0058626635_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626635_row53167494153413"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626635_p11599783153413"><a name="zh-cn_topic_0058626635_p11599783153413"></a><a name="zh-cn_topic_0058626635_p11599783153413"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626635_p58405153413"><a name="zh-cn_topic_0058626635_p58405153413"></a><a name="zh-cn_topic_0058626635_p58405153413"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626635_p4730855153413"><a name="zh-cn_topic_0058626635_p4730855153413"></a><a name="zh-cn_topic_0058626635_p4730855153413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626635_p47654998153413"><a name="zh-cn_topic_0058626635_p47654998153413"></a><a name="zh-cn_topic_0058626635_p47654998153413"></a>需要更新的元数据信息，请参见<a href="#zh-cn_topic_0058626635_li54973602211845">•metadata参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058626635_li54973602211845"></a>metadata参数说明

    <a name="zh-cn_topic_0058626635_table32717123212358"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626635_row2280240212358"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626635_p50481723212358"><a name="zh-cn_topic_0058626635_p50481723212358"></a><a name="zh-cn_topic_0058626635_p50481723212358"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626635_p62487767212358"><a name="zh-cn_topic_0058626635_p62487767212358"></a><a name="zh-cn_topic_0058626635_p62487767212358"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626635_p28344363212358"><a name="zh-cn_topic_0058626635_p28344363212358"></a><a name="zh-cn_topic_0058626635_p28344363212358"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626635_p14192096212358"><a name="zh-cn_topic_0058626635_p14192096212358"></a><a name="zh-cn_topic_0058626635_p14192096212358"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626635_row8709150212358"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626635_p34352524212358"><a name="zh-cn_topic_0058626635_p34352524212358"></a><a name="zh-cn_topic_0058626635_p34352524212358"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626635_p31091026212358"><a name="zh-cn_topic_0058626635_p31091026212358"></a><a name="zh-cn_topic_0058626635_p31091026212358"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626635_p35345177212358"><a name="zh-cn_topic_0058626635_p35345177212358"></a><a name="zh-cn_topic_0058626635_p35345177212358"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626635_p44387080212358"><a name="zh-cn_topic_0058626635_p44387080212358"></a><a name="zh-cn_topic_0058626635_p44387080212358"></a>一个或多个键值对形式的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "metadata": {
            "key1": "value1", 
            "key2": "value2"
        }
    }
    ```


## 响应消息<a name="section5147449911340"></a>

-   响应参数

    <a name="zh-cn_topic_0058626635_table11977025201856"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626635_row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626635_p52300707201856"><a name="zh-cn_topic_0058626635_p52300707201856"></a><a name="zh-cn_topic_0058626635_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626635_p3642697315541"><a name="zh-cn_topic_0058626635_p3642697315541"></a><a name="zh-cn_topic_0058626635_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626635_p17319263201856"><a name="zh-cn_topic_0058626635_p17319263201856"></a><a name="zh-cn_topic_0058626635_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626635_row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626635_p16378828201856"><a name="zh-cn_topic_0058626635_p16378828201856"></a><a name="zh-cn_topic_0058626635_p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626635_p6490369115541"><a name="zh-cn_topic_0058626635_p6490369115541"></a><a name="zh-cn_topic_0058626635_p6490369115541"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626635_p20205612201856"><a name="zh-cn_topic_0058626635_p20205612201856"></a><a name="zh-cn_topic_0058626635_p20205612201856"></a>键值对，云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058626635_row2012491218193"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626635_p129522216412"><a name="zh-cn_topic_0058626635_p129522216412"></a><a name="zh-cn_topic_0058626635_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626635_p1595262111415"><a name="zh-cn_topic_0058626635_p1595262111415"></a><a name="zh-cn_topic_0058626635_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626635_p109527215417"><a name="zh-cn_topic_0058626635_p109527215417"></a><a name="zh-cn_topic_0058626635_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#zh-cn_topic_0058626635_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058626635_li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0058626635_zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "metadata": {
            "key1": "value1", 
            "key2": "value2"
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

    ```
    {
        "badRequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section1751558211340"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

