# 创建云硬盘过户<a name="evs_04_2106"></a>

## 功能介绍<a name="zh-cn_topic_0092887872_section44805042171914"></a>

指定云硬盘来创建云硬盘过户记录，创建成功后，会返回过户记录ID以及身份认证密钥。

云硬盘在过户过程中的状态变化如下：创建云硬盘过户后，云硬盘状态由“available”变为“awaiting-transfer”。当云硬盘过户被接收后，云硬盘状态变为“available”。

## 接口约束<a name="zh-cn_topic_0092887872_section47607821172029"></a>

只有当云硬盘状态为available时，支持创建过户，其他不支持过户的约束如下：

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

## URI<a name="section1351917332235"></a>

-   URI格式

    POST /v2/\{project\_id\}/os-volume-transfer

-   参数说明

    <a name="table12146232414"></a>
    <table><thead align="left"><tr id="row1221412122414"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p17214424242"><a name="p17214424242"></a><a name="p17214424242"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p7214122102419"><a name="p7214122102419"></a><a name="p7214122102419"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1021542202417"><a name="p1021542202417"></a><a name="p1021542202417"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row202151428245"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p32155212418"><a name="p32155212418"></a><a name="p32155212418"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p721519211241"><a name="p721519211241"></a><a name="p721519211241"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p6215122152416"><a name="p6215122152416"></a><a name="p6215122152416"></a>项目ID。</p>
    <p id="p721518282414"><a name="p721518282414"></a><a name="p721518282414"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="zh-cn_topic_0092887872_section3832507172056"></a>

