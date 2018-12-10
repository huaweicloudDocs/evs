# 查询云硬盘快照详细信息列表<a name="ZH-CN_TOPIC_0123550104"></a>

## 功能介绍<a name="section29798282112049"></a>

查询云硬盘快照详细列表信息。

## URI<a name="section56404342112049"></a>

-   URI格式

    GET /v2/\{project\_id\}/ os-vendor-snapshots/detail


-   参数说明

    <a name="table37114383112049"></a>
    <table><thead align="left"><tr id="row4845983112049"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p56980371112049"><a name="p56980371112049"></a><a name="p56980371112049"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p52007339112049"><a name="p52007339112049"></a><a name="p52007339112049"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p51844944112049"><a name="p51844944112049"></a><a name="p51844944112049"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row38690921112049"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p46956895112049"><a name="p46956895112049"></a><a name="p46956895112049"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p45412121112049"><a name="p45412121112049"></a><a name="p45412121112049"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p54503167112049"><a name="p54503167112049"></a><a name="p54503167112049"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section54272198112126"></a>

-   参数说明

    <a name="table262294112126"></a>
    <table><thead align="left"><tr id="row15086975112126"><th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.1"><p id="p14085481112126"><a name="p14085481112126"></a><a name="p14085481112126"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.1.5.1.2"><p id="p73303112126"><a name="p73303112126"></a><a name="p73303112126"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p5937586112126"><a name="p5937586112126"></a><a name="p5937586112126"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="p11182433112126"><a name="p11182433112126"></a><a name="p11182433112126"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row33533036112126"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p373114017611"><a name="p373114017611"></a><a name="p373114017611"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p9733405620"><a name="p9733405620"></a><a name="p9733405620"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p167311401064"><a name="p167311401064"></a><a name="p167311401064"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p18735401366"><a name="p18735401366"></a><a name="p18735401366"></a>偏移量。</p>
    <div class="note" id="note158681239962"><a name="note158681239962"></a><a name="note158681239962"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p18766406612"><a name="p18766406612"></a><a name="p18766406612"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row47675000112126"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p137684010618"><a name="p137684010618"></a><a name="p137684010618"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p3769401863"><a name="p3769401863"></a><a name="p3769401863"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1476124010618"><a name="p1476124010618"></a><a name="p1476124010618"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p19769400614"><a name="p19769400614"></a><a name="p19769400614"></a>返回结果个数限制，值为大于0的整数。默认值为1000。</p>
    </td>
    </tr>
    <tr id="row13436622112126"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p1676144017613"><a name="p1676144017613"></a><a name="p1676144017613"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p87614408618"><a name="p87614408618"></a><a name="p87614408618"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p167617402061"><a name="p167617402061"></a><a name="p167617402061"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p97618401260"><a name="p97618401260"></a><a name="p97618401260"></a>云硬盘快照名称。最大支持255个字节。</p>
    </td>
    </tr>
    <tr id="row1141410332065"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p5761401568"><a name="p5761401568"></a><a name="p5761401568"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p77654015617"><a name="p77654015617"></a><a name="p77654015617"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p157694017617"><a name="p157694017617"></a><a name="p157694017617"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p7762404620"><a name="p7762404620"></a><a name="p7762404620"></a>云硬盘快照状态，具体请参见A.3 云硬盘快照状态。</p>
    </td>
    </tr>
    <tr id="row44141633861"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p576204015617"><a name="p576204015617"></a><a name="p576204015617"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p10761840364"><a name="p10761840364"></a><a name="p10761840364"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p97619401468"><a name="p97619401468"></a><a name="p97619401468"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p16761740967"><a name="p16761740967"></a><a name="p16761740967"></a>云硬盘快照对应的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row04149331262"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p076204017617"><a name="p076204017617"></a><a name="p076204017617"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p17761140469"><a name="p17761140469"></a><a name="p17761140469"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1476174016620"><a name="p1476174016620"></a><a name="p1476174016620"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p1476134011615"><a name="p1476134011615"></a><a name="p1476134011615"></a>云硬盘快照对应的云硬盘所在的可用区。</p>
    </td>
    </tr>
    <tr id="row193286371269"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p576184013611"><a name="p576184013611"></a><a name="p576184013611"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p7765401560"><a name="p7765401560"></a><a name="p7765401560"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p0762409612"><a name="p0762409612"></a><a name="p0762409612"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p487845411817"><a name="p487845411817"></a><a name="p487845411817"></a>指定快照id进行过滤。</p>
    </td>
    </tr>
    <tr id="row1132919377615"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p10768401367"><a name="p10768401367"></a><a name="p10768401367"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p1476140761"><a name="p1476140761"></a><a name="p1476140761"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p4765401464"><a name="p4765401464"></a><a name="p4765401464"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p476040768"><a name="p476040768"></a><a name="p476040768"></a>专属存储的名称。</p>
    </td>
    </tr>
    <tr id="row632920371464"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p1768406611"><a name="p1768406611"></a><a name="p1768406611"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p176114016618"><a name="p176114016618"></a><a name="p176114016618"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p14761940262"><a name="p14761940262"></a><a name="p14761940262"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p12763408618"><a name="p12763408618"></a><a name="p12763408618"></a>专属存储ID。</p>
    </td>
    </tr>
    <tr id="row932973714613"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p976174012616"><a name="p976174012616"></a><a name="p976174012616"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p1076440762"><a name="p1076440762"></a><a name="p1076440762"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p776204016615"><a name="p776204016615"></a><a name="p776204016615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p87615401565"><a name="p87615401565"></a><a name="p87615401565"></a>服务类型。</p>
    <p id="p1079317498816"><a name="p1079317498816"></a><a name="p1079317498816"></a>仅支持EVS、DSS、DESS</p>
    <p id="p1497011418920"><a name="p1497011418920"></a><a name="p1497011418920"></a>service_type为EVS时，dedicated_storage_name和dedicated_storage_id必须都为空。</p>
    </td>
    </tr>
    <tr id="row193294371062"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="p11762405613"><a name="p11762405613"></a><a name="p11762405613"></a>enterprise_project_ids</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="p8761401868"><a name="p8761401868"></a><a name="p8761401868"></a>list&lt;string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p47614403614"><a name="p47614403614"></a><a name="p47614403614"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p13996325393"><a name="p13996325393"></a><a name="p13996325393"></a>企业项目id列表。</p>
    <p id="p2076940961"><a name="p2076940961"></a><a name="p2076940961"></a>格式为enterprise_project_ids =['eid1','eid2',...,'eidx']，会返回对应企业项目id的快照详情列表。“enterprise_project_ids”中的无效企业项目id直接忽略。</p>
    <p id="p27614402614"><a name="p27614402614"></a><a name="p27614402614"></a>最多可输入100个企业项目id。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    无


