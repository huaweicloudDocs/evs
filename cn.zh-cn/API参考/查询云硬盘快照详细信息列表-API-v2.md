# 查询云硬盘快照详细信息列表<a name="evs_04_2021"></a>

## 功能介绍<a name="section29798282112049"></a>

查询云硬盘快照详细列表信息。支持企业项目授权功能。

## URI<a name="section56404342112049"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudsnapshots/detail


-   参数说明

    <a name="evs_04_2023_table37114383112049"></a>
    <table><thead align="left"><tr id="evs_04_2023_row4845983112049"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="evs_04_2023_p56980371112049"><a name="evs_04_2023_p56980371112049"></a><a name="evs_04_2023_p56980371112049"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="evs_04_2023_p52007339112049"><a name="evs_04_2023_p52007339112049"></a><a name="evs_04_2023_p52007339112049"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="evs_04_2023_p51844944112049"><a name="evs_04_2023_p51844944112049"></a><a name="evs_04_2023_p51844944112049"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2023_row38690921112049"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="evs_04_2023_p46956895112049"><a name="evs_04_2023_p46956895112049"></a><a name="evs_04_2023_p46956895112049"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="evs_04_2023_p45412121112049"><a name="evs_04_2023_p45412121112049"></a><a name="evs_04_2023_p45412121112049"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="evs_04_2023_p54503167112049"><a name="evs_04_2023_p54503167112049"></a><a name="evs_04_2023_p54503167112049"></a>项目ID。</p>
    <p id="evs_04_2023_p55811451337"><a name="evs_04_2023_p55811451337"></a><a name="evs_04_2023_p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Request filter参数说明

    <a name="evs_04_2023_table262294112126"></a>
    <table><thead align="left"><tr id="evs_04_2023_row15086975112126"><th class="cellrowborder" valign="top" width="15.752475247524753%" id="mcps1.1.5.1.1"><p id="evs_04_2023_p14085481112126"><a name="evs_04_2023_p14085481112126"></a><a name="evs_04_2023_p14085481112126"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.89108910891089%" id="mcps1.1.5.1.2"><p id="evs_04_2023_p73303112126"><a name="evs_04_2023_p73303112126"></a><a name="evs_04_2023_p73303112126"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="evs_04_2023_p5937586112126"><a name="evs_04_2023_p5937586112126"></a><a name="evs_04_2023_p5937586112126"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="evs_04_2023_p11182433112126"><a name="evs_04_2023_p11182433112126"></a><a name="evs_04_2023_p11182433112126"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2023_row33533036112126"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p373114017611"><a name="evs_04_2023_p373114017611"></a><a name="evs_04_2023_p373114017611"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p9733405620"><a name="evs_04_2023_p9733405620"></a><a name="evs_04_2023_p9733405620"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p167311401064"><a name="evs_04_2023_p167311401064"></a><a name="evs_04_2023_p167311401064"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p18735401366"><a name="evs_04_2023_p18735401366"></a><a name="evs_04_2023_p18735401366"></a>偏移量。</p>
    <div class="note" id="evs_04_2023_note158681239962"><a name="evs_04_2023_note158681239962"></a><a name="evs_04_2023_note158681239962"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2023_p18766406612"><a name="evs_04_2023_p18766406612"></a><a name="evs_04_2023_p18766406612"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2023_row47675000112126"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p137684010618"><a name="evs_04_2023_p137684010618"></a><a name="evs_04_2023_p137684010618"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p3769401863"><a name="evs_04_2023_p3769401863"></a><a name="evs_04_2023_p3769401863"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p1476124010618"><a name="evs_04_2023_p1476124010618"></a><a name="evs_04_2023_p1476124010618"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p19769400614"><a name="evs_04_2023_p19769400614"></a><a name="evs_04_2023_p19769400614"></a>返回结果个数限制。</p>
    <p id="evs_04_2023_p169978140101"><a name="evs_04_2023_p169978140101"></a><a name="evs_04_2023_p169978140101"></a><span id="evs_04_2023_text138349551887"><a name="evs_04_2023_text138349551887"></a><a name="evs_04_2023_text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2023_row13436622112126"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p1676144017613"><a name="evs_04_2023_p1676144017613"></a><a name="evs_04_2023_p1676144017613"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p87614408618"><a name="evs_04_2023_p87614408618"></a><a name="evs_04_2023_p87614408618"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p167617402061"><a name="evs_04_2023_p167617402061"></a><a name="evs_04_2023_p167617402061"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p97618401260"><a name="evs_04_2023_p97618401260"></a><a name="evs_04_2023_p97618401260"></a>云硬盘快照名称。最大支持255个字节。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row1141410332065"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p5761401568"><a name="evs_04_2023_p5761401568"></a><a name="evs_04_2023_p5761401568"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p77654015617"><a name="evs_04_2023_p77654015617"></a><a name="evs_04_2023_p77654015617"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p157694017617"><a name="evs_04_2023_p157694017617"></a><a name="evs_04_2023_p157694017617"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p7762404620"><a name="evs_04_2023_p7762404620"></a><a name="evs_04_2023_p7762404620"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row44141633861"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p576204015617"><a name="evs_04_2023_p576204015617"></a><a name="evs_04_2023_p576204015617"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p10761840364"><a name="evs_04_2023_p10761840364"></a><a name="evs_04_2023_p10761840364"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p97619401468"><a name="evs_04_2023_p97619401468"></a><a name="evs_04_2023_p97619401468"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p16761740967"><a name="evs_04_2023_p16761740967"></a><a name="evs_04_2023_p16761740967"></a>云硬盘快照对应的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row04149331262"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p076204017617"><a name="evs_04_2023_p076204017617"></a><a name="evs_04_2023_p076204017617"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p17761140469"><a name="evs_04_2023_p17761140469"></a><a name="evs_04_2023_p17761140469"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p1476174016620"><a name="evs_04_2023_p1476174016620"></a><a name="evs_04_2023_p1476174016620"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p1476134011615"><a name="evs_04_2023_p1476134011615"></a><a name="evs_04_2023_p1476134011615"></a>云硬盘快照对应的云硬盘所在的可用区。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row193286371269"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p576184013611"><a name="evs_04_2023_p576184013611"></a><a name="evs_04_2023_p576184013611"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p7765401560"><a name="evs_04_2023_p7765401560"></a><a name="evs_04_2023_p7765401560"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p0762409612"><a name="evs_04_2023_p0762409612"></a><a name="evs_04_2023_p0762409612"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p487845411817"><a name="evs_04_2023_p487845411817"></a><a name="evs_04_2023_p487845411817"></a>指定快照id进行过滤。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row1132919377615"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p10768401367"><a name="evs_04_2023_p10768401367"></a><a name="evs_04_2023_p10768401367"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p1476140761"><a name="evs_04_2023_p1476140761"></a><a name="evs_04_2023_p1476140761"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p4765401464"><a name="evs_04_2023_p4765401464"></a><a name="evs_04_2023_p4765401464"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p476040768"><a name="evs_04_2023_p476040768"></a><a name="evs_04_2023_p476040768"></a>专属存储的名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row632920371464"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p1768406611"><a name="evs_04_2023_p1768406611"></a><a name="evs_04_2023_p1768406611"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p176114016618"><a name="evs_04_2023_p176114016618"></a><a name="evs_04_2023_p176114016618"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p14761940262"><a name="evs_04_2023_p14761940262"></a><a name="evs_04_2023_p14761940262"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p12763408618"><a name="evs_04_2023_p12763408618"></a><a name="evs_04_2023_p12763408618"></a>专属存储ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row932973714613"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p976174012616"><a name="evs_04_2023_p976174012616"></a><a name="evs_04_2023_p976174012616"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p1076440762"><a name="evs_04_2023_p1076440762"></a><a name="evs_04_2023_p1076440762"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p776204016615"><a name="evs_04_2023_p776204016615"></a><a name="evs_04_2023_p776204016615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p87615401565"><a name="evs_04_2023_p87615401565"></a><a name="evs_04_2023_p87615401565"></a>服务类型。</p>
    <p id="evs_04_2023_p1079317498816"><a name="evs_04_2023_p1079317498816"></a><a name="evs_04_2023_p1079317498816"></a>仅支持EVS、DSS、DESS</p>
    <p id="evs_04_2023_p1497011418920"><a name="evs_04_2023_p1497011418920"></a><a name="evs_04_2023_p1497011418920"></a>service_type为EVS时，dedicated_storage_name和dedicated_storage_id必须都为空。</p>
    </td>
    </tr>
    <tr id="evs_04_2023_row9529426343"><td class="cellrowborder" valign="top" width="15.752475247524753%" headers="mcps1.1.5.1.1 "><p id="evs_04_2023_p17746165016465"><a name="evs_04_2023_p17746165016465"></a><a name="evs_04_2023_p17746165016465"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.89108910891089%" headers="mcps1.1.5.1.2 "><p id="evs_04_2023_p1474605013468"><a name="evs_04_2023_p1474605013468"></a><a name="evs_04_2023_p1474605013468"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2023_p117461050114615"><a name="evs_04_2023_p117461050114615"></a><a name="evs_04_2023_p117461050114615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2023_p2746950164617"><a name="evs_04_2023_p2746950164617"></a><a name="evs_04_2023_p2746950164617"></a>指定企业项目id进行过滤。</p>
    <p id="evs_04_2023_p4746185064614"><a name="evs_04_2023_p4746185064614"></a><a name="evs_04_2023_p4746185064614"></a>传入“all_granted_eps”，代表查询权限范围内的所有企业项目下的云硬盘。</p>
    <div class="note" id="evs_04_2023_note1664605004618"><a name="evs_04_2023_note1664605004618"></a><a name="evs_04_2023_note1664605004618"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2023_evs_04_2013_p18336524404"><a name="evs_04_2023_evs_04_2013_p18336524404"></a><a name="evs_04_2023_evs_04_2013_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section416875095210"></a>

