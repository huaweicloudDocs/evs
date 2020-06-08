# 查询云硬盘列表<a name="evs_04_2068"></a>

## 功能介绍<a name="section60214390"></a>

查询云硬盘列表。

## URI<a name="section5058598"></a>

-   URI格式

    GET /v2/\{project\_id\}/volumes

-   参数说明

    <a name="table58294385"></a>
    <table><thead align="left"><tr id="row24683273"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p53188122"><a name="p53188122"></a><a name="p53188122"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p13270664"><a name="p13270664"></a><a name="p13270664"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p1182010"><a name="p1182010"></a><a name="p1182010"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row28634009"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p37653388"><a name="p37653388"></a><a name="p37653388"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p30025596"><a name="p30025596"></a><a name="p30025596"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p16154192"><a name="p16154192"></a><a name="p16154192"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="table48630339152531"></a>
    <table><thead align="left"><tr id="row30502978152531"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="p54822134152531"><a name="p54822134152531"></a><a name="p54822134152531"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.2"><p id="p11407863152531"><a name="p11407863152531"></a><a name="p11407863152531"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p51621676152531"><a name="p51621676152531"></a><a name="p51621676152531"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="p20606205152531"><a name="p20606205152531"></a><a name="p20606205152531"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row58489940152531"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p49168107152914"><a name="p49168107152914"></a><a name="p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p23193765152914"><a name="p23193765152914"></a><a name="p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p66755704152914"><a name="p66755704152914"></a><a name="p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p38502923152914"><a name="p38502923152914"></a><a name="p38502923152914"></a><span id="text138882914373"><a name="text138882914373"></a><a name="text138882914373"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="row38948343152859"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p17125818152914"><a name="p17125818152914"></a><a name="p17125818152914"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p14491527153320"><a name="p14491527153320"></a><a name="p14491527153320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p22259725152914"><a name="p22259725152914"></a><a name="p22259725152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p58207321152914"><a name="p58207321152914"></a><a name="p58207321152914"></a>云硬盘名称。<span id="text37302935152245"><a name="text37302935152245"></a><a name="text37302935152245"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row61932754152911"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p20335623152914"><a name="p20335623152914"></a><a name="p20335623152914"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p36572733152914"><a name="p36572733152914"></a><a name="p36572733152914"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p9601396152914"><a name="p9601396152914"></a><a name="p9601396152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p39515603152914"><a name="p39515603152914"></a><a name="p39515603152914"></a>返回结果个数限制。</p>
    <p id="p99431755191418"><a name="p99431755191418"></a><a name="p99431755191418"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="p14657115572511"><a name="p14657115572511"></a><a name="p14657115572511"></a>当租户所有的云硬盘数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="p1233994321914"><a name="p1233994321914"></a><a name="p1233994321914"></a><strong id="b15619135183016"><a name="b15619135183016"></a><a name="b15619135183016"></a>GET /v2/<em id="i86219512306"><a name="i86219512306"></a><a name="i86219512306"></a>xxx</em>/volumes?limit=50</strong>，表示查询第1~50个云硬盘。<strong id="b18611337305"><a name="b18611337305"></a><a name="b18611337305"></a>GET /v2/<em id="i149081817173015"><a name="i149081817173015"></a><a name="i149081817173015"></a>xxx</em>/volumes?offset=50&amp;limit=50</strong>，表示查询第51~100个云硬盘。</p>
    </td>
    </tr>
    <tr id="row4561665015299"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p17172513152914"><a name="p17172513152914"></a><a name="p17172513152914"></a>sort_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p43305182153332"><a name="p43305182153332"></a><a name="p43305182153332"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p60186269152914"><a name="p60186269152914"></a><a name="p60186269152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p43249593152914"><a name="p43249593152914"></a><a name="p43249593152914"></a>返回结果按该关键字排序，支持id，status，size，created_at等关键字，默认为“created_at”。</p>
    </td>
    </tr>
    <tr id="row5831630415296"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p54896674152914"><a name="p54896674152914"></a><a name="p54896674152914"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p4460297153338"><a name="p4460297153338"></a><a name="p4460297153338"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p3809857152914"><a name="p3809857152914"></a><a name="p3809857152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><div class="p" id="p2025341125211"><a name="p2025341125211"></a><a name="p2025341125211"></a>返回结果按照降序或升序排列，默认为“desc”。<a name="ul107075455529"></a><a name="ul107075455529"></a><ul id="ul107075455529"><li>降序：desc</li><li>升序：asc</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row1669400215294"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p19336748152914"><a name="p19336748152914"></a><a name="p19336748152914"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p22139675153443"><a name="p22139675153443"></a><a name="p22139675153443"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p32652321152914"><a name="p32652321152914"></a><a name="p32652321152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p1812219549521"><a name="p1812219549521"></a><a name="p1812219549521"></a>偏移量</p>
    <p id="p27592310152914"><a name="p27592310152914"></a><a name="p27592310152914"></a>偏移量为一个大于0小于磁盘总个数的整数，表示查询该偏移量后面的所有的云硬盘。</p>
    </td>
    </tr>
    <tr id="row4150243115292"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p49243814152914"><a name="p49243814152914"></a><a name="p49243814152914"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p15960789153343"><a name="p15960789153343"></a><a name="p15960789153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p26598214152914"><a name="p26598214152914"></a><a name="p26598214152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p6971702152914"><a name="p6971702152914"></a><a name="p6971702152914"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row33130210152857"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p49206403152914"><a name="p49206403152914"></a><a name="p49206403152914"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p6448822153343"><a name="p6448822153343"></a><a name="p6448822153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p49578561152914"><a name="p49578561152914"></a><a name="p49578561152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p56440503152914"><a name="p56440503152914"></a><a name="p56440503152914"></a>云硬盘元数据。</p>
    </td>
    </tr>
    <tr id="row20664390152531"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p7393147152914"><a name="p7393147152914"></a><a name="p7393147152914"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p59504247153343"><a name="p59504247153343"></a><a name="p59504247153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p53841259152914"><a name="p53841259152914"></a><a name="p53841259152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p66174752152914"><a name="p66174752152914"></a><a name="p66174752152914"></a>AZ信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询状态为available的云硬盘为例。