## 响应<a name="section50618846112239"></a>

-   响应参数

    <a name="table55593749112239"></a>
    <table><thead align="left"><tr id="row12503066112239"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="p6115391112239"><a name="p6115391112239"></a><a name="p6115391112239"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="p25584640112239"><a name="p25584640112239"></a><a name="p25584640112239"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p21559929112239"><a name="p21559929112239"></a><a name="p21559929112239"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59821639112239"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p1254928141117"><a name="p1254928141117"></a><a name="p1254928141117"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p32542028171112"><a name="p32542028171112"></a><a name="p32542028171112"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1325417283117"><a name="p1325417283117"></a><a name="p1325417283117"></a>快照的总数量，不受limit、offset参数的影响。</p>
    </td>
    </tr>
    <tr id="row60405564112239"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p16254228181117"><a name="p16254228181117"></a><a name="p16254228181117"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p52546289117"><a name="p52546289117"></a><a name="p52546289117"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1825462821113"><a name="p1825462821113"></a><a name="p1825462821113"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="row1081819219117"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p1025582813117"><a name="p1025582813117"></a><a name="p1025582813117"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p1025513281119"><a name="p1025513281119"></a><a name="p1025513281119"></a>list&lt;map&lt;string,string&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1255112811117"><a name="p1255112811117"></a><a name="p1255112811117"></a>云硬盘快照列表查询位置标记，与响应body中的snapshots同级，当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   snapshots参数说明

    <a name="table43291794165"></a>
    <table><thead align="left"><tr id="row669989131614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="p1369912961618"><a name="p1369912961618"></a><a name="p1369912961618"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.53%" id="mcps1.1.4.1.2"><p id="p1069917913161"><a name="p1069917913161"></a><a name="p1069917913161"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="p196991790169"><a name="p196991790169"></a><a name="p196991790169"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row769918919163"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p7699149141616"><a name="p7699149141616"></a><a name="p7699149141616"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p970179141613"><a name="p970179141613"></a><a name="p970179141613"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p1370119131610"><a name="p1370119131610"></a><a name="p1370119131610"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row470139171619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p87011094167"><a name="p87011094167"></a><a name="p87011094167"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p11701119111617"><a name="p11701119111617"></a><a name="p11701119111617"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p14701129151612"><a name="p14701129151612"></a><a name="p14701129151612"></a>云硬盘快照的状态，具体请参见A.3 云硬盘快照状态。</p>
    </td>
    </tr>
    <tr id="row1970113916161"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p127019912167"><a name="p127019912167"></a><a name="p127019912167"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p13701691161"><a name="p13701691161"></a><a name="p13701691161"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p1470118917161"><a name="p1470118917161"></a><a name="p1470118917161"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row127011894169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p570114991613"><a name="p570114991613"></a><a name="p570114991613"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p197013921610"><a name="p197013921610"></a><a name="p197013921610"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p127014921612"><a name="p127014921612"></a><a name="p127014921612"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row0701796168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p970115917165"><a name="p970115917165"></a><a name="p970115917165"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p370109111619"><a name="p370109111619"></a><a name="p370109111619"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p1370113921616"><a name="p1370113921616"></a><a name="p1370113921616"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="row14701193168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p11701398164"><a name="p11701398164"></a><a name="p11701398164"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p870120981616"><a name="p870120981616"></a><a name="p870120981616"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p470117911615"><a name="p470117911615"></a><a name="p470117911615"></a>云硬盘快照更新时间。</p>
    </td>
    </tr>
    <tr id="row1670169151619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p470112913161"><a name="p470112913161"></a><a name="p470112913161"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p187013901618"><a name="p187013901618"></a><a name="p187013901618"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p1470112981613"><a name="p1470112981613"></a><a name="p1470112981613"></a>云硬盘快照的元数据信息。</p>
    <p id="p1567410577152"><a name="p1567410577152"></a><a name="p1567410577152"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="row2701209191619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1170120991610"><a name="p1170120991610"></a><a name="p1170120991610"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p470220919169"><a name="p470220919169"></a><a name="p470220919169"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p117021914162"><a name="p117021914162"></a><a name="p117021914162"></a>快照所属的云硬盘。</p>
    </td>
    </tr>
    <tr id="row7702129121618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1570215918168"><a name="p1570215918168"></a><a name="p1570215918168"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p470213913168"><a name="p470213913168"></a><a name="p470213913168"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p19702179121617"><a name="p19702179121617"></a><a name="p19702179121617"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="row570214931611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1870220916166"><a name="p1870220916166"></a><a name="p1870220916166"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p16702096169"><a name="p16702096169"></a><a name="p16702096169"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p3702199191611"><a name="p3702199191611"></a><a name="p3702199191611"></a>租户ID。</p>
    </td>
    </tr>
    <tr id="row470219961618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1770210915169"><a name="p1770210915169"></a><a name="p1770210915169"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p1070212915167"><a name="p1070212915167"></a><a name="p1070212915167"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p170219911618"><a name="p170219911618"></a><a name="p170219911618"></a>快照进度。</p>
    </td>
    </tr>
    <tr id="row13702159201614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p47025941614"><a name="p47025941614"></a><a name="p47025941614"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p147021695165"><a name="p147021695165"></a><a name="p147021695165"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p670212941619"><a name="p670212941619"></a><a name="p670212941619"></a>专属存储的名称。</p>
    </td>
    </tr>
    <tr id="row970217913169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1470214910165"><a name="p1470214910165"></a><a name="p1470214910165"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p137021597169"><a name="p137021597169"></a><a name="p137021597169"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p117024915160"><a name="p117024915160"></a><a name="p117024915160"></a>专属存储ID。</p>
    </td>
    </tr>
    <tr id="row1070209171613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p177022914166"><a name="p177022914166"></a><a name="p177022914166"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p4702495168"><a name="p4702495168"></a><a name="p4702495168"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p2702199161612"><a name="p2702199161612"></a><a name="p2702199161612"></a>服务类型。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "count": 3,
        "snapshots_links": [{
            "href": "https://172.28.9.185:8776/v2/20a68d6b7a124ae2b6b8a22046ee5966/snapshots/detail?limit=1&marker=fc05d5d7-7e99-42fb-b6f2-9ddd1b990e67",
            "rel": "next"
        }],
        "snapshots": [{
            "status": "available",
            "description": null,
            "dedicated_storage_id": null,
            "updated_at": "2018-06-06T10:58:47.349051",
            "volume_id": "f687bd70-37b3-4f00-a900-0ba1cfaa5196",
            "id": "fc05d5d7-7e99-42fb-b6f2-9ddd1b990e67",
            "size": 1,
            "os-extended-snapshot-attributes:progress": "100%",
            "name": "test03",
            "os-extended-snapshot-attributes:project_id": "20a68d6b7a124ae2b6b8a22046ee5966",
            "dedicated_storage_name": null,
            "service_type": "EVS",
            "created_at": "2018-05-30T03:14:44.457975",
            "metadata": {
                
            }
        }]
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


## 返回值<a name="section16529200112352"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

