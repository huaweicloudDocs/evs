# 查询单个云硬盘过户记录详情<a name="evs_04_3072"></a>

## 功能介绍<a name="zh-cn_topic_0092902035_section44805042171914"></a>

查询单个云硬盘的过户记录详情，比如过户记录创建时间、ID以及名称等信息。

## URI<a name="zh-cn_topic_0092887872_section21748494171940"></a>

-   URI格式

    GET /v3/\{project\_id\}/os-volume-transfer/\{transfer\_id\}

-   参数说明

    <a name="table5162674110529"></a>
    <table><thead align="left"><tr id="row4741724810529"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p1559190910529"><a name="p1559190910529"></a><a name="p1559190910529"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p5498513910529"><a name="p5498513910529"></a><a name="p5498513910529"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p2461124910529"><a name="p2461124910529"></a><a name="p2461124910529"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4735411910529"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p1047843010529"><a name="p1047843010529"></a><a name="p1047843010529"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p4344649310529"><a name="p4344649310529"></a><a name="p4344649310529"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p2950506910529"><a name="p2950506910529"></a><a name="p2950506910529"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row22943135111210"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p53024664151925"><a name="p53024664151925"></a><a name="p53024664151925"></a>transfer_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p30503151925"><a name="p30503151925"></a><a name="p30503151925"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p2470771151925"><a name="p2470771151925"></a><a name="p2470771151925"></a>云硬盘过户记录ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0092902035_section3832507172056"></a>

-   请求样例：

    ```
    GET  https://{endpoint}/v3/{project_id}/os-volume-transfer/cac5c677-73a9-4288-bb9c-b2ebfb547377
    ```


## 响应消息<a name="section5804104214399"></a>

