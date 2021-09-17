# 创建云硬盘<a name="evs_04_2065"></a>

## 功能介绍<a name="section60214390"></a>

创建云硬盘。

## URI<a name="section5058598"></a>

-   URI格式

    POST /v2/\{project\_id\}/volumes

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


## 请求消息<a name="section45527389"></a>

-   请求参数

    <a name="table14875192916817"></a>
    <table><thead align="left"><tr id="row787616296812"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="p16876529689"><a name="p16876529689"></a><a name="p16876529689"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="p787612917814"><a name="p787612917814"></a><a name="p787612917814"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p1876122910813"><a name="p1876122910813"></a><a name="p1876122910813"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p1387612912813"><a name="p1387612912813"></a><a name="p1387612912813"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row178767291181"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p6877132916817"><a name="p6877132916817"></a><a name="p6877132916817"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="evs_04_2010_p159017261855"><a name="evs_04_2010_p159017261855"></a><a name="evs_04_2010_p159017261855"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p38777298820"><a name="p38777298820"></a><a name="p38777298820"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p138771229785"><a name="p138771229785"></a><a name="p138771229785"></a>待创建的云硬盘信息，请参见<a href="#li10966323">•volume参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row8340105741820"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p10998181615194"><a name="p10998181615194"></a><a name="p10998181615194"></a>OS-SCH-HNT:scheduler_hints</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p599918163190"><a name="p599918163190"></a><a name="p599918163190"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p59991816161911"><a name="p59991816161911"></a><a name="p59991816161911"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p699951661910"><a name="p699951661910"></a><a name="p699951661910"></a>调度参数，当前支持dedicated_storage_id字段，表明将云硬盘创建在DSS存储池中。</p>
    <p id="p399931613199"><a name="p399931613199"></a><a name="p399931613199"></a>更多详细信息请参见<a href="https://support.huaweicloud.com/api-dss/dss_02_1001.html" target="_blank" rel="noopener noreferrer">获取单个专属分布式存储池详情</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li10966323"></a>volume参数说明

    <a name="table31588048"></a>
    <table><thead align="left"><tr id="row57330849"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="p13287175"><a name="p13287175"></a><a name="p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="p2519427"><a name="p2519427"></a><a name="p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p2747002"><a name="p2747002"></a><a name="p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p21180630"><a name="p21180630"></a><a name="p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19750463"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p56283646"><a name="p56283646"></a><a name="p56283646"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p62681466"><a name="p62681466"></a><a name="p62681466"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p44033946"><a name="p44033946"></a><a name="p44033946"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p2830512315431"><a name="p2830512315431"></a><a name="p2830512315431"></a>指定要创建云硬盘的所属AZ，若指定的AZ不存在，则创建云硬盘失败。</p>
    <div class="note" id="note18354235112810"><a name="note18354235112810"></a><a name="note18354235112810"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p143265317104"><a name="p143265317104"></a><a name="p143265317104"></a>获取AZ的方法：请参考<a href="查询所有的可用分区信息-Cinder-v3.md">查询所有的可用分区信息</a>获取。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row38837194143627"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p56611368143638"><a name="p56611368143638"></a><a name="p56611368143638"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p22118134143638"><a name="p22118134143638"></a><a name="p22118134143638"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p46738440143638"><a name="p46738440143638"></a><a name="p46738440143638"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p27717319143638"><a name="p27717319143638"></a><a name="p27717319143638"></a>源云硬盘ID，指定该参数表示创建云硬盘方式为从源云硬盘克隆。当前云硬盘服务不支持该功能。</p>
    </td>
    </tr>
    <tr id="row22709757"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p27551015"><a name="p27551015"></a><a name="p27551015"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p17039762"><a name="p17039762"></a><a name="p17039762"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p38043494"><a name="p38043494"></a><a name="p38043494"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p5711105614375"><a name="p5711105614375"></a><a name="p5711105614375"></a>云硬盘的描述。<span id="text246920431523"><a name="text246920431523"></a><a name="text246920431523"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row28636870143814"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p42660241143822"><a name="p42660241143822"></a><a name="p42660241143822"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p32927512143822"><a name="p32927512143822"></a><a name="p32927512143822"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p49882844143822"><a name="p49882844143822"></a><a name="p49882844143822"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p13978564143822"><a name="p13978564143822"></a><a name="p13978564143822"></a>快照ID，指定该参数表示创建云硬盘方式为从快照创建。</p>
    <div class="note" id="note13293123112911"><a name="note13293123112911"></a><a name="note13293123112911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1220354818121"><a name="p1220354818121"></a><a name="p1220354818121"></a>获取快照ID的方法：请参见<a href="查询云硬盘快照详细信息列表-Cinder-v3.md">查询云硬盘快照详细信息列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row35520574142458"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p55945721142836"><a name="p55945721142836"></a><a name="p55945721142836"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p35309578142836"><a name="p35309578142836"></a><a name="p35309578142836"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p41503608142836"><a name="p41503608142836"></a><a name="p41503608142836"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><div class="p" id="evs_04_2013_p27784979"><a name="evs_04_2013_p27784979"></a><a name="evs_04_2013_p27784979"></a>云硬盘大小，单位为GB，其限制如下：<a name="evs_04_2013_ul24506304547"></a><a name="evs_04_2013_ul24506304547"></a><ul id="evs_04_2013_ul24506304547"><li>系统盘：1GB-1024GB</li><li>数据盘：10GB-32768GB</li></ul>
    </div>
    <p id="evs_04_2013_p1869819398426"><a name="evs_04_2013_p1869819398426"></a><a name="evs_04_2013_p1869819398426"></a>创建空白云硬盘，size为必选，请在范围内根据需求自定义。</p>
    <p id="evs_04_2013_p433134181712"><a name="evs_04_2013_p433134181712"></a><a name="evs_04_2013_p433134181712"></a>从快照创建云硬盘时，size为必选，且云硬盘大小不能小于快照大小。</p>
    <p id="evs_04_2013_p108486266429"><a name="evs_04_2013_p108486266429"></a><a name="evs_04_2013_p108486266429"></a>从镜像创建云硬盘时，size为必选，且云硬盘大小不小于镜像属性中min_disk要求的最小云硬盘容量。</p>
    </td>
    </tr>
    <tr id="row729385014252"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p29547213143016"><a name="p29547213143016"></a><a name="p29547213143016"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p44514090143016"><a name="p44514090143016"></a><a name="p44514090143016"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p48871527143016"><a name="p48871527143016"></a><a name="p48871527143016"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p44011641143911"><a name="p44011641143911"></a><a name="p44011641143911"></a>云硬盘名称。<span id="text24730431420"><a name="text24730431420"></a><a name="text24730431420"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row4663112514255"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p4059158214322"><a name="p4059158214322"></a><a name="p4059158214322"></a>imageRef</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p6669267314322"><a name="p6669267314322"></a><a name="p6669267314322"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p3339747014322"><a name="p3339747014322"></a><a name="p3339747014322"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p2084053914322"><a name="p2084053914322"></a><a name="p2084053914322"></a>镜像ID，指定该参数表示创建云硬盘方式为从镜像创建。</p>
    <div class="note" id="note13789049151930"><a name="note13789049151930"></a><a name="note13789049151930"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p56992577151930"><a name="p56992577151930"></a><a name="p56992577151930"></a>不支持通过BMS的镜像创建BMS系统盘。</p>
    <p id="p9572163215333"><a name="p9572163215333"></a><a name="p9572163215333"></a>获取镜像ID的方法：请参见<a href="https://support.huaweicloud.com/api-ims/ims_03_0602.html" target="_blank" rel="noopener noreferrer">查询镜像列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row1270246214258"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p31198636143253"><a name="p31198636143253"></a><a name="p31198636143253"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p44061594143253"><a name="p44061594143253"></a><a name="p44061594143253"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p12219401143253"><a name="p12219401143253"></a><a name="p12219401143253"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p14380476104717"><a name="p14380476104717"></a><a name="p14380476104717"></a>云硬盘类型。</p>
    <div class="p" id="p147871251104619"><a name="p147871251104619"></a><a name="p147871251104619"></a>目前支持“SSD”，“GPSSD”和“SAS”三种。<a name="evs_04_2003_ul169651733203316"></a><a name="evs_04_2003_ul169651733203316"></a><ul id="evs_04_2003_ul169651733203316"><li>“SSD”为超高IO云硬盘</li><li>“GPSSD”为通用型SSD云硬盘</li><li>“SAS”为高IO云硬盘</li></ul>
    </div>
    <p id="p62741351184614"><a name="p62741351184614"></a><a name="p62741351184614"></a>当指定的云硬盘类型在avaliability_zone内不存在时，则创建云硬盘失败。</p>
    <div class="note" id="note21808274104217"><a name="note21808274104217"></a><a name="note21808274104217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul5307015718498"></a><a name="ul5307015718498"></a><ul id="ul5307015718498"><li><span id="text7492111913438"><a name="text7492111913438"></a><a name="text7492111913438"></a>从快照创建云硬盘时，volume_type字段必须和快照源云硬盘保持一致。</span></li><li>了解不同磁盘类型的详细信息，请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0044524691.html" target="_blank" rel="noopener noreferrer">磁盘类型及性能介绍</a>。</li></ul>
    </div></div>
    </td>
    </tr>
    <tr id="row5295776142511"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p1235117143943"><a name="p1235117143943"></a><a name="p1235117143943"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p32935684143943"><a name="p32935684143943"></a><a name="p32935684143943"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p50544710143943"><a name="p50544710143943"></a><a name="p50544710143943"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p480861143943"><a name="p480861143943"></a><a name="p480861143943"></a>云硬盘的metadata数据，<span id="text648010431128"><a name="text648010431128"></a><a name="text648010431128"></a>metadata中的key和value长度不大于255个字节</span>。</p>
    <p id="p618213246557"><a name="p618213246557"></a><a name="p618213246557"></a>“metadata”字段信息说明请参见“metadata字段说明”表格，表格中列举了部分字段，您还可以根据创建磁盘的要求输入其他字段，请参见<a href="#li4145283210319">•metadata参数说明</a>。</p>
    <div class="note" id="note660019322131"><a name="note660019322131"></a><a name="note660019322131"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p1600173216137"><a name="evs_04_2013_p1600173216137"></a><a name="evs_04_2013_p1600173216137"></a>metadata里面不能有value为null的键值对。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row24630747142515"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p38669085144023"><a name="p38669085144023"></a><a name="p38669085144023"></a>source_replica</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p45188191144023"><a name="p45188191144023"></a><a name="p45188191144023"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p36364878144023"><a name="p36364878144023"></a><a name="p36364878144023"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p59874001144023"><a name="p59874001144023"></a><a name="p59874001144023"></a>该参数表示从磁盘的克隆来创建云硬盘，当前云硬盘服务不支持该功能。</p>
    </td>
    </tr>
    <tr id="row33780455142518"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p56697807144126"><a name="p56697807144126"></a><a name="p56697807144126"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p29119653144126"><a name="p29119653144126"></a><a name="p29119653144126"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p9881663144126"><a name="p9881663144126"></a><a name="p9881663144126"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p62217221144126"><a name="p62217221144126"></a><a name="p62217221144126"></a><span id="text13343838181111"><a name="text13343838181111"></a><a name="text13343838181111"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="row46893009142655"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p16191875144233"><a name="p16191875144233"></a><a name="p16191875144233"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p36473476144233"><a name="p36473476144233"></a><a name="p36473476144233"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p1561611144233"><a name="p1561611144233"></a><a name="p1561611144233"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><div class="p" id="p4531155053519"><a name="p4531155053519"></a><a name="p4531155053519"></a>创建共享云硬盘的信息。默认值为false。<a name="ul202952187368"></a><a name="ul202952187368"></a><ul id="ul202952187368"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    <p id="p96242024104913"><a name="p96242024104913"></a><a name="p96242024104913"></a>请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0032860759.html" target="_blank" rel="noopener noreferrer">共享云硬盘及使用方法</a>了解更多信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >不支持同时使用“source\_volid“、“snapshot\_id“和“imageRef“这三个字段中的任意两个。