-   请求参数

    <a name="table42671863"></a>
    <table><thead align="left"><tr id="row12592542"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p13362997"><a name="p13362997"></a><a name="p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p8661001"><a name="p8661001"></a><a name="p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p30452481"><a name="p30452481"></a><a name="p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44%" id="mcps1.1.5.1.4"><p id="p50731910"><a name="p50731910"></a><a name="p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5187493615377"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p4112025815377"><a name="p4112025815377"></a><a name="p4112025815377"></a>transfer</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p4240658415377"><a name="p4240658415377"></a><a name="p4240658415377"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1238131615377"><a name="p1238131615377"></a><a name="p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.1.5.1.4 "><p id="p6336250715377"><a name="p6336250715377"></a><a name="p6336250715377"></a>标记创建云硬盘过户操作，请参见<a href="#li55316081111336">•transfer参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li55316081111336"></a>transfer参数说明

    <a name="zh-cn_topic_0092887872_table881415614117"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0092887872_row168152061012"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0092887872_p17815961816"><a name="zh-cn_topic_0092887872_p17815961816"></a><a name="zh-cn_topic_0092887872_p17815961816"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0092887872_p9815116514"><a name="zh-cn_topic_0092887872_p9815116514"></a><a name="zh-cn_topic_0092887872_p9815116514"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0092887872_p11815176017"><a name="zh-cn_topic_0092887872_p11815176017"></a><a name="zh-cn_topic_0092887872_p11815176017"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="43.43434343434344%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0092887872_p881596417"><a name="zh-cn_topic_0092887872_p881596417"></a><a name="zh-cn_topic_0092887872_p881596417"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0092887872_row6815269119"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0092887872_p15774191420418"><a name="zh-cn_topic_0092887872_p15774191420418"></a><a name="zh-cn_topic_0092887872_p15774191420418"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0092887872_p11815126917"><a name="zh-cn_topic_0092887872_p11815126917"></a><a name="zh-cn_topic_0092887872_p11815126917"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0092887872_p178154611118"><a name="zh-cn_topic_0092887872_p178154611118"></a><a name="zh-cn_topic_0092887872_p178154611118"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0092887872_p88151664117"><a name="zh-cn_topic_0092887872_p88151664117"></a><a name="zh-cn_topic_0092887872_p88151664117"></a>云硬盘ID。</p>
    <p id="p0664195210426"><a name="p0664195210426"></a><a name="p0664195210426"></a>通过<a href="查询所有云硬盘详情-Cinder-v3.md">查询所有云硬盘详情</a>获取。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row48151561014"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0092887872_p1781517616118"><a name="zh-cn_topic_0092887872_p1781517616118"></a><a name="zh-cn_topic_0092887872_p1781517616118"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0092887872_p10815136119"><a name="zh-cn_topic_0092887872_p10815136119"></a><a name="zh-cn_topic_0092887872_p10815136119"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0092887872_p98151467115"><a name="zh-cn_topic_0092887872_p98151467115"></a><a name="zh-cn_topic_0092887872_p98151467115"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0092887872_p17815196917"><a name="zh-cn_topic_0092887872_p17815196917"></a><a name="zh-cn_topic_0092887872_p17815196917"></a>云硬盘过户记录的名称。<span id="text726643673017"><a name="text726643673017"></a><a name="text726643673017"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "transfer": {
            "volume_id": "c86b9af4-151d-4ead-b62c-5fb967af0e37", 
            "name": "first volume"
        }
    }
    ```


## 响应消息<a name="zh-cn_topic_0092887872_section23586530172122"></a>

-   响应参数

    <a name="table367317440212"></a>
    <table><thead align="left"><tr id="row167314412210"><th class="cellrowborder" valign="top" width="24.05%" id="mcps1.1.4.1.1"><p id="p467324415210"><a name="p467324415210"></a><a name="p467324415210"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.05%" id="mcps1.1.4.1.2"><p id="p156746441427"><a name="p156746441427"></a><a name="p156746441427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.9%" id="mcps1.1.4.1.3"><p id="p8674134413213"><a name="p8674134413213"></a><a name="p8674134413213"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row196747441326"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="p967411441324"><a name="p967411441324"></a><a name="p967411441324"></a>transfer</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="p106741844324"><a name="p106741844324"></a><a name="p106741844324"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="p1067484418216"><a name="p1067484418216"></a><a name="p1067484418216"></a>云硬盘过户信息，请参见<a href="#li32419762111447">•transfer参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li32419762111447"></a>transfer参数说明

    <a name="zh-cn_topic_0092887872_table6685576181553"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0092887872_row1296752181553"><th class="cellrowborder" valign="top" width="24.05%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0092887872_p37928058181553"><a name="zh-cn_topic_0092887872_p37928058181553"></a><a name="zh-cn_topic_0092887872_p37928058181553"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.05%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0092887872_p52273840181553"><a name="zh-cn_topic_0092887872_p52273840181553"></a><a name="zh-cn_topic_0092887872_p52273840181553"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.9%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0092887872_p42375363181553"><a name="zh-cn_topic_0092887872_p42375363181553"></a><a name="zh-cn_topic_0092887872_p42375363181553"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0092887872_row45833953181553"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p21562735181553"><a name="zh-cn_topic_0092887872_p21562735181553"></a><a name="zh-cn_topic_0092887872_p21562735181553"></a>auth_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p1751085181553"><a name="zh-cn_topic_0092887872_p1751085181553"></a><a name="zh-cn_topic_0092887872_p1751085181553"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p13253466181553"><a name="zh-cn_topic_0092887872_p13253466181553"></a><a name="zh-cn_topic_0092887872_p13253466181553"></a>云硬盘过户的身份认证密钥。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row12974480107"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p1097410819109"><a name="zh-cn_topic_0092887872_p1097410819109"></a><a name="zh-cn_topic_0092887872_p1097410819109"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p797448121011"><a name="zh-cn_topic_0092887872_p797448121011"></a><a name="zh-cn_topic_0092887872_p797448121011"></a>List&lt; Dict &gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p17974484101"><a name="zh-cn_topic_0092887872_p17974484101"></a><a name="zh-cn_topic_0092887872_p17974484101"></a>云硬盘过户记录的链接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row862121220101"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p1762112141010"><a name="zh-cn_topic_0092887872_p1762112141010"></a><a name="zh-cn_topic_0092887872_p1762112141010"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p4623123109"><a name="zh-cn_topic_0092887872_p4623123109"></a><a name="zh-cn_topic_0092887872_p4623123109"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p186221213104"><a name="zh-cn_topic_0092887872_p186221213104"></a><a name="zh-cn_topic_0092887872_p186221213104"></a>云硬盘过户记录的创建时间。</p>
    <p id="p189414591376"><a name="p189414591376"></a><a name="p189414591376"></a><span id="text164869573817"><a name="text164869573817"></a><a name="text164869573817"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row569771417102"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p369761461010"><a name="zh-cn_topic_0092887872_p369761461010"></a><a name="zh-cn_topic_0092887872_p369761461010"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p769712143104"><a name="zh-cn_topic_0092887872_p769712143104"></a><a name="zh-cn_topic_0092887872_p769712143104"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p56979145107"><a name="zh-cn_topic_0092887872_p56979145107"></a><a name="zh-cn_topic_0092887872_p56979145107"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row2457217151019"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p94571174106"><a name="zh-cn_topic_0092887872_p94571174106"></a><a name="zh-cn_topic_0092887872_p94571174106"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p174577172105"><a name="zh-cn_topic_0092887872_p174577172105"></a><a name="zh-cn_topic_0092887872_p174577172105"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p18457171718107"><a name="zh-cn_topic_0092887872_p18457171718107"></a><a name="zh-cn_topic_0092887872_p18457171718107"></a>云硬盘过户记录的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0092887872_row527752431012"><td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0092887872_p10277112415105"><a name="zh-cn_topic_0092887872_p10277112415105"></a><a name="zh-cn_topic_0092887872_p10277112415105"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.05%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0092887872_p4277132441017"><a name="zh-cn_topic_0092887872_p4277132441017"></a><a name="zh-cn_topic_0092887872_p4277132441017"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0092887872_p827720241108"><a name="zh-cn_topic_0092887872_p827720241108"></a><a name="zh-cn_topic_0092887872_p827720241108"></a>云硬盘过户记录的名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "transfer": {
            "id": "1a7059f5-8ed7-45b7-8d05-2811e5d09f24", 
            "created_at": "2015-02-25T03:56:53.081642", 
            "name": "first volume", 
            "volume_id": "c86b9af4-151d-4ead-b62c-5fb967af0e37", 
            "auth_key": "9266c59563c84664", 
            "links": [
                {
                    "href": "https://localhost/v2/firstproject/os-volume-transfer/3", 
                    "rel": "self"
                }, 
                {
                    "href": "https://localhost/firstproject/os-volume-transfer/3", 
                    "rel": "bookmark"
                }
            ]
        }
    }
    ```


## 状态码<a name="zh-cn_topic_0092887872_section10353980172239"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

