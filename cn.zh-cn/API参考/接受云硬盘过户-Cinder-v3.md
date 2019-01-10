# 接受云硬盘过户<a name="ZH-CN_TOPIC_0102728949"></a>

## 功能介绍<a name="zh-cn_topic_0092901819_section44805042171914"></a>

通过云硬盘过户记录ID以及身份认证密钥来接受云硬盘过户。

## URI<a name="zh-cn_topic_0092887872_section21748494171940"></a>

-   URI格式

    POST /v3/\{project\_id\}/os-volume-transfer/\{transfer\_id\}/accept

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
    </td>
    </tr>
    <tr id="row22943135111210"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p46454683111210"><a name="p46454683111210"></a><a name="p46454683111210"></a>transfer_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p4732946111210"><a name="p4732946111210"></a><a name="p4732946111210"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p47824366111210"><a name="p47824366111210"></a><a name="p47824366111210"></a>云硬盘过户记录ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 约束<a name="zh-cn_topic_0092901819_section47607821172029"></a>

-   包周期的云硬盘不支持过户。
-   冻结的云硬盘不支持过户。
-   加密的云硬盘不支持过户。
-   云硬盘有对应的备份和快照时不支持过户。
-   云硬盘有备份策略时不支持过户。
-   DSS专属存储的云硬盘不支持过户。
-   DESS专属存储的云硬盘不支持过户。
-   EVS系统盘不支持过户。

>![](public_sys-resources/icon-note.gif) **说明：**   
>若使用以上不支持过户的云硬盘，则返回的错误码为400。  

## 请求<a name="zh-cn_topic_0092901819_section3832507172056"></a>

-   请求参数

    <a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_table42671863"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_row12592542"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p13362997"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p13362997"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p8661001"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p8661001"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p30452481"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p30452481"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p50731910"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p50731910"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_row5187493615377"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4112025815377"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4112025815377"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4112025815377"></a>accept</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4240658415377"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4240658415377"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p4240658415377"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p1238131615377"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p1238131615377"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p6336250715377"><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p6336250715377"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0093348348_p6336250715377"></a>标记接受云硬盘过户操作。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   accept参数说明

    <a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_table881415614117"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_row168152061012"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p17815961816"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p17815961816"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p17815961816"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p9815116514"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p9815116514"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p9815116514"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="23%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p11815176017"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p11815176017"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p11815176017"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="41%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p881596417"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p881596417"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092887872_p881596417"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0093348349_zh-cn_topic_0092887872_row6815269119"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0093348349_p64366674111553"><a name="zh-cn_topic_0093348349_p64366674111553"></a><a name="zh-cn_topic_0093348349_p64366674111553"></a>auth_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0093348349_p46318102111553"><a name="zh-cn_topic_0093348349_p46318102111553"></a><a name="zh-cn_topic_0093348349_p46318102111553"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0093348349_p60778811111553"><a name="zh-cn_topic_0093348349_p60778811111553"></a><a name="zh-cn_topic_0093348349_p60778811111553"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="41%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0093348349_p24136681111553"><a name="zh-cn_topic_0093348349_p24136681111553"></a><a name="zh-cn_topic_0093348349_p24136681111553"></a>云硬盘过户的身份认证密钥。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "accept": {
            "auth_key": "9266c59563c84664"
        }
    }
    ```


## 响应<a name="section10834135717381"></a>

-   响应参数

    <a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_table6685576181553"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_row1296752181553"><th class="cellrowborder" valign="top" width="24.67753224677532%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p37928058181553"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p37928058181553"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p37928058181553"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.67753224677532%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p52273840181553"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p52273840181553"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p52273840181553"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="50.64493550644935%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p42375363181553"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p42375363181553"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p42375363181553"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0093348349_row13910103243912"><td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0093348349_p12910123263919"><a name="zh-cn_topic_0093348349_p12910123263919"></a><a name="zh-cn_topic_0093348349_p12910123263919"></a>transfer</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0093348349_p291020325394"><a name="zh-cn_topic_0093348349_p291020325394"></a><a name="zh-cn_topic_0093348349_p291020325394"></a>map&lt;string, object&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.64493550644935%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0093348349_p2910143215398"><a name="zh-cn_topic_0093348349_p2910143215398"></a><a name="zh-cn_topic_0093348349_p2910143215398"></a>云硬盘过户信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_row569771417102"><td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p369761461010"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p369761461010"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p369761461010"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p769712143104"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p769712143104"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p769712143104"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.64493550644935%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p56979145107"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p56979145107"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p56979145107"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_row2457217151019"><td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p94571174106"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p94571174106"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p94571174106"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p174577172105"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p174577172105"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p174577172105"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.64493550644935%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p18457171718107"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p18457171718107"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p18457171718107"></a>云硬盘过户记录的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_row527752431012"><td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p10277112415105"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p10277112415105"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p10277112415105"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p4277132441017"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p4277132441017"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p4277132441017"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.64493550644935%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p827720241108"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p827720241108"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p827720241108"></a>云硬盘过户记录的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_row10511614102910"><td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p19144131917296"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p19144131917296"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p19144131917296"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.67753224677532%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p950720235293"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p950720235293"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p950720235293"></a>List&lt; Dict &gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="50.64493550644935%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p184902291294"><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p184902291294"></a><a name="zh-cn_topic_0093348349_zh-cn_topic_0092901819_p184902291294"></a>云硬盘过户记录的链接。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "transfer": {
            "id": "cac5c677-73a9-4288-bb9c-b2ebfb547377", 
            "name": "first volume transfer", 
            "volume_id": "894623a6-e901-4312-aa06-4275e6321cce", 
            "links": [
                {
                    "href": "https://localhost/v3/firstproject/os-volume-transfer/1", 
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


## 返回值<a name="zh-cn_topic_0092901819_section10353980172239"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