-   响应参数

    <a name="evs_04_2109_table6510124331610"></a>
    <table><thead align="left"><tr id="evs_04_2109_row1751054317165"><th class="cellrowborder" valign="top" width="26.32%" id="mcps1.1.4.1.1"><p id="evs_04_2109_p851014331611"><a name="evs_04_2109_p851014331611"></a><a name="evs_04_2109_p851014331611"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.05%" id="mcps1.1.4.1.2"><p id="evs_04_2109_p5510174319163"><a name="evs_04_2109_p5510174319163"></a><a name="evs_04_2109_p5510174319163"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.629999999999995%" id="mcps1.1.4.1.3"><p id="evs_04_2109_p45101438167"><a name="evs_04_2109_p45101438167"></a><a name="evs_04_2109_p45101438167"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2109_row175101243141616"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_p5510743171617"><a name="evs_04_2109_p5510743171617"></a><a name="evs_04_2109_p5510743171617"></a>transfer</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_p115101943131611"><a name="evs_04_2109_p115101943131611"></a><a name="evs_04_2109_p115101943131611"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_p14510134319169"><a name="evs_04_2109_p14510134319169"></a><a name="evs_04_2109_p14510134319169"></a>云硬盘过户记录详情，请参见<a href="#evs_04_2109_li61468331112723">•transfer参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2109_li61468331112723"></a>transfer参数说明

    <a name="evs_04_2109_zh-cn_topic_0092902035_table6685576181553"></a>
    <table><thead align="left"><tr id="evs_04_2109_zh-cn_topic_0092902035_row1296752181553"><th class="cellrowborder" valign="top" width="26.32%" id="mcps1.1.4.1.1"><p id="evs_04_2109_zh-cn_topic_0092902035_p37928058181553"><a name="evs_04_2109_zh-cn_topic_0092902035_p37928058181553"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p37928058181553"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.05%" id="mcps1.1.4.1.2"><p id="evs_04_2109_zh-cn_topic_0092902035_p52273840181553"><a name="evs_04_2109_zh-cn_topic_0092902035_p52273840181553"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p52273840181553"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="52.629999999999995%" id="mcps1.1.4.1.3"><p id="evs_04_2109_zh-cn_topic_0092902035_p42375363181553"><a name="evs_04_2109_zh-cn_topic_0092902035_p42375363181553"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p42375363181553"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2109_zh-cn_topic_0092902035_row12974480107"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_zh-cn_topic_0092902035_p1097410819109"><a name="evs_04_2109_zh-cn_topic_0092902035_p1097410819109"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p1097410819109"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_zh-cn_topic_0092902035_p797448121011"><a name="evs_04_2109_zh-cn_topic_0092902035_p797448121011"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p797448121011"></a>List&lt; Dict &gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_zh-cn_topic_0092902035_p17974484101"><a name="evs_04_2109_zh-cn_topic_0092902035_p17974484101"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p17974484101"></a>云硬盘过户记录的链接。</p>
    </td>
    </tr>
    <tr id="evs_04_2109_zh-cn_topic_0092902035_row862121220101"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_zh-cn_topic_0092902035_p1762112141010"><a name="evs_04_2109_zh-cn_topic_0092902035_p1762112141010"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p1762112141010"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_zh-cn_topic_0092902035_p4623123109"><a name="evs_04_2109_zh-cn_topic_0092902035_p4623123109"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p4623123109"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_zh-cn_topic_0092902035_p186221213104"><a name="evs_04_2109_zh-cn_topic_0092902035_p186221213104"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p186221213104"></a>云硬盘过户记录的创建时间。</p>
    <p id="evs_04_2109_p8210113613819"><a name="evs_04_2109_p8210113613819"></a><a name="evs_04_2109_p8210113613819"></a><span id="evs_04_2109_text164869573817"><a name="evs_04_2109_text164869573817"></a><a name="evs_04_2109_text164869573817"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2109_zh-cn_topic_0092902035_row569771417102"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_zh-cn_topic_0092902035_p369761461010"><a name="evs_04_2109_zh-cn_topic_0092902035_p369761461010"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p369761461010"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_zh-cn_topic_0092902035_p769712143104"><a name="evs_04_2109_zh-cn_topic_0092902035_p769712143104"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p769712143104"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_zh-cn_topic_0092902035_p56979145107"><a name="evs_04_2109_zh-cn_topic_0092902035_p56979145107"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p56979145107"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2109_zh-cn_topic_0092902035_row2457217151019"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_zh-cn_topic_0092902035_p94571174106"><a name="evs_04_2109_zh-cn_topic_0092902035_p94571174106"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p94571174106"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_zh-cn_topic_0092902035_p174577172105"><a name="evs_04_2109_zh-cn_topic_0092902035_p174577172105"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p174577172105"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_zh-cn_topic_0092902035_p18457171718107"><a name="evs_04_2109_zh-cn_topic_0092902035_p18457171718107"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p18457171718107"></a>云硬盘过户记录的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2109_zh-cn_topic_0092902035_row527752431012"><td class="cellrowborder" valign="top" width="26.32%" headers="mcps1.1.4.1.1 "><p id="evs_04_2109_zh-cn_topic_0092902035_p10277112415105"><a name="evs_04_2109_zh-cn_topic_0092902035_p10277112415105"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p10277112415105"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.05%" headers="mcps1.1.4.1.2 "><p id="evs_04_2109_zh-cn_topic_0092902035_p4277132441017"><a name="evs_04_2109_zh-cn_topic_0092902035_p4277132441017"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p4277132441017"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="52.629999999999995%" headers="mcps1.1.4.1.3 "><p id="evs_04_2109_zh-cn_topic_0092902035_p827720241108"><a name="evs_04_2109_zh-cn_topic_0092902035_p827720241108"></a><a name="evs_04_2109_zh-cn_topic_0092902035_p827720241108"></a>云硬盘过户记录的名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "transfer": {
            "id": "cac5c677-73a9-4288-bb9c-b2ebfb547377", 
            "created_at": "2015-02-25T03:56:53.081642", 
            "name": "first volume transfer", 
            "volume_id": "894623a6-e901-4312-aa06-4275e6321cce", 
            "links": [
                {
                    "href": "https://localhost/v2/firstproject/os-volume-transfer/1", 
                    "rel": "self"
                }, 
                {
                    "href": "https://localhost/firstproject/os-volume-transfer/1", 
                    "rel": "bookmark"
                }
            ]
        }
    }
    ```


## 状态码<a name="zh-cn_topic_0092887872_section10353980172239"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