-   <a name="li4145283210319"></a>metadata参数说明

    <a name="evs_04_2013_table3430728295554"></a>
    <table><thead align="left"><tr id="evs_04_2013_row4496975195554"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="evs_04_2013_p5979314595726"><a name="evs_04_2013_p5979314595726"></a><a name="evs_04_2013_p5979314595726"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="evs_04_2013_p1140655395726"><a name="evs_04_2013_p1140655395726"></a><a name="evs_04_2013_p1140655395726"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.3"><p id="evs_04_2013_p5151561095726"><a name="evs_04_2013_p5151561095726"></a><a name="evs_04_2013_p5151561095726"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="46%" id="mcps1.1.5.1.4"><p id="evs_04_2013_p1201488395726"><a name="evs_04_2013_p1201488395726"></a><a name="evs_04_2013_p1201488395726"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row456195295554"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p1562408795622"><a name="evs_04_2013_p1562408795622"></a><a name="evs_04_2013_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p5759155095622"><a name="evs_04_2013_p5759155095622"></a><a name="evs_04_2013_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p3440400295622"><a name="evs_04_2013_p3440400295622"></a><a name="evs_04_2013_p3440400295622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p4269864016712"><a name="p4269864016712"></a><a name="p4269864016712"></a>metadata中的表示加密功能的字段，0代表不加密，1代表加密。</p>
    <p id="evs_04_2013_p3526077895622"><a name="evs_04_2013_p3526077895622"></a><a name="evs_04_2013_p3526077895622"></a>该字段不存在时，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="evs_04_2013_row247050109562"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p241272995622"><a name="evs_04_2013_p241272995622"></a><a name="evs_04_2013_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p6121338895622"><a name="evs_04_2013_p6121338895622"></a><a name="evs_04_2013_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p5933737595622"><a name="evs_04_2013_p5933737595622"></a><a name="evs_04_2013_p5933737595622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p4159804295622"><a name="evs_04_2013_p4159804295622"></a><a name="evs_04_2013_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    <div class="note" id="note1483983117491"><a name="note1483983117491"></a><a name="note1483983117491"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p093935613512"><a name="evs_04_2013_p093935613512"></a><a name="evs_04_2013_p093935613512"></a>请参考<a href="https://support.huaweicloud.com/api-dew/ListKeys.html" target="_blank" rel="noopener noreferrer">查询密钥列表</a>，通过HTTPS请求获取密钥ID。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row60499086104915"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p1478896104915"><a name="evs_04_2013_p1478896104915"></a><a name="evs_04_2013_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p52681767104915"><a name="evs_04_2013_p52681767104915"></a><a name="evs_04_2013_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p39364763104915"><a name="evs_04_2013_p39364763104915"></a><a name="evs_04_2013_p39364763104915"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="evs_04_2013_ul14462208141855"></a><a name="evs_04_2013_ul14462208141855"></a><ul id="evs_04_2013_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD (虚拟块存储设备 , Virtual Block Device)类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。<div class="note" id="evs_04_2013_note30831239112110"><a name="evs_04_2013_note30831239112110"></a><a name="evs_04_2013_note30831239112110"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p9045701112110"><a name="evs_04_2013_p9045701112110"></a><a name="evs_04_2013_p9045701112110"></a>当shareable参数值设置为true，不指定hw:passthrough参数值时，创建的云硬盘为VBD类型共享云硬盘。</p>
    </div></div>
    </li></ul>
    </td>
    </tr>
    <tr id="row6091294618292"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p3500156018292"><a name="p3500156018292"></a><a name="p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p1655411118292"><a name="p1655411118292"></a><a name="p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="p6581460618292"><a name="p6581460618292"></a><a name="p6581460618292"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="p47931946183150"><a name="p47931946183150"></a><a name="p47931946183150"></a>从快照创建云硬盘时，如需使用link克隆方式，请指定该字段的值为0。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >以上表格中仅提供了部分“metadata”字段信息说明供您参考，您还可以根据创建磁盘的要求输入其他字段。
    >-   如果是从快照创建云硬盘，则不支持传入“\_\_system\_\_encrypted“和“\_\_system\_\_cmkid“字段，创建出来的云硬盘与快照源云硬盘的加密属性一致。
    >-   如果是从镜像创建云硬盘，则不支持传入“\_\_system\_\_encrypted“和“\_\_system\_\_cmkid“字段，创建出来的云硬盘与镜像的加密属性一致。
    >-   如果是从快照创建云硬盘，则不支持传入“hw:passthrough“字段，创建出来的云硬盘的设备类型与快照源云硬盘保持一致。
    >-   如果是从镜像创建云硬盘，则不支持传入“hw:passthrough“字段，创建出来的云硬盘的设备类型为VBD类型。

