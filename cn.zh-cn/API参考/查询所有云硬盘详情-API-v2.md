# 查询所有云硬盘详情<a name="zh-cn_topic_0127947068"></a>

## 功能介绍<a name="section37076589"></a>

查询所有云硬盘的详细信息。支持企业项目授权功能。

## URI<a name="section65253851"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudvolumes/detail

-   参数说明

    <a name="table17404391"></a>
    <table><thead align="left"><tr id="row60677108"><th class="cellrowborder" valign="top" width="33.33%" id="mcps1.1.4.1.1"><p id="p15898735"><a name="p15898735"></a><a name="p15898735"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.06%" id="mcps1.1.4.1.2"><p id="p12729171"><a name="p12729171"></a><a name="p12729171"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.61%" id="mcps1.1.4.1.3"><p id="p24429894"><a name="p24429894"></a><a name="p24429894"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row32664435"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p28573568"><a name="p28573568"></a><a name="p28573568"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.06%" headers="mcps1.1.4.1.2 "><p id="p32757653"><a name="p32757653"></a><a name="p32757653"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.61%" headers="mcps1.1.4.1.3 "><p id="p36124251"><a name="p36124251"></a><a name="p36124251"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="table48630339152531"></a>
    <table><thead align="left"><tr id="row30502978152531"><th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.1"><p id="p1248947195510"><a name="p1248947195510"></a><a name="p1248947195510"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="p11407863152531"><a name="p11407863152531"></a><a name="p11407863152531"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p51621676152531"><a name="p51621676152531"></a><a name="p51621676152531"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p20606205152531"><a name="p20606205152531"></a><a name="p20606205152531"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row58489940152531"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p49168107152914"><a name="p49168107152914"></a><a name="p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p23193765152914"><a name="p23193765152914"></a><a name="p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p66755704152914"><a name="p66755704152914"></a><a name="p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p38502923152914"><a name="p38502923152914"></a><a name="p38502923152914"></a><span id="text1258514515457"><a name="text1258514515457"></a><a name="text1258514515457"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="row38948343152859"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p17125818152914"><a name="p17125818152914"></a><a name="p17125818152914"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p14491527153320"><a name="p14491527153320"></a><a name="p14491527153320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p22259725152914"><a name="p22259725152914"></a><a name="p22259725152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p58207321152914"><a name="p58207321152914"></a><a name="p58207321152914"></a>云硬盘名称。<span id="text37302935152245"><a name="text37302935152245"></a><a name="text37302935152245"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row61932754152911"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p20335623152914"><a name="p20335623152914"></a><a name="p20335623152914"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p36572733152914"><a name="p36572733152914"></a><a name="p36572733152914"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p9601396152914"><a name="p9601396152914"></a><a name="p9601396152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p39515603152914"><a name="p39515603152914"></a><a name="p39515603152914"></a>返回结果个数限制。</p>
    <p id="p149409221913"><a name="p149409221913"></a><a name="p149409221913"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    </td>
    </tr>
    <tr id="row4561665015299"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p17172513152914"><a name="p17172513152914"></a><a name="p17172513152914"></a>sort_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p43305182153332"><a name="p43305182153332"></a><a name="p43305182153332"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p60186269152914"><a name="p60186269152914"></a><a name="p60186269152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p1015961694520"><a name="p1015961694520"></a><a name="p1015961694520"></a>返回结果按该关键字排序，支持id，status，size，created_at等关键字，默认为“created_at”。</p>
    </td>
    </tr>
    <tr id="row5831630415296"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p54896674152914"><a name="p54896674152914"></a><a name="p54896674152914"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p4460297153338"><a name="p4460297153338"></a><a name="p4460297153338"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p3809857152914"><a name="p3809857152914"></a><a name="p3809857152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><div class="p" id="p85141444124814"><a name="p85141444124814"></a><a name="p85141444124814"></a>返回结果按照降序或升序排列，默认为“desc”。<a name="ul1097217103492"></a><a name="ul1097217103492"></a><ul id="ul1097217103492"><li>降序：desc</li><li>升序：asc</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row1669400215294"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p19336748152914"><a name="p19336748152914"></a><a name="p19336748152914"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p22139675153443"><a name="p22139675153443"></a><a name="p22139675153443"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p32652321152914"><a name="p32652321152914"></a><a name="p32652321152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p27592310152914"><a name="p27592310152914"></a><a name="p27592310152914"></a>偏移量（偏移量为一个大于0小于磁盘总个数的整数，表示查询该偏移量后面的所有的磁盘）。</p>
    </td>
    </tr>
    <tr id="row4150243115292"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p49243814152914"><a name="p49243814152914"></a><a name="p49243814152914"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p15960789153343"><a name="p15960789153343"></a><a name="p15960789153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p26598214152914"><a name="p26598214152914"></a><a name="p26598214152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p6971702152914"><a name="p6971702152914"></a><a name="p6971702152914"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row33130210152857"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p49206403152914"><a name="p49206403152914"></a><a name="p49206403152914"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p6448822153343"><a name="p6448822153343"></a><a name="p6448822153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p49578561152914"><a name="p49578561152914"></a><a name="p49578561152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p56440503152914"><a name="p56440503152914"></a><a name="p56440503152914"></a>云硬盘元数据。</p>
    </td>
    </tr>
    <tr id="row20664390152531"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p7393147152914"><a name="p7393147152914"></a><a name="p7393147152914"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p59504247153343"><a name="p59504247153343"></a><a name="p59504247153343"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p53841259152914"><a name="p53841259152914"></a><a name="p53841259152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p66174752152914"><a name="p66174752152914"></a><a name="p66174752152914"></a>AZ信息。</p>
    </td>
    </tr>
    <tr id="row433212398420"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p1441713429428"><a name="p1441713429428"></a><a name="p1441713429428"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p1541984214429"><a name="p1541984214429"></a><a name="p1541984214429"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p18419174234210"><a name="p18419174234210"></a><a name="p18419174234210"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><div class="p" id="p16419144210429"><a name="p16419144210429"></a><a name="p16419144210429"></a>是否为共享云硬盘。<a name="ul202952187368"></a><a name="ul202952187368"></a><ul id="ul202952187368"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row193541948124512"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p25711629468"><a name="p25711629468"></a><a name="p25711629468"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p45717224620"><a name="p45717224620"></a><a name="p45717224620"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p2571172104610"><a name="p2571172104610"></a><a name="p2571172104610"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p1457172174620"><a name="p1457172174620"></a><a name="p1457172174620"></a>服务类型，仅支持EVS、DSS、DESS。</p>
    </td>
    </tr>
    <tr id="row176903519453"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p1857152194612"><a name="p1857152194612"></a><a name="p1857152194612"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p18571162124611"><a name="p18571162124611"></a><a name="p18571162124611"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p857120219462"><a name="p857120219462"></a><a name="p857120219462"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p1857162154615"><a name="p1857162154615"></a><a name="p1857162154615"></a>专属存储池ID，可过滤出该专属存储池下的所有云硬盘，必须精确匹配。</p>
    </td>
    </tr>
    <tr id="row10814055174517"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p125717218464"><a name="p125717218464"></a><a name="p125717218464"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p157110213469"><a name="p157110213469"></a><a name="p157110213469"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p1557117211469"><a name="p1557117211469"></a><a name="p1557117211469"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p2057114211466"><a name="p2057114211466"></a><a name="p2057114211466"></a>专属存储池的名字，可过滤出该专属存储池下的所有云硬盘，支持模糊匹配。</p>
    </td>
    </tr>
    <tr id="row1484019429236"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p4338154142317"><a name="p4338154142317"></a><a name="p4338154142317"></a>volume_type_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p193381354122315"><a name="p193381354122315"></a><a name="p193381354122315"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p3338754132315"><a name="p3338754132315"></a><a name="p3338754132315"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p3338155422319"><a name="p3338155422319"></a><a name="p3338155422319"></a>云硬盘类型id。</p>
    <p id="p14520972319"><a name="p14520972319"></a><a name="p14520972319"></a>通过<a href="查询云硬盘类型列表-Cinder-v3.md">查询云硬盘类型列表</a>可以查到，即volume_types参数说明表格中的“id”。</p>
    </td>
    </tr>
    <tr id="row1758151163616"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p85819112362"><a name="p85819112362"></a><a name="p85819112362"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p75815112367"><a name="p75815112367"></a><a name="p75815112367"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p3581911193617"><a name="p3581911193617"></a><a name="p3581911193617"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p45812118360"><a name="p45812118360"></a><a name="p45812118360"></a>云硬盘id。</p>
    </td>
    </tr>
    <tr id="row3113151415129"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p11113121412125"><a name="p11113121412125"></a><a name="p11113121412125"></a>ids</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p1811371412124"><a name="p1811371412124"></a><a name="p1811371412124"></a>Array of strings</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p9113191413128"><a name="p9113191413128"></a><a name="p9113191413128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p7651828190"><a name="p7651828190"></a><a name="p7651828190"></a>云硬盘id列表，格式为ids=['id1','id2',...,'idx']，返回“ids”中有效id的云硬盘详情，无效的id会被忽略。</p>
    <p id="p2640155471814"><a name="p2640155471814"></a><a name="p2640155471814"></a>支持查询最多60个id对应的云硬盘详情。</p>
    <p id="p649163291315"><a name="p649163291315"></a><a name="p649163291315"></a>如果“id”和“ids”查询参数同时存在，“id”会被忽略。</p>
    </td>
    </tr>
    <tr id="row16449173514611"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p17746165016465"><a name="p17746165016465"></a><a name="p17746165016465"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p1474605013468"><a name="p1474605013468"></a><a name="p1474605013468"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p117461050114615"><a name="p117461050114615"></a><a name="p117461050114615"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p2746950164617"><a name="p2746950164617"></a><a name="p2746950164617"></a>指定企业项目id进行过滤。</p>
    <p id="p4746185064614"><a name="p4746185064614"></a><a name="p4746185064614"></a>传入“all_granted_eps”，代表查询权限范围内的所有企业项目下的云硬盘。</p>
    <div class="note" id="note1664605004618"><a name="note1664605004618"></a><a name="note1664605004618"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0020235144_p18336524404"><a name="zh-cn_topic_0020235144_p18336524404"></a><a name="zh-cn_topic_0020235144_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section50413755"></a>