以查询状态为available的云硬盘快照为例。

-   请求样例：

    ```
    GET https://{endpoint}/v2/{project_id}/cloudsnapshots/detail?status=available
    ```


## 响应消息<a name="section50618846112239"></a>

-   响应参数

    <a name="zh-cn_topic_0123550104_table55593749112239"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0123550104_row12503066112239"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0123550104_p6115391112239"><a name="zh-cn_topic_0123550104_p6115391112239"></a><a name="zh-cn_topic_0123550104_p6115391112239"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0123550104_p25584640112239"><a name="zh-cn_topic_0123550104_p25584640112239"></a><a name="zh-cn_topic_0123550104_p25584640112239"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0123550104_p21559929112239"><a name="zh-cn_topic_0123550104_p21559929112239"></a><a name="zh-cn_topic_0123550104_p21559929112239"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0123550104_row59821639112239"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1254928141117"><a name="zh-cn_topic_0123550104_p1254928141117"></a><a name="zh-cn_topic_0123550104_p1254928141117"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p32542028171112"><a name="zh-cn_topic_0123550104_p32542028171112"></a><a name="zh-cn_topic_0123550104_p32542028171112"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1325417283117"><a name="zh-cn_topic_0123550104_p1325417283117"></a><a name="zh-cn_topic_0123550104_p1325417283117"></a>快照的总数量，不受limit、offset参数的影响。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row60405564112239"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p16254228181117"><a name="zh-cn_topic_0123550104_p16254228181117"></a><a name="zh-cn_topic_0123550104_p16254228181117"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p52546289117"><a name="zh-cn_topic_0123550104_p52546289117"></a><a name="zh-cn_topic_0123550104_p52546289117"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1825462821113"><a name="zh-cn_topic_0123550104_p1825462821113"></a><a name="zh-cn_topic_0123550104_p1825462821113"></a>快照信息，请参见<a href="#zh-cn_topic_0123550104_li444161713165">•snapshots参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row1081819219117"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1025582813117"><a name="zh-cn_topic_0123550104_p1025582813117"></a><a name="zh-cn_topic_0123550104_p1025582813117"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p1025513281119"><a name="zh-cn_topic_0123550104_p1025513281119"></a><a name="zh-cn_topic_0123550104_p1025513281119"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1255112811117"><a name="zh-cn_topic_0123550104_p1255112811117"></a><a name="zh-cn_topic_0123550104_p1255112811117"></a>云硬盘快照列表查询位置标记，当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="row151261146152816"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0123550104_li444161713165"></a>snapshots参数说明

    <a name="zh-cn_topic_0123550104_table43291794165"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0123550104_row669989131614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0123550104_p1369912961618"><a name="zh-cn_topic_0123550104_p1369912961618"></a><a name="zh-cn_topic_0123550104_p1369912961618"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.53%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0123550104_p1069917913161"><a name="zh-cn_topic_0123550104_p1069917913161"></a><a name="zh-cn_topic_0123550104_p1069917913161"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0123550104_p196991790169"><a name="zh-cn_topic_0123550104_p196991790169"></a><a name="zh-cn_topic_0123550104_p196991790169"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0123550104_row769918919163"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p7699149141616"><a name="zh-cn_topic_0123550104_p7699149141616"></a><a name="zh-cn_topic_0123550104_p7699149141616"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p970179141613"><a name="zh-cn_topic_0123550104_p970179141613"></a><a name="zh-cn_topic_0123550104_p970179141613"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1370119131610"><a name="zh-cn_topic_0123550104_p1370119131610"></a><a name="zh-cn_topic_0123550104_p1370119131610"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row470139171619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p87011094167"><a name="zh-cn_topic_0123550104_p87011094167"></a><a name="zh-cn_topic_0123550104_p87011094167"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p11701119111617"><a name="zh-cn_topic_0123550104_p11701119111617"></a><a name="zh-cn_topic_0123550104_p11701119111617"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p14701129151612"><a name="zh-cn_topic_0123550104_p14701129151612"></a><a name="zh-cn_topic_0123550104_p14701129151612"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row1970113916161"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p127019912167"><a name="zh-cn_topic_0123550104_p127019912167"></a><a name="zh-cn_topic_0123550104_p127019912167"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p13701691161"><a name="zh-cn_topic_0123550104_p13701691161"></a><a name="zh-cn_topic_0123550104_p13701691161"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1470118917161"><a name="zh-cn_topic_0123550104_p1470118917161"></a><a name="zh-cn_topic_0123550104_p1470118917161"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row127011894169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p570114991613"><a name="zh-cn_topic_0123550104_p570114991613"></a><a name="zh-cn_topic_0123550104_p570114991613"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p197013921610"><a name="zh-cn_topic_0123550104_p197013921610"></a><a name="zh-cn_topic_0123550104_p197013921610"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p127014921612"><a name="zh-cn_topic_0123550104_p127014921612"></a><a name="zh-cn_topic_0123550104_p127014921612"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row0701796168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p970115917165"><a name="zh-cn_topic_0123550104_p970115917165"></a><a name="zh-cn_topic_0123550104_p970115917165"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p370109111619"><a name="zh-cn_topic_0123550104_p370109111619"></a><a name="zh-cn_topic_0123550104_p370109111619"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1370113921616"><a name="zh-cn_topic_0123550104_p1370113921616"></a><a name="zh-cn_topic_0123550104_p1370113921616"></a>云硬盘快照创建时间。</p>
    <p id="p361892920377"><a name="p361892920377"></a><a name="p361892920377"></a><span id="text2094118359374"><a name="text2094118359374"></a><a name="text2094118359374"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row14701193168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p11701398164"><a name="zh-cn_topic_0123550104_p11701398164"></a><a name="zh-cn_topic_0123550104_p11701398164"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p870120981616"><a name="zh-cn_topic_0123550104_p870120981616"></a><a name="zh-cn_topic_0123550104_p870120981616"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p470117911615"><a name="zh-cn_topic_0123550104_p470117911615"></a><a name="zh-cn_topic_0123550104_p470117911615"></a>云硬盘快照更新时间。</p>
    <p id="p4345174117374"><a name="p4345174117374"></a><a name="p4345174117374"></a><span id="text146161141113716"><a name="text146161141113716"></a><a name="text146161141113716"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row1670169151619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p470112913161"><a name="zh-cn_topic_0123550104_p470112913161"></a><a name="zh-cn_topic_0123550104_p470112913161"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p187013901618"><a name="zh-cn_topic_0123550104_p187013901618"></a><a name="zh-cn_topic_0123550104_p187013901618"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p1470112981613"><a name="zh-cn_topic_0123550104_p1470112981613"></a><a name="zh-cn_topic_0123550104_p1470112981613"></a>云硬盘快照的元数据信息。</p>
    <p id="zh-cn_topic_0123550104_p1567410577152"><a name="zh-cn_topic_0123550104_p1567410577152"></a><a name="zh-cn_topic_0123550104_p1567410577152"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row2701209191619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1170120991610"><a name="zh-cn_topic_0123550104_p1170120991610"></a><a name="zh-cn_topic_0123550104_p1170120991610"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p470220919169"><a name="zh-cn_topic_0123550104_p470220919169"></a><a name="zh-cn_topic_0123550104_p470220919169"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p117021914162"><a name="zh-cn_topic_0123550104_p117021914162"></a><a name="zh-cn_topic_0123550104_p117021914162"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row7702129121618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1570215918168"><a name="zh-cn_topic_0123550104_p1570215918168"></a><a name="zh-cn_topic_0123550104_p1570215918168"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p470213913168"><a name="zh-cn_topic_0123550104_p470213913168"></a><a name="zh-cn_topic_0123550104_p470213913168"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p19702179121617"><a name="zh-cn_topic_0123550104_p19702179121617"></a><a name="zh-cn_topic_0123550104_p19702179121617"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row570214931611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1870220916166"><a name="zh-cn_topic_0123550104_p1870220916166"></a><a name="zh-cn_topic_0123550104_p1870220916166"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p16702096169"><a name="zh-cn_topic_0123550104_p16702096169"></a><a name="zh-cn_topic_0123550104_p16702096169"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p3702199191611"><a name="zh-cn_topic_0123550104_p3702199191611"></a><a name="zh-cn_topic_0123550104_p3702199191611"></a>租户ID。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row470219961618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1770210915169"><a name="zh-cn_topic_0123550104_p1770210915169"></a><a name="zh-cn_topic_0123550104_p1770210915169"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p1070212915167"><a name="zh-cn_topic_0123550104_p1070212915167"></a><a name="zh-cn_topic_0123550104_p1070212915167"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p170219911618"><a name="zh-cn_topic_0123550104_p170219911618"></a><a name="zh-cn_topic_0123550104_p170219911618"></a><span id="text4730642777"><a name="text4730642777"></a><a name="text4730642777"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row13702159201614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p47025941614"><a name="zh-cn_topic_0123550104_p47025941614"></a><a name="zh-cn_topic_0123550104_p47025941614"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p147021695165"><a name="zh-cn_topic_0123550104_p147021695165"></a><a name="zh-cn_topic_0123550104_p147021695165"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p670212941619"><a name="zh-cn_topic_0123550104_p670212941619"></a><a name="zh-cn_topic_0123550104_p670212941619"></a>专属存储的名称。</p>
    <p id="p345061161019"><a name="p345061161019"></a><a name="p345061161019"></a><span id="text1133045881216"><a name="text1133045881216"></a><a name="text1133045881216"></a>当使用了专属存储，才会有该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row970217913169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p1470214910165"><a name="zh-cn_topic_0123550104_p1470214910165"></a><a name="zh-cn_topic_0123550104_p1470214910165"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p137021597169"><a name="zh-cn_topic_0123550104_p137021597169"></a><a name="zh-cn_topic_0123550104_p137021597169"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p117024915160"><a name="zh-cn_topic_0123550104_p117024915160"></a><a name="zh-cn_topic_0123550104_p117024915160"></a>专属存储ID。</p>
    <p id="p103841424137"><a name="p103841424137"></a><a name="p103841424137"></a><span id="text1467622131318"><a name="text1467622131318"></a><a name="text1467622131318"></a>当使用了专属存储，才会有该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0123550104_row1070209171613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0123550104_p177022914166"><a name="zh-cn_topic_0123550104_p177022914166"></a><a name="zh-cn_topic_0123550104_p177022914166"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0123550104_p4702495168"><a name="zh-cn_topic_0123550104_p4702495168"></a><a name="zh-cn_topic_0123550104_p4702495168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0123550104_p2702199161612"><a name="zh-cn_topic_0123550104_p2702199161612"></a><a name="zh-cn_topic_0123550104_p2702199161612"></a>服务类型。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li0419202382514"></a>error参数说明

    <a name="evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2013_p19541716103019"><a name="evs_04_2013_p19541716103019"></a><a name="evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2013_p39375186103019"><a name="evs_04_2013_p39375186103019"></a><a name="evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2013_p38578950103019"><a name="evs_04_2013_p38578950103019"></a><a name="evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p46815658103019"><a name="evs_04_2013_p46815658103019"></a><a name="evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p33971979103019"><a name="evs_04_2013_p33971979103019"></a><a name="evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p21623243103019"><a name="evs_04_2013_p21623243103019"></a><a name="evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p59870541103019"><a name="evs_04_2013_p59870541103019"></a><a name="evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p17675690103019"><a name="evs_04_2013_p17675690103019"></a><a name="evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p6087468103019"><a name="evs_04_2013_p6087468103019"></a><a name="evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2013_p54787218103019"><a name="evs_04_2013_p54787218103019"></a><a name="evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "count": 3, 
        "snapshots_links": [
            {
                "href": "https://172.28.9.185:8776/v2/20a68d6b7a124ae2b6b8a22046ee5966/snapshots/detail?limit=1&marker=fc05d5d7-7e99-42fb-b6f2-9ddd1b990e67", 
                "rel": "next"
            }
        ], 
        "snapshots": [
            {
                "status": "available", 
                "description": null, 
                "updated_at": "2018-06-06T10:58:47.349051", 
                "volume_id": "f687bd70-37b3-4f00-a900-0ba1cfaa5196", 
                "id": "fc05d5d7-7e99-42fb-b6f2-9ddd1b990e67", 
                "size": 1, 
                "os-extended-snapshot-attributes:progress": "100%", 
                "name": "test03", 
                "os-extended-snapshot-attributes:project_id": "20a68d6b7a124ae2b6b8a22046ee5966", 
                "service_type": "EVS", 
                "created_at": "2018-05-30T03:14:44.457975", 
                "metadata": { }
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


## 状态码<a name="section16529200112352"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