-   请求样例

    ```
    {
        "volume": {
            "name": "openapi_vol01", 
            "imageRef": "027cf713-45a6-45f0-ac1b-0ccc57ac12e2", 
            "availability_zone": "az-dc-1", 
            "description": "create for api test", 
            "volume_type": "SATA", 
            "metadata": {
                "volume_owner": "openapi"
            },  
            "multiattach": false, 
            "size": 40
        }, 
        "OS-SCH-HNT:scheduler_hints": {
            "dedicated_storage_id": "eddc1a3e-4145-45be-98d7-bf6f65af9767"
        }
    }
    ```


## 响应消息<a name="section7093323"></a>

-   响应参数

    <a name="table192671691419"></a>
    <table><thead align="left"><tr id="row1626713984113"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="p626716915410"><a name="p626716915410"></a><a name="p626716915410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="p10268199164120"><a name="p10268199164120"></a><a name="p10268199164120"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.1.4.1.3"><p id="p226814984116"><a name="p226814984116"></a><a name="p226814984116"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20268997416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p192684913418"><a name="p192684913418"></a><a name="p192684913418"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p1326816984113"><a name="p1326816984113"></a><a name="p1326816984113"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p1826816912416"><a name="p1826816912416"></a><a name="p1826816912416"></a>创建出来的云硬盘，请参见<a href="#li3451542201439">•volumes参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row197012674215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li3451542201439"></a>volumes参数说明

    <a name="table34701445142557"></a>
    <table><thead align="left"><tr id="row12524911142557"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="p7884856142557"><a name="p7884856142557"></a><a name="p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="p34693598142557"><a name="p34693598142557"></a><a name="p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.1.4.1.3"><p id="p58539486142557"><a name="p58539486142557"></a><a name="p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row444782011610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p18308336144438"><a name="p18308336144438"></a><a name="p18308336144438"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p6580236144438"><a name="p6580236144438"></a><a name="p6580236144438"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p21928856144438"><a name="p21928856144438"></a><a name="p21928856144438"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row44077962142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p14226985144438"><a name="p14226985144438"></a><a name="p14226985144438"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p11535156144438"><a name="p11535156144438"></a><a name="p11535156144438"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p50473003144438"><a name="p50473003144438"></a><a name="p50473003144438"></a>云硬盘URI自描述信息，请参见<a href="#li1043159617124">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row16186817142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p19162411144438"><a name="p19162411144438"></a><a name="p19162411144438"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p8651439144438"><a name="p8651439144438"></a><a name="p8651439144438"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p55103877144438"><a name="p55103877144438"></a><a name="p55103877144438"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="row2987651144410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p39625821144438"><a name="p39625821144438"></a><a name="p39625821144438"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p55574965144438"><a name="p55574965144438"></a><a name="p55574965144438"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p24889213144438"><a name="p24889213144438"></a><a name="p24889213144438"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row45785905142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p24843442144438"><a name="p24843442144438"></a><a name="p24843442144438"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p66161799144438"><a name="p66161799144438"></a><a name="p66161799144438"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p27432950144438"><a name="p27432950144438"></a><a name="p27432950144438"></a>挂载信息，请参见<a href="#li3900093617124">•attachments参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row35247553142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p179170144438"><a name="p179170144438"></a><a name="p179170144438"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p14512814144438"><a name="p14512814144438"></a><a name="p14512814144438"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p58206487144438"><a name="p58206487144438"></a><a name="p58206487144438"></a>云硬盘所属AZ。</p>
    </td>
    </tr>
    <tr id="row27126244142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p19727534144438"><a name="p19727534144438"></a><a name="p19727534144438"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p54426427144438"><a name="p54426427144438"></a><a name="p54426427144438"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2010_p8780414125315"><a name="evs_04_2010_p8780414125315"></a><a name="evs_04_2010_p8780414125315"></a>是否为启动云硬盘。<a name="ul185931714111"></a><a name="ul185931714111"></a><ul id="ul185931714111"><li>true：表示为启动云硬盘。</li><li>false：表示为非启动云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row17610291172344"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p5866739172351"><a name="p5866739172351"></a><a name="p5866739172351"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p5443865172351"><a name="p5443865172351"></a><a name="p5443865172351"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p15286422172351"><a name="p15286422172351"></a><a name="p15286422172351"></a><span id="text115706570229"><a name="text115706570229"></a><a name="text115706570229"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="row49237196142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p28651206144438"><a name="p28651206144438"></a><a name="p28651206144438"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p1296456144535"><a name="p1296456144535"></a><a name="p1296456144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p28821893144438"><a name="p28821893144438"></a><a name="p28821893144438"></a>创建云硬盘的时间。</p>
    <p id="p586613505312"><a name="p586613505312"></a><a name="p586613505312"></a><span id="text28661350936"><a name="text28661350936"></a><a name="text28661350936"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row39017307142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p6085885144438"><a name="p6085885144438"></a><a name="p6085885144438"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p18611115144535"><a name="p18611115144535"></a><a name="p18611115144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p44410693144438"><a name="p44410693144438"></a><a name="p44410693144438"></a>云硬盘描述。</p>
    </td>
    </tr>
    <tr id="row20107664142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p28923171144438"><a name="p28923171144438"></a><a name="p28923171144438"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p22198851144535"><a name="p22198851144535"></a><a name="p22198851144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p9630579144438"><a name="p9630579144438"></a><a name="p9630579144438"></a>云硬盘类型。</p>
    <div class="p" id="p18390159171918"><a name="p18390159171918"></a><a name="p18390159171918"></a>目前支持“SSD”，“GPSSD”和“SAS”三种。<a name="evs_04_2003_ul169651733203316_1"></a><a name="evs_04_2003_ul169651733203316_1"></a><ul id="evs_04_2003_ul169651733203316_1"><li>“SSD”为超高IO云硬盘</li><li>“GPSSD”为通用型SSD云硬盘</li><li>“SAS”为高IO云硬盘</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row12897861142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p41370851144438"><a name="p41370851144438"></a><a name="p41370851144438"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p7354807144535"><a name="p7354807144535"></a><a name="p7354807144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p27786537144438"><a name="p27786537144438"></a><a name="p27786537144438"></a><span id="text6498181171119"><a name="text6498181171119"></a><a name="text6498181171119"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="row45680217142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p56617581144438"><a name="p56617581144438"></a><a name="p56617581144438"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p25180208144535"><a name="p25180208144535"></a><a name="p25180208144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p40860550144438"><a name="p40860550144438"></a><a name="p40860550144438"></a>所属一致性组ID。</p>
    <p id="p1919420431188"><a name="p1919420431188"></a><a name="p1919420431188"></a><span id="text161944439182"><a name="text161944439182"></a><a name="text161944439182"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="row47480567142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p58114746144438"><a name="p58114746144438"></a><a name="p58114746144438"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p47440982144535"><a name="p47440982144535"></a><a name="p47440982144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p52975605144438"><a name="p52975605144438"></a><a name="p52975605144438"></a>源云硬盘ID。</p>
    <p id="p14532184716186"><a name="p14532184716186"></a><a name="p14532184716186"></a><span id="text12532347191815"><a name="text12532347191815"></a><a name="text12532347191815"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="row31517135142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p31619531144438"><a name="p31619531144438"></a><a name="p31619531144438"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p66078031144535"><a name="p66078031144535"></a><a name="p66078031144535"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p57055846144438"><a name="p57055846144438"></a><a name="p57055846144438"></a>快照ID。</p>
    </td>
    </tr>
    <tr id="row15610713142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p53325033144438"><a name="p53325033144438"></a><a name="p53325033144438"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p24360403144438"><a name="p24360403144438"></a><a name="p24360403144438"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p42403730144438"><a name="p42403730144438"></a><a name="p42403730144438"></a>元数据，请参见<a href="#li29114110314">•metadata参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row5657368142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p42241765144438"><a name="p42241765144438"></a><a name="p42241765144438"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p66139813144438"><a name="p66139813144438"></a><a name="p66139813144438"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p17400122144438"><a name="p17400122144438"></a><a name="p17400122144438"></a>云硬盘大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="row39412545144428"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p1113688144438"><a name="p1113688144438"></a><a name="p1113688144438"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p51894643144540"><a name="p51894643144540"></a><a name="p51894643144540"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p26218517352"><a name="p26218517352"></a><a name="p26218517352"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="row25381049144431"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p26680804144438"><a name="p26680804144438"></a><a name="p26680804144438"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p39072645144540"><a name="p39072645144540"></a><a name="p39072645144540"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p42877354144438"><a name="p42877354144438"></a><a name="p42877354144438"></a>云硬盘更新时间。</p>
    <p id="p15772145473814"><a name="p15772145473814"></a><a name="p15772145473814"></a><span id="text151181202390"><a name="text151181202390"></a><a name="text151181202390"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row48384415144425"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p51969649144438"><a name="p51969649144438"></a><a name="p51969649144438"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p5099125121957"><a name="p5099125121957"></a><a name="p5099125121957"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="p15113052144438"><a name="p15113052144438"></a><a name="p15113052144438"></a>是否为可共享云硬盘。</p>
    <div class="note" id="note182866179314"><a name="note182866179314"></a><a name="note182866179314"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p45212589213213"><a name="evs_04_2013_p45212589213213"></a><a name="evs_04_2013_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row42462677142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p11561839144438"><a name="p11561839144438"></a><a name="p11561839144438"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p64093800144438"><a name="p64093800144438"></a><a name="p64093800144438"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2010_p4781191416535"><a name="evs_04_2010_p4781191416535"></a><a name="evs_04_2010_p4781191416535"></a>是否为共享云硬盘。<a name="ul161621719119"></a><a name="ul161621719119"></a><ul id="ul161621719119"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li1043159617124"></a>links参数说明

    <a name="table4005083311851"></a>
    <table><thead align="left"><tr id="row4647546111851"><th class="cellrowborder" valign="top" width="19.27807219278072%" id="mcps1.1.4.1.1"><p id="p641601411851"><a name="p641601411851"></a><a name="p641601411851"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.0975902409759%" id="mcps1.1.4.1.2"><p id="p4993509511851"><a name="p4993509511851"></a><a name="p4993509511851"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.624337566243376%" id="mcps1.1.4.1.3"><p id="p6579322611851"><a name="p6579322611851"></a><a name="p6579322611851"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2765107611851"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p2514470311851"><a name="p2514470311851"></a><a name="p2514470311851"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p2345507511851"><a name="p2345507511851"></a><a name="p2345507511851"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p812224311851"><a name="p812224311851"></a><a name="p812224311851"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="row599132611851"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p1553537811851"><a name="p1553537811851"></a><a name="p1553537811851"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p5040609911851"><a name="p5040609911851"></a><a name="p5040609911851"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p193416911851"><a name="p193416911851"></a><a name="p193416911851"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li3900093617124"></a>attachments参数说明

    <a name="table3471673811913"></a>
    <table><thead align="left"><tr id="row950913211913"><th class="cellrowborder" valign="top" width="19.27807219278072%" id="mcps1.1.4.1.1"><p id="p3204224811913"><a name="p3204224811913"></a><a name="p3204224811913"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.0975902409759%" id="mcps1.1.4.1.2"><p id="p4528532911913"><a name="p4528532911913"></a><a name="p4528532911913"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.624337566243376%" id="mcps1.1.4.1.3"><p id="p2610634411913"><a name="p2610634411913"></a><a name="p2610634411913"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3423911011913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p2190452911913"><a name="p2190452911913"></a><a name="p2190452911913"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p2943640011913"><a name="p2943640011913"></a><a name="p2943640011913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p6002094011913"><a name="p6002094011913"></a><a name="p6002094011913"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="row331754911913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p28604711913"><a name="p28604711913"></a><a name="p28604711913"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p2316983311913"><a name="p2316983311913"></a><a name="p2316983311913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p1570218411913"><a name="p1570218411913"></a><a name="p1570218411913"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="row41611216113819"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p26997962113823"><a name="p26997962113823"></a><a name="p26997962113823"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p39351338113823"><a name="p39351338113823"></a><a name="p39351338113823"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p16333436113823"><a name="p16333436113823"></a><a name="p16333436113823"></a>挂载的时间信息。</p>
    <p id="p103581088395"><a name="p103581088395"></a><a name="p103581088395"></a><span id="text136037162396"><a name="text136037162396"></a><a name="text136037162396"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row710192811913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p3838529111913"><a name="p3838529111913"></a><a name="p3838529111913"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p2220087511913"><a name="p2220087511913"></a><a name="p2220087511913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p3370764811913"><a name="p3370764811913"></a><a name="p3370764811913"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="row3493337611913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p1103121411913"><a name="p1103121411913"></a><a name="p1103121411913"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p2111318111913"><a name="p2111318111913"></a><a name="p2111318111913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p1089110111913"><a name="p1089110111913"></a><a name="p1089110111913"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row3091104611913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p2076682611913"><a name="p2076682611913"></a><a name="p2076682611913"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p439134611913"><a name="p439134611913"></a><a name="p439134611913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p2192276811913"><a name="p2192276811913"></a><a name="p2192276811913"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="row6308718811913"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="p978858311913"><a name="p978858311913"></a><a name="p978858311913"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="p5467773011913"><a name="p5467773011913"></a><a name="p5467773011913"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p4371205011913"><a name="p4371205011913"></a><a name="p4371205011913"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li29114110314"></a>metadata参数说明

    <a name="evs_04_3004_table3430728295554"></a>
    <table><thead align="left"><tr id="evs_04_3004_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_3004_p8809200174410"><a name="evs_04_3004_p8809200174410"></a><a name="evs_04_3004_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_3004_p168135017449"><a name="evs_04_3004_p168135017449"></a><a name="evs_04_3004_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_3004_p1282213034412"><a name="evs_04_3004_p1282213034412"></a><a name="evs_04_3004_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_3004_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p1562408795622"><a name="evs_04_3004_p1562408795622"></a><a name="evs_04_3004_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p5759155095622"><a name="evs_04_3004_p5759155095622"></a><a name="evs_04_3004_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_3004_p177192813501"><a name="evs_04_3004_p177192813501"></a><a name="evs_04_3004_p177192813501"></a>metadata中的表示加密功能的字段。<a name="evs_04_3004_ul141951225145011"></a><a name="evs_04_3004_ul141951225145011"></a><ul id="evs_04_3004_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_3004_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p241272995622"><a name="evs_04_3004_p241272995622"></a><a name="evs_04_3004_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p6121338895622"><a name="evs_04_3004_p6121338895622"></a><a name="evs_04_3004_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_3004_p4159804295622"><a name="evs_04_3004_p4159804295622"></a><a name="evs_04_3004_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="evs_04_3004_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p1478896104915"><a name="evs_04_3004_p1478896104915"></a><a name="evs_04_3004_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p52681767104915"><a name="evs_04_3004_p52681767104915"></a><a name="evs_04_3004_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_3004_p17177177145116"><a name="evs_04_3004_p17177177145116"></a><a name="evs_04_3004_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="evs_04_3004_ul14462208141855"></a><a name="evs_04_3004_ul14462208141855"></a><ul id="evs_04_3004_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_3004_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p3500156018292"><a name="evs_04_3004_p3500156018292"></a><a name="evs_04_3004_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p1655411118292"><a name="evs_04_3004_p1655411118292"></a><a name="evs_04_3004_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_3004_p47931946183150"><a name="evs_04_3004_p47931946183150"></a><a name="evs_04_3004_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
    </td>
    </tr>
    <tr id="evs_04_3004_row124351901058"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p843510018510"><a name="evs_04_3004_p843510018510"></a><a name="evs_04_3004_p843510018510"></a>orderID</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p1943520259"><a name="evs_04_3004_p1943520259"></a><a name="evs_04_3004_p1943520259"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_3004_p174351007511"><a name="evs_04_3004_p174351007511"></a><a name="evs_04_3004_p174351007511"></a>metadata中的表示云硬盘计费类型的字段。</p>
    <p id="evs_04_3004_p121347762"><a name="evs_04_3004_p121347762"></a><a name="evs_04_3004_p121347762"></a>当该字段有值时，表示该云硬盘的计费类型为包周期计费，否则计费类型为按需计费。</p>
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
    <p id="evs_04_2013_p54787218103019"><a name="evs_04_2013_p54787218103019"></a><a name="evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "volume": {
            "attachments": [ ], 
            "availability_zone": "az-dc-1", 
            "bootable": "false", 
            "consistencygroup_id": null, 
            "created_at": "2016-05-25T02:38:40.392463", 
            "description": "create for api test", 
            "encrypted": false, 
            "id": "8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
            "links": [
                {
                    "href": "https://volume.localdomain.com:8776/v2/5dd0b0056f3d47b6ab4121667d35621a/volumes/8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
                    "rel": "self"
                }, 
                {
                    "href": "https://volume.localdomain.com:8776/5dd0b0056f3d47b6ab4121667d35621a/volumes/8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
                    "rel": "bookmark"
                }
            ], 
            "metadata": {
                "volume_owner": "openapi"
            }, 
            "name": "openapi_vol01", 
            "replication_status": "disabled", 
            "multiattach": false, 
            "size": 40, 
            "snapshot_id": null, 
            "source_volid": null, 
            "status": "creating", 
            "updated_at": null, 
            "user_id": "39f6696ae23740708d0f358a253c2637", 
            "volume_type": "SATA"
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错为：

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

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