以查询状态为available的共享云硬盘为例。

-   请求样例：

    ```
    GET https://{endpoint}/v2/{project_id}/cloudvolumes/detail?status=available&multiattach=true
    ```


## 响应消息<a name="section1042116365411"></a>

-   响应参数

    <a name="zh-cn_topic_0098680634_table34701445142557"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_row12524911142557"><th class="cellrowborder" valign="top" width="18.82%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_p7884856142557"><a name="zh-cn_topic_0098680634_p7884856142557"></a><a name="zh-cn_topic_0098680634_p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.53%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_p34693598142557"><a name="zh-cn_topic_0098680634_p34693598142557"></a><a name="zh-cn_topic_0098680634_p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_p58539486142557"><a name="zh-cn_topic_0098680634_p58539486142557"></a><a name="zh-cn_topic_0098680634_p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_row42521635152937"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p14844956152939"><a name="zh-cn_topic_0098680634_p14844956152939"></a><a name="zh-cn_topic_0098680634_p14844956152939"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p61590812152939"><a name="zh-cn_topic_0098680634_p61590812152939"></a><a name="zh-cn_topic_0098680634_p61590812152939"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p34852014152939"><a name="zh-cn_topic_0098680634_p34852014152939"></a><a name="zh-cn_topic_0098680634_p34852014152939"></a>查询请求返回的云硬盘列表，请参见<a href="#zh-cn_topic_0098680634_li1435719516515">•volumes参数说明</a> 。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row15981815184017"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p16197151919407"><a name="zh-cn_topic_0098680634_p16197151919407"></a><a name="zh-cn_topic_0098680634_p16197151919407"></a>volumes_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p12197151915402"><a name="zh-cn_topic_0098680634_p12197151915402"></a><a name="zh-cn_topic_0098680634_p12197151915402"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p17197141954017"><a name="zh-cn_topic_0098680634_p17197141954017"></a><a name="zh-cn_topic_0098680634_p17197141954017"></a>云硬盘列表查询位置标记。如果本次查询只返回部分列表信息时，会返回查询到的当前磁盘mark标记的url，可以继续使用这个url查询剩余列表信息，请参见<a href="#zh-cn_topic_0098680634_li1077125119136">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row444782011610"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p0730182411511"><a name="zh-cn_topic_0098680634_p0730182411511"></a><a name="zh-cn_topic_0098680634_p0730182411511"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1573092465118"><a name="zh-cn_topic_0098680634_p1573092465118"></a><a name="zh-cn_topic_0098680634_p1573092465118"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p10730152455119"><a name="zh-cn_topic_0098680634_p10730152455119"></a><a name="zh-cn_topic_0098680634_p10730152455119"></a>查询到的云硬盘总数量，不受分页影响。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row141841349561"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p129522216412"><a name="zh-cn_topic_0098680634_p129522216412"></a><a name="zh-cn_topic_0098680634_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1595262111415"><a name="zh-cn_topic_0098680634_p1595262111415"></a><a name="zh-cn_topic_0098680634_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p109527215417"><a name="zh-cn_topic_0098680634_p109527215417"></a><a name="zh-cn_topic_0098680634_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#zh-cn_topic_0098680634_li0419202382514"> error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0098680634_li1435719516515"></a>volumes参数说明

    <a name="zh-cn_topic_0098680634_table9519314115310"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_row07772014165315"><th class="cellrowborder" valign="top" width="20.1%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_p977791416537"><a name="zh-cn_topic_0098680634_p977791416537"></a><a name="zh-cn_topic_0098680634_p977791416537"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_p1777191445316"><a name="zh-cn_topic_0098680634_p1777191445316"></a><a name="zh-cn_topic_0098680634_p1777191445316"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_p9894141375614"><a name="zh-cn_topic_0098680634_p9894141375614"></a><a name="zh-cn_topic_0098680634_p9894141375614"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_row157775141539"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1577716144532"><a name="zh-cn_topic_0098680634_p1577716144532"></a><a name="zh-cn_topic_0098680634_p1577716144532"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p2077712145534"><a name="zh-cn_topic_0098680634_p2077712145534"></a><a name="zh-cn_topic_0098680634_p2077712145534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p577711405310"><a name="zh-cn_topic_0098680634_p577711405310"></a><a name="zh-cn_topic_0098680634_p577711405310"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row197771014165318"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1777771465312"><a name="zh-cn_topic_0098680634_p1777771465312"></a><a name="zh-cn_topic_0098680634_p1777771465312"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1577781445313"><a name="zh-cn_topic_0098680634_p1577781445313"></a><a name="zh-cn_topic_0098680634_p1577781445313"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p377719149537"><a name="zh-cn_topic_0098680634_p377719149537"></a><a name="zh-cn_topic_0098680634_p377719149537"></a>云硬盘URI自描述信息，请参见<a href="#zh-cn_topic_0098680634_li1077125119136">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row14777131435317"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p677751415313"><a name="zh-cn_topic_0098680634_p677751415313"></a><a name="zh-cn_topic_0098680634_p677751415313"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p7777614185310"><a name="zh-cn_topic_0098680634_p7777614185310"></a><a name="zh-cn_topic_0098680634_p7777614185310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p977716143532"><a name="zh-cn_topic_0098680634_p977716143532"></a><a name="zh-cn_topic_0098680634_p977716143532"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row377719149532"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p17777714195313"><a name="zh-cn_topic_0098680634_p17777714195313"></a><a name="zh-cn_topic_0098680634_p17777714195313"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p17771514195316"><a name="zh-cn_topic_0098680634_p17771514195316"></a><a name="zh-cn_topic_0098680634_p17771514195316"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p137771014165316"><a name="zh-cn_topic_0098680634_p137771014165316"></a><a name="zh-cn_topic_0098680634_p137771014165316"></a>云硬盘状态，请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1577714145535"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p8777171445317"><a name="zh-cn_topic_0098680634_p8777171445317"></a><a name="zh-cn_topic_0098680634_p8777171445317"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p14777161435318"><a name="zh-cn_topic_0098680634_p14777161435318"></a><a name="zh-cn_topic_0098680634_p14777161435318"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1977761417532"><a name="zh-cn_topic_0098680634_p1977761417532"></a><a name="zh-cn_topic_0098680634_p1977761417532"></a>挂载信息，请参见<a href="#zh-cn_topic_0098680634_li12430153610291">•attachments参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row137779149535"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p7777614155317"><a name="zh-cn_topic_0098680634_p7777614155317"></a><a name="zh-cn_topic_0098680634_p7777614155317"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p977731415320"><a name="zh-cn_topic_0098680634_p977731415320"></a><a name="zh-cn_topic_0098680634_p977731415320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1577710143534"><a name="zh-cn_topic_0098680634_p1577710143534"></a><a name="zh-cn_topic_0098680634_p1577710143534"></a>云硬盘所属的AZ信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row577741415319"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p16777171425319"><a name="zh-cn_topic_0098680634_p16777171425319"></a><a name="zh-cn_topic_0098680634_p16777171425319"></a>os-vol-host-attr:host</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p8777201414538"><a name="zh-cn_topic_0098680634_p8777201414538"></a><a name="zh-cn_topic_0098680634_p8777201414538"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1677701445318"><a name="zh-cn_topic_0098680634_p1677701445318"></a><a name="zh-cn_topic_0098680634_p1677701445318"></a><span id="zh-cn_topic_0098680634_text542510472571"><a name="zh-cn_topic_0098680634_text542510472571"></a><a name="zh-cn_topic_0098680634_text542510472571"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row19777171445315"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p13777914155316"><a name="zh-cn_topic_0098680634_p13777914155316"></a><a name="zh-cn_topic_0098680634_p13777914155316"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p9777101475310"><a name="zh-cn_topic_0098680634_p9777101475310"></a><a name="zh-cn_topic_0098680634_p9777101475310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p97771314105319"><a name="zh-cn_topic_0098680634_p97771314105319"></a><a name="zh-cn_topic_0098680634_p97771314105319"></a>源云硬盘ID，如果是从源云硬盘创建，则有值。</p>
    <p id="zh-cn_topic_0098680634_p1066441210106"><a name="zh-cn_topic_0098680634_p1066441210106"></a><a name="zh-cn_topic_0098680634_p1066441210106"></a><span id="zh-cn_topic_0098680634_text88578719717"><a name="zh-cn_topic_0098680634_text88578719717"></a><a name="zh-cn_topic_0098680634_text88578719717"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1577751412539"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p10777201435317"><a name="zh-cn_topic_0098680634_p10777201435317"></a><a name="zh-cn_topic_0098680634_p10777201435317"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p87771614125315"><a name="zh-cn_topic_0098680634_p87771614125315"></a><a name="zh-cn_topic_0098680634_p87771614125315"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p877714143532"><a name="zh-cn_topic_0098680634_p877714143532"></a><a name="zh-cn_topic_0098680634_p877714143532"></a>快照ID，如果是从快照创建，则有值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row7777114155318"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p8777151410534"><a name="zh-cn_topic_0098680634_p8777151410534"></a><a name="zh-cn_topic_0098680634_p8777151410534"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p17778191485311"><a name="zh-cn_topic_0098680634_p17778191485311"></a><a name="zh-cn_topic_0098680634_p17778191485311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p3778181416532"><a name="zh-cn_topic_0098680634_p3778181416532"></a><a name="zh-cn_topic_0098680634_p3778181416532"></a>描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row67785148537"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p277810146537"><a name="zh-cn_topic_0098680634_p277810146537"></a><a name="zh-cn_topic_0098680634_p277810146537"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p3778141415318"><a name="zh-cn_topic_0098680634_p3778141415318"></a><a name="zh-cn_topic_0098680634_p3778141415318"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p47781314105312"><a name="zh-cn_topic_0098680634_p47781314105312"></a><a name="zh-cn_topic_0098680634_p47781314105312"></a>云硬盘创建时间。</p>
    <p id="zh-cn_topic_0098680634_p20997172813263"><a name="zh-cn_topic_0098680634_p20997172813263"></a><a name="zh-cn_topic_0098680634_p20997172813263"></a><span id="zh-cn_topic_0098680634_text17996183912613"><a name="zh-cn_topic_0098680634_text17996183912613"></a><a name="zh-cn_topic_0098680634_text17996183912613"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row67781214105315"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p377811416530"><a name="zh-cn_topic_0098680634_p377811416530"></a><a name="zh-cn_topic_0098680634_p377811416530"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p0778131415310"><a name="zh-cn_topic_0098680634_p0778131415310"></a><a name="zh-cn_topic_0098680634_p0778131415310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p47786148539"><a name="zh-cn_topic_0098680634_p47786148539"></a><a name="zh-cn_topic_0098680634_p47786148539"></a>云硬盘类型。</p>
    <div class="p" id="zh-cn_topic_0098680634_zh-cn_topic_0044524833_p112762317377"><a name="zh-cn_topic_0098680634_zh-cn_topic_0044524833_p112762317377"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0044524833_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="zh-cn_topic_0098680634_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="zh-cn_topic_0098680634_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row137786149533"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p14778214185315"><a name="zh-cn_topic_0098680634_p14778214185315"></a><a name="zh-cn_topic_0098680634_p14778214185315"></a>os-vol-tenant-attr:tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p19778514175310"><a name="zh-cn_topic_0098680634_p19778514175310"></a><a name="zh-cn_topic_0098680634_p19778514175310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1677871415318"><a name="zh-cn_topic_0098680634_p1677871415318"></a><a name="zh-cn_topic_0098680634_p1677871415318"></a>云硬盘所属的租户ID。<span id="zh-cn_topic_0098680634_text19941457165313"><a name="zh-cn_topic_0098680634_text19941457165313"></a><a name="zh-cn_topic_0098680634_text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row18778181445315"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p12778114205320"><a name="zh-cn_topic_0098680634_p12778114205320"></a><a name="zh-cn_topic_0098680634_p12778114205320"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p18778141414532"><a name="zh-cn_topic_0098680634_p18778141414532"></a><a name="zh-cn_topic_0098680634_p18778141414532"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p2778614165317"><a name="zh-cn_topic_0098680634_p2778614165317"></a><a name="zh-cn_topic_0098680634_p2778614165317"></a>云硬盘大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row19778191410534"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p6778101415532"><a name="zh-cn_topic_0098680634_p6778101415532"></a><a name="zh-cn_topic_0098680634_p6778101415532"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p17788145537"><a name="zh-cn_topic_0098680634_p17788145537"></a><a name="zh-cn_topic_0098680634_p17788145537"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1778814165312"><a name="zh-cn_topic_0098680634_p1778814165312"></a><a name="zh-cn_topic_0098680634_p1778814165312"></a>云硬盘的元数据，请参见<a href="#zh-cn_topic_0098680634_li29114110314">•metadata参数说明</a>。</p>
    <p id="zh-cn_topic_0098680634_p87781014105314"><a name="zh-cn_topic_0098680634_p87781014105314"></a><a name="zh-cn_topic_0098680634_p87781014105314"></a>如果元数据中不包含hw:passthrough字段，云硬盘默认为VBD类型。</p>
    <p id="zh-cn_topic_0098680634_p137786148534"><a name="zh-cn_topic_0098680634_p137786148534"></a><a name="zh-cn_topic_0098680634_p137786148534"></a>如果元数据中不包含__system__encrypted字段，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row877851418537"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p17778214105317"><a name="zh-cn_topic_0098680634_p17778214105317"></a><a name="zh-cn_topic_0098680634_p17778214105317"></a>os-vol-mig-status-attr:migstat</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p177891485319"><a name="zh-cn_topic_0098680634_p177891485319"></a><a name="zh-cn_topic_0098680634_p177891485319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p978016142531"><a name="zh-cn_topic_0098680634_p978016142531"></a><a name="zh-cn_topic_0098680634_p978016142531"></a><span id="zh-cn_topic_0098680634_text203605127103"><a name="zh-cn_topic_0098680634_text203605127103"></a><a name="zh-cn_topic_0098680634_text203605127103"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1278081415531"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p17780101425317"><a name="zh-cn_topic_0098680634_p17780101425317"></a><a name="zh-cn_topic_0098680634_p17780101425317"></a>os-vol-mig-status-attr:name_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p47801514165310"><a name="zh-cn_topic_0098680634_p47801514165310"></a><a name="zh-cn_topic_0098680634_p47801514165310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p278041410539"><a name="zh-cn_topic_0098680634_p278041410539"></a><a name="zh-cn_topic_0098680634_p278041410539"></a><span id="zh-cn_topic_0098680634_text4617175712110"><a name="zh-cn_topic_0098680634_text4617175712110"></a><a name="zh-cn_topic_0098680634_text4617175712110"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row7780171418539"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p978017142534"><a name="zh-cn_topic_0098680634_p978017142534"></a><a name="zh-cn_topic_0098680634_p978017142534"></a>os-volume-replication:extended_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p12780191455320"><a name="zh-cn_topic_0098680634_p12780191455320"></a><a name="zh-cn_topic_0098680634_p12780191455320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p278051495317"><a name="zh-cn_topic_0098680634_p278051495317"></a><a name="zh-cn_topic_0098680634_p278051495317"></a><span id="zh-cn_topic_0098680634_text379518478151"><a name="zh-cn_topic_0098680634_text379518478151"></a><a name="zh-cn_topic_0098680634_text379518478151"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row15780614195318"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p47452553185118"><a name="zh-cn_topic_0098680634_p47452553185118"></a><a name="zh-cn_topic_0098680634_p47452553185118"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p18451581185118"><a name="zh-cn_topic_0098680634_p18451581185118"></a><a name="zh-cn_topic_0098680634_p18451581185118"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p27951625185124"><a name="zh-cn_topic_0098680634_p27951625185124"></a><a name="zh-cn_topic_0098680634_p27951625185124"></a><span id="zh-cn_topic_0098680634_text141191141115618"><a name="zh-cn_topic_0098680634_text141191141115618"></a><a name="zh-cn_topic_0098680634_text141191141115618"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row778012145537"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p47806145531"><a name="zh-cn_topic_0098680634_p47806145531"></a><a name="zh-cn_topic_0098680634_p47806145531"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p378051485319"><a name="zh-cn_topic_0098680634_p378051485319"></a><a name="zh-cn_topic_0098680634_p378051485319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1478011145538"><a name="zh-cn_topic_0098680634_p1478011145538"></a><a name="zh-cn_topic_0098680634_p1478011145538"></a><span id="zh-cn_topic_0098680634_text6498181171119"><a name="zh-cn_topic_0098680634_text6498181171119"></a><a name="zh-cn_topic_0098680634_text6498181171119"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row127801014115315"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1780101435315"><a name="zh-cn_topic_0098680634_p1780101435315"></a><a name="zh-cn_topic_0098680634_p1780101435315"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p147803142534"><a name="zh-cn_topic_0098680634_p147803142534"></a><a name="zh-cn_topic_0098680634_p147803142534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1780314115312"><a name="zh-cn_topic_0098680634_p1780314115312"></a><a name="zh-cn_topic_0098680634_p1780314115312"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row478012147531"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p207801914195310"><a name="zh-cn_topic_0098680634_p207801914195310"></a><a name="zh-cn_topic_0098680634_p207801914195310"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p57802014195314"><a name="zh-cn_topic_0098680634_p57802014195314"></a><a name="zh-cn_topic_0098680634_p57802014195314"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p478011417532"><a name="zh-cn_topic_0098680634_p478011417532"></a><a name="zh-cn_topic_0098680634_p478011417532"></a><span id="zh-cn_topic_0098680634_text13343838181111"><a name="zh-cn_topic_0098680634_text13343838181111"></a><a name="zh-cn_topic_0098680634_text13343838181111"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row5780814175319"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p117801414155319"><a name="zh-cn_topic_0098680634_p117801414155319"></a><a name="zh-cn_topic_0098680634_p117801414155319"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p18780121416536"><a name="zh-cn_topic_0098680634_p18780121416536"></a><a name="zh-cn_topic_0098680634_p18780121416536"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p8780414125315"><a name="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p8780414125315"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p8780414125315"></a>是否为启动云硬盘。<a name="zh-cn_topic_0098680634_ul185931714111"></a><a name="zh-cn_topic_0098680634_ul185931714111"></a><ul id="zh-cn_topic_0098680634_ul185931714111"><li>true：表示为启动云硬盘。</li><li>false：表示为非启动云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row18780121455311"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1478018149536"><a name="zh-cn_topic_0098680634_p1478018149536"></a><a name="zh-cn_topic_0098680634_p1478018149536"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1078151416531"><a name="zh-cn_topic_0098680634_p1078151416531"></a><a name="zh-cn_topic_0098680634_p1078151416531"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p178141465319"><a name="zh-cn_topic_0098680634_p178141465319"></a><a name="zh-cn_topic_0098680634_p178141465319"></a>云硬盘更新时间。</p>
    <p id="zh-cn_topic_0098680634_p134522013390"><a name="zh-cn_topic_0098680634_p134522013390"></a><a name="zh-cn_topic_0098680634_p134522013390"></a><span id="zh-cn_topic_0098680634_text10160926103914"><a name="zh-cn_topic_0098680634_text10160926103914"></a><a name="zh-cn_topic_0098680634_text10160926103914"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1578113141536"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1578191419531"><a name="zh-cn_topic_0098680634_p1578191419531"></a><a name="zh-cn_topic_0098680634_p1578191419531"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p378121416538"><a name="zh-cn_topic_0098680634_p378121416538"></a><a name="zh-cn_topic_0098680634_p378121416538"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p17811114125319"><a name="zh-cn_topic_0098680634_p17811114125319"></a><a name="zh-cn_topic_0098680634_p17811114125319"></a>是否为可共享云硬盘。</p>
    <div class="note" id="zh-cn_topic_0098680634_note3800959821323"><a name="zh-cn_topic_0098680634_note3800959821323"></a><a name="zh-cn_topic_0098680634_note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0098680634_p45212589213213"><a name="zh-cn_topic_0098680634_p45212589213213"></a><a name="zh-cn_topic_0098680634_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row157811614145318"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p3781191418536"><a name="zh-cn_topic_0098680634_p3781191418536"></a><a name="zh-cn_topic_0098680634_p3781191418536"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p37812014135310"><a name="zh-cn_topic_0098680634_p37812014135310"></a><a name="zh-cn_topic_0098680634_p37812014135310"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p4781191416535"><a name="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p4781191416535"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0098680634_p4781191416535"></a>是否为共享云硬盘。<a name="zh-cn_topic_0098680634_ul161621719119"></a><a name="zh-cn_topic_0098680634_ul161621719119"></a><ul id="zh-cn_topic_0098680634_ul161621719119"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row11781131475317"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p19781814165316"><a name="zh-cn_topic_0098680634_p19781814165316"></a><a name="zh-cn_topic_0098680634_p19781814165316"></a>volume_image_metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p5781314145311"><a name="zh-cn_topic_0098680634_p5781314145311"></a><a name="zh-cn_topic_0098680634_p5781314145311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p15781414175316"><a name="zh-cn_topic_0098680634_p15781414175316"></a><a name="zh-cn_topic_0098680634_p15781414175316"></a>如果云硬盘是从镜像创建的则会有该字段，否则该字段为空。</p>
    <div class="note" id="zh-cn_topic_0098680634_note410975220289"><a name="zh-cn_topic_0098680634_note410975220289"></a><a name="zh-cn_topic_0098680634_note410975220289"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235147_p16054517146"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235147_p16054517146"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235147_p16054517146"></a>关于“volume_image_metadata”字段的详细说明，具体请参见<a href="https://support.huaweicloud.com/api-ims/zh-cn_topic_0020091566.html" target="_blank" rel="noopener noreferrer">查询镜像详情（OpenStack原生）</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1781131415319"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p47811214165316"><a name="zh-cn_topic_0098680634_p47811214165316"></a><a name="zh-cn_topic_0098680634_p47811214165316"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p107811114125311"><a name="zh-cn_topic_0098680634_p107811114125311"></a><a name="zh-cn_topic_0098680634_p107811114125311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p17781151418539"><a name="zh-cn_topic_0098680634_p17781151418539"></a><a name="zh-cn_topic_0098680634_p17781151418539"></a>服务类型，结果为EVS、DSS、DESS。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row1678151415535"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p12781121410537"><a name="zh-cn_topic_0098680634_p12781121410537"></a><a name="zh-cn_topic_0098680634_p12781121410537"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1278151417534"><a name="zh-cn_topic_0098680634_p1278151417534"></a><a name="zh-cn_topic_0098680634_p1278151417534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p12781111465310"><a name="zh-cn_topic_0098680634_p12781111465310"></a><a name="zh-cn_topic_0098680634_p12781111465310"></a>云硬盘所属的专属存储池ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row16781161411537"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p1178131435314"><a name="zh-cn_topic_0098680634_p1178131435314"></a><a name="zh-cn_topic_0098680634_p1178131435314"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1478161475312"><a name="zh-cn_topic_0098680634_p1478161475312"></a><a name="zh-cn_topic_0098680634_p1478161475312"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p1781171475316"><a name="zh-cn_topic_0098680634_p1781171475316"></a><a name="zh-cn_topic_0098680634_p1781171475316"></a>云硬盘所属的专属存储池的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row13766235174313"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p69881644104318"><a name="zh-cn_topic_0098680634_p69881644104318"></a><a name="zh-cn_topic_0098680634_p69881644104318"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1198854414439"><a name="zh-cn_topic_0098680634_p1198854414439"></a><a name="zh-cn_topic_0098680634_p1198854414439"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p18988144418437"><a name="zh-cn_topic_0098680634_p18988144418437"></a><a name="zh-cn_topic_0098680634_p18988144418437"></a>云硬盘的标签。</p>
    <p id="zh-cn_topic_0098680634_p898894418432"><a name="zh-cn_topic_0098680634_p898894418432"></a><a name="zh-cn_topic_0098680634_p898894418432"></a>如果云硬盘有标签，则会有该字段，否则该字段为空。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row73891538114311"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p149881344124319"><a name="zh-cn_topic_0098680634_p149881344124319"></a><a name="zh-cn_topic_0098680634_p149881344124319"></a>wwn</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p3988174494319"><a name="zh-cn_topic_0098680634_p3988174494319"></a><a name="zh-cn_topic_0098680634_p3988174494319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p6988244114313"><a name="zh-cn_topic_0098680634_p6988244114313"></a><a name="zh-cn_topic_0098680634_p6988244114313"></a>云硬盘挂载时的唯一标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_row86151047729"><td class="cellrowborder" valign="top" width="20.1%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p39941261495"><a name="zh-cn_topic_0098680634_p39941261495"></a><a name="zh-cn_topic_0098680634_p39941261495"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p1499413644915"><a name="zh-cn_topic_0098680634_p1499413644915"></a><a name="zh-cn_topic_0098680634_p1499413644915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p35013964916"><a name="zh-cn_topic_0098680634_p35013964916"></a><a name="zh-cn_topic_0098680634_p35013964916"></a>云硬盘上绑定的企业项目ID。</p>
    <div class="note" id="zh-cn_topic_0098680634_note6417183517"><a name="zh-cn_topic_0098680634_note6417183517"></a><a name="zh-cn_topic_0098680634_note6417183517"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p18336524404"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p18336524404"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0098680634_li1077125119136"></a>links参数说明

    <a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_table24355024185927"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row16225418185927"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p39190461185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p39190461185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p39190461185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20310744185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20310744185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20310744185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p47699944185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p47699944185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p47699944185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row38490285185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p30705403185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p30705403185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p30705403185927"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p4109689185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p4109689185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p4109689185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p53015590185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p53015590185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p53015590185927"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row7378265185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p60768596185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p60768596185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p60768596185927"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23309219185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23309219185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23309219185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p57795935185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p57795935185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p57795935185927"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0098680634_li12430153610291"></a>attachments参数说明

    <a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_table6503386185927"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row1296819185927"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p37933504185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p37933504185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p37933504185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p52714965185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p52714965185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p52714965185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p50913593185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p50913593185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p50913593185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row30360408185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p43274016185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p43274016185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p43274016185927"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p15534392185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p15534392185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p15534392185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p49891705185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p49891705185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p49891705185927"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row49550172185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p54141023185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p54141023185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p54141023185927"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23346722185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23346722185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p23346722185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p35416329185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p35416329185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p35416329185927"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row35650386185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p2000176185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p2000176185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p2000176185927"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p27796542185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p27796542185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p27796542185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38329099185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38329099185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38329099185927"></a>挂载的时间信息。</p>
    <p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p3414132514312"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p3414132514312"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p3414132514312"></a><span id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_text7299269449"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_text7299269449"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_text7299269449"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row9417574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p24626033185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p24626033185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p24626033185927"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48551632185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48551632185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48551632185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48591276185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48591276185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48591276185927"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row34668301185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p56668991185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p56668991185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p56668991185927"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p26785545185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p26785545185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p26785545185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48959624185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48959624185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p48959624185927"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row41070280185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38358373185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38358373185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p38358373185927"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20020490185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20020490185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p20020490185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p22392462185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p22392462185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p22392462185927"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_row205574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p16651565185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p16651565185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p16651565185927"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p6599487185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p6599487185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p6599487185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p14021450185927"><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p14021450185927"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0058762429_p14021450185927"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0098680634_li29114110314"></a>metadata参数说明

    <a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_table3430728295554"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p8809200174410"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p8809200174410"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p168135017449"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p168135017449"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1282213034412"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1282213034412"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1562408795622"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1562408795622"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p5759155095622"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p5759155095622"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p177192813501"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p177192813501"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p177192813501"></a>metadata中的表示加密功能的字段。<a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul141951225145011"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul141951225145011"></a><ul id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p241272995622"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p241272995622"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p6121338895622"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p6121338895622"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p4159804295622"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p4159804295622"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1478896104915"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1478896104915"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p52681767104915"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p52681767104915"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p17177177145116"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p17177177145116"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul14462208141855"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul14462208141855"></a><ul id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p3500156018292"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p3500156018292"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1655411118292"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1655411118292"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p47931946183150"><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p47931946183150"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0102756196_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0098680634_li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0098680634_zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "count": 1, 
        "volumes": [
            {
                "attachments": [ ], 
                "availability_zone": "az-dc-1", 
                "bootable": "false", 
                "consistencygroup_id": null, 
                "created_at": "2016-05-25T02:42:10.856332", 
                "description": null, 
                "encrypted": false, 
                "id": "b104b8db-170d-441b-897a-3c8ba9c5a214", 
                "links": [
                    {
                        "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                        "rel": "bookmark"
                    }
                ], 
                "metadata": {}, 
                "name": "zjb_u25_test", 
                "os-vol-host-attr:host": "pod01.xxx#SATA", 
                "volume_image_metadata": { }, 
                "os-vol-mig-status-attr:migstat": null, 
                "os-vol-mig-status-attr:name_id": null, 
                "os-vol-tenant-attr:tenant_id": "dd14c6ac581f40059e27f5320b60bf2f", 
                "os-volume-replication:extended_status": null, 
                "replication_status": "disabled", 
                "multiattach": false, 
                "size": 1, 
                "snapshot_id": null, 
                "source_volid": null, 
                "status": "available", 
                "updated_at": "2016-05-25T02:42:22.341984", 
                "user_id": "b0524e8342084ef5b74f158f78fc3049", 
                "volume_type": "SATA", 
                "service_type": "EVS", 
                "dedicated_storage_id": null, 
                "dedicated_storage_name": null, 
                "wwn": " 688860300000d136fa16f48f05992360"
            }
        ], 
        "volumes_links": [
            {
                "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/detail?limit=1&marker=b104b8db-170d-441b-897a-3c8ba9c5a214", 
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


## 状态码<a name="section56982329"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