-   请求样例

    ```
    GET https://{endpoint}/v2/{project_id}/volumes?status=available
    ```


## 响应消息<a name="section7093323"></a>

-   响应参数

    <a name="table682710305552"></a>
    <table><thead align="left"><tr id="row18828730125511"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p17828103014554"><a name="p17828103014554"></a><a name="p17828103014554"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p982813025513"><a name="p982813025513"></a><a name="p982813025513"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p10828123085512"><a name="p10828123085512"></a><a name="p10828123085512"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row6828153014554"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p1828130105513"><a name="p1828130105513"></a><a name="p1828130105513"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p582813013559"><a name="p582813013559"></a><a name="p582813013559"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p158281930195514"><a name="p158281930195514"></a><a name="p158281930195514"></a>查询请求返回的云硬盘列表，请参见<a href="#li3451542201439">•volumes参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row16651711135716"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p20139619153059"><a name="p20139619153059"></a><a name="p20139619153059"></a>volumes_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p20696419153059"><a name="p20696419153059"></a><a name="p20696419153059"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p27977197153059"><a name="p27977197153059"></a><a name="p27977197153059"></a>云硬盘列表查询位置标记。如果本次查询只返回部分列表信息时，会返回查询到的当前磁盘mark标记的url，可以继续使用这个url查询剩余列表信息。</p>
    </td>
    </tr>
    <tr id="row1383518379555"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li3451542201439"></a>volumes参数说明

    <a name="table34701445142557"></a>
    <table><thead align="left"><tr id="row12524911142557"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p7884856142557"><a name="p7884856142557"></a><a name="p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p34693598142557"><a name="p34693598142557"></a><a name="p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p58539486142557"><a name="p58539486142557"></a><a name="p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row444782011610"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p9640386153059"><a name="p9640386153059"></a><a name="p9640386153059"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p42673774153059"><a name="p42673774153059"></a><a name="p42673774153059"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p4455949153059"><a name="p4455949153059"></a><a name="p4455949153059"></a>云硬盘ID</p>
    </td>
    </tr>
    <tr id="row44077962142557"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p27161806153059"><a name="p27161806153059"></a><a name="p27161806153059"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p52622641153059"><a name="p52622641153059"></a><a name="p52622641153059"></a>list&lt;map&lt;String, String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p49157451153059"><a name="p49157451153059"></a><a name="p49157451153059"></a>云硬盘URI自描述信息，请参见<a href="#li1077125119136">•links参数说明</a></p>
    </td>
    </tr>
    <tr id="row16186817142557"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p66757462153059"><a name="p66757462153059"></a><a name="p66757462153059"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p38645307153059"><a name="p38645307153059"></a><a name="p38645307153059"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p14572483153059"><a name="p14572483153059"></a><a name="p14572483153059"></a>云硬盘名称。<span id="text67711291"><a name="text67711291"></a><a name="text67711291"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li1077125119136"></a>links参数说明

    <a name="evs_04_2067_table24355024185927"></a>
    <table><thead align="left"><tr id="evs_04_2067_row16225418185927"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2067_p39190461185927"><a name="evs_04_2067_p39190461185927"></a><a name="evs_04_2067_p39190461185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2067_p20310744185927"><a name="evs_04_2067_p20310744185927"></a><a name="evs_04_2067_p20310744185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="evs_04_2067_p47699944185927"><a name="evs_04_2067_p47699944185927"></a><a name="evs_04_2067_p47699944185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2067_row38490285185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2067_p30705403185927"><a name="evs_04_2067_p30705403185927"></a><a name="evs_04_2067_p30705403185927"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2067_p4109689185927"><a name="evs_04_2067_p4109689185927"></a><a name="evs_04_2067_p4109689185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="evs_04_2067_p53015590185927"><a name="evs_04_2067_p53015590185927"></a><a name="evs_04_2067_p53015590185927"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="evs_04_2067_row7378265185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2067_p60768596185927"><a name="evs_04_2067_p60768596185927"></a><a name="evs_04_2067_p60768596185927"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2067_p23309219185927"><a name="evs_04_2067_p23309219185927"></a><a name="evs_04_2067_p23309219185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="evs_04_2067_p57795935185927"><a name="evs_04_2067_p57795935185927"></a><a name="evs_04_2067_p57795935185927"></a>快捷链接标记名称。</p>
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
        "volumes": [
            {
                "id": "6b604cef-9bd8-4f5a-ae56-45839e6e1f0a", 
                "links": [
                    {
                        "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/6b604cef-9bd8-4f5a-ae56-45839e6e1f0a", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/6b604cef-9bd8-4f5a-ae56-45839e6e1f0a", 
                        "rel": "bookmark"
                    }
                ], 
                "name": "zjb_u25_test"
            }, 
            {
                "id": "2bce4552-9a7d-48fa-8484-abbbf64b206e", 
                "links": [
                    {
                        "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/2bce4552-9a7d-48fa-8484-abbbf64b206e", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/2bce4552-9a7d-48fa-8484-abbbf64b206e", 
                        "rel": "bookmark"
                    }
                ], 
                "name": "zjb_u25_test"
            }, 
            {
                "id": "3f1b98ec-a8b5-4e92-a727-88def62d5ad3", 
                "links": [
                    {
                        "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/3f1b98ec-a8b5-4e92-a727-88def62d5ad3", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/3f1b98ec-a8b5-4e92-a727-88def62d5ad3", 
                        "rel": "bookmark"
                    }
                ], 
                "name": "zjb_u25_test"
            }
        ], 
        "volumes_links": [
            {
                "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes?limit=3&marker=3f1b98ec-a8b5-4e92-a727-88def62d5ad3", 
                "rel": "next"
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


## 状态码<a name="section63839913"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

