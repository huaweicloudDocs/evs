# 创建云硬盘<a name="ZH-CN_TOPIC_0102534367"></a>

## 功能介绍<a name="section60214390"></a>

创建云硬盘。

## URI<a name="section5058598"></a>

-   URI格式

    POST /v3/\{project\_id\}/volumes

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
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section45527389"></a>

-   请求参数

    <a name="zh-cn_topic_0058762427_table31588048"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762427_row57330849"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058762427_p13287175"><a name="zh-cn_topic_0058762427_p13287175"></a><a name="zh-cn_topic_0058762427_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058762427_p2519427"><a name="zh-cn_topic_0058762427_p2519427"></a><a name="zh-cn_topic_0058762427_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058762427_p2747002"><a name="zh-cn_topic_0058762427_p2747002"></a><a name="zh-cn_topic_0058762427_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058762427_p21180630"><a name="zh-cn_topic_0058762427_p21180630"></a><a name="zh-cn_topic_0058762427_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762427_row1445032621467"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p121240421469"><a name="zh-cn_topic_0058762427_p121240421469"></a><a name="zh-cn_topic_0058762427_p121240421469"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p3109590421469"><a name="zh-cn_topic_0058762427_p3109590421469"></a><a name="zh-cn_topic_0058762427_p3109590421469"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p3574029221469"><a name="zh-cn_topic_0058762427_p3574029221469"></a><a name="zh-cn_topic_0058762427_p3574029221469"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p928256921469"><a name="zh-cn_topic_0058762427_p928256921469"></a><a name="zh-cn_topic_0058762427_p928256921469"></a>待创建的云硬盘信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row19750463"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p56283646"><a name="zh-cn_topic_0058762427_p56283646"></a><a name="zh-cn_topic_0058762427_p56283646"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p62681466"><a name="zh-cn_topic_0058762427_p62681466"></a><a name="zh-cn_topic_0058762427_p62681466"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p44033946"><a name="zh-cn_topic_0058762427_p44033946"></a><a name="zh-cn_topic_0058762427_p44033946"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p2830512315431"><a name="zh-cn_topic_0058762427_p2830512315431"></a><a name="zh-cn_topic_0058762427_p2830512315431"></a>指定要创建云硬盘的所属AZ，若指定的AZ不存在，则创建云硬盘失败。</p>
    <div class="note" id="zh-cn_topic_0058762427_note18354235112810"><a name="zh-cn_topic_0058762427_note18354235112810"></a><a name="zh-cn_topic_0058762427_note18354235112810"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_p14110155594414"><a name="zh-cn_topic_0058762427_p14110155594414"></a><a name="zh-cn_topic_0058762427_p14110155594414"></a>获取AZ的方法：请参考<a href="查询所有的可用分区信息.md">查询所有的可用分区信息</a>获取。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row38837194143627"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p56611368143638"><a name="zh-cn_topic_0058762427_p56611368143638"></a><a name="zh-cn_topic_0058762427_p56611368143638"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p22118134143638"><a name="zh-cn_topic_0058762427_p22118134143638"></a><a name="zh-cn_topic_0058762427_p22118134143638"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p46738440143638"><a name="zh-cn_topic_0058762427_p46738440143638"></a><a name="zh-cn_topic_0058762427_p46738440143638"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p27717319143638"><a name="zh-cn_topic_0058762427_p27717319143638"></a><a name="zh-cn_topic_0058762427_p27717319143638"></a>源云硬盘ID，指定该参数表示创建云硬盘方式为从源云硬盘克隆。当前云硬盘服务不支持该功能。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row22709757"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p27551015"><a name="zh-cn_topic_0058762427_p27551015"></a><a name="zh-cn_topic_0058762427_p27551015"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p17039762"><a name="zh-cn_topic_0058762427_p17039762"></a><a name="zh-cn_topic_0058762427_p17039762"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p38043494"><a name="zh-cn_topic_0058762427_p38043494"></a><a name="zh-cn_topic_0058762427_p38043494"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p5711105614375"><a name="zh-cn_topic_0058762427_p5711105614375"></a><a name="zh-cn_topic_0058762427_p5711105614375"></a>云硬盘的描述。<span id="zh-cn_topic_0058762427_text246920431523"><a name="zh-cn_topic_0058762427_text246920431523"></a><a name="zh-cn_topic_0058762427_text246920431523"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row28636870143814"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p42660241143822"><a name="zh-cn_topic_0058762427_p42660241143822"></a><a name="zh-cn_topic_0058762427_p42660241143822"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p32927512143822"><a name="zh-cn_topic_0058762427_p32927512143822"></a><a name="zh-cn_topic_0058762427_p32927512143822"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p49882844143822"><a name="zh-cn_topic_0058762427_p49882844143822"></a><a name="zh-cn_topic_0058762427_p49882844143822"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p13978564143822"><a name="zh-cn_topic_0058762427_p13978564143822"></a><a name="zh-cn_topic_0058762427_p13978564143822"></a>快照ID，指定该参数表示创建云硬盘方式为从快照创建。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row35520574142458"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p55945721142836"><a name="zh-cn_topic_0058762427_p55945721142836"></a><a name="zh-cn_topic_0058762427_p55945721142836"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p35309578142836"><a name="zh-cn_topic_0058762427_p35309578142836"></a><a name="zh-cn_topic_0058762427_p35309578142836"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p41503608142836"><a name="zh-cn_topic_0058762427_p41503608142836"></a><a name="zh-cn_topic_0058762427_p41503608142836"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p14164893102658"><a name="zh-cn_topic_0058762427_p14164893102658"></a><a name="zh-cn_topic_0058762427_p14164893102658"></a>云硬盘大小，单位为GB。</p>
    <a name="zh-cn_topic_0058762427_ul4671484110271"></a><a name="zh-cn_topic_0058762427_ul4671484110271"></a><ul id="zh-cn_topic_0058762427_ul4671484110271"><li>从镜像创建云硬盘时，云硬盘大小不能小于镜像大小。</li><li>从快照创建云硬盘时，云硬盘大小不能小于快照大小。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row729385014252"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p29547213143016"><a name="zh-cn_topic_0058762427_p29547213143016"></a><a name="zh-cn_topic_0058762427_p29547213143016"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p44514090143016"><a name="zh-cn_topic_0058762427_p44514090143016"></a><a name="zh-cn_topic_0058762427_p44514090143016"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p48871527143016"><a name="zh-cn_topic_0058762427_p48871527143016"></a><a name="zh-cn_topic_0058762427_p48871527143016"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p44011641143911"><a name="zh-cn_topic_0058762427_p44011641143911"></a><a name="zh-cn_topic_0058762427_p44011641143911"></a>云硬盘名称。<span id="zh-cn_topic_0058762427_text24730431420"><a name="zh-cn_topic_0058762427_text24730431420"></a><a name="zh-cn_topic_0058762427_text24730431420"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row4663112514255"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p4059158214322"><a name="zh-cn_topic_0058762427_p4059158214322"></a><a name="zh-cn_topic_0058762427_p4059158214322"></a>imageRef</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p6669267314322"><a name="zh-cn_topic_0058762427_p6669267314322"></a><a name="zh-cn_topic_0058762427_p6669267314322"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p3339747014322"><a name="zh-cn_topic_0058762427_p3339747014322"></a><a name="zh-cn_topic_0058762427_p3339747014322"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p2084053914322"><a name="zh-cn_topic_0058762427_p2084053914322"></a><a name="zh-cn_topic_0058762427_p2084053914322"></a>镜像ID，指定该参数表示创建云硬盘方式为从镜像创建。</p>
    <div class="note" id="zh-cn_topic_0058762427_note13789049151930"><a name="zh-cn_topic_0058762427_note13789049151930"></a><a name="zh-cn_topic_0058762427_note13789049151930"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_p56992577151930"><a name="zh-cn_topic_0058762427_p56992577151930"></a><a name="zh-cn_topic_0058762427_p56992577151930"></a>不支持通过BMS的镜像创建BMS系统盘。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row1270246214258"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p31198636143253"><a name="zh-cn_topic_0058762427_p31198636143253"></a><a name="zh-cn_topic_0058762427_p31198636143253"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p44061594143253"><a name="zh-cn_topic_0058762427_p44061594143253"></a><a name="zh-cn_topic_0058762427_p44061594143253"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p12219401143253"><a name="zh-cn_topic_0058762427_p12219401143253"></a><a name="zh-cn_topic_0058762427_p12219401143253"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p14380476104717"><a name="zh-cn_topic_0058762427_p14380476104717"></a><a name="zh-cn_topic_0058762427_p14380476104717"></a>云硬盘类型。</p>
    <div class="p" id="zh-cn_topic_0058762427_p18356539113258"><a name="zh-cn_topic_0058762427_p18356539113258"></a><a name="zh-cn_topic_0058762427_p18356539113258"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="zh-cn_topic_0058762427_ul4378238815463"></a><a name="zh-cn_topic_0058762427_ul4378238815463"></a><ul id="zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    <p id="zh-cn_topic_0058762427_p62741351184614"><a name="zh-cn_topic_0058762427_p62741351184614"></a><a name="zh-cn_topic_0058762427_p62741351184614"></a>当指定的云硬盘类型在avaliability_zone内不存在时，则创建云硬盘失败。</p>
    <div class="note" id="zh-cn_topic_0058762427_note21808274104217"><a name="zh-cn_topic_0058762427_note21808274104217"></a><a name="zh-cn_topic_0058762427_note21808274104217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0058762427_ul5307015718498"></a><a name="zh-cn_topic_0058762427_ul5307015718498"></a><ul id="zh-cn_topic_0058762427_ul5307015718498"><li><span id="zh-cn_topic_0058762427_text147918435218"><a name="zh-cn_topic_0058762427_text147918435218"></a><a name="zh-cn_topic_0058762427_text147918435218"></a>从快照创建云硬盘时，volume_type字段必须和快照源云硬盘保持一致。</span></li></ul>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row5295776142511"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p1235117143943"><a name="zh-cn_topic_0058762427_p1235117143943"></a><a name="zh-cn_topic_0058762427_p1235117143943"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p32935684143943"><a name="zh-cn_topic_0058762427_p32935684143943"></a><a name="zh-cn_topic_0058762427_p32935684143943"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p50544710143943"><a name="zh-cn_topic_0058762427_p50544710143943"></a><a name="zh-cn_topic_0058762427_p50544710143943"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p480861143943"><a name="zh-cn_topic_0058762427_p480861143943"></a><a name="zh-cn_topic_0058762427_p480861143943"></a>云硬盘的metadata数据，<span id="zh-cn_topic_0058762427_text648010431128"><a name="zh-cn_topic_0058762427_text648010431128"></a><a name="zh-cn_topic_0058762427_text648010431128"></a>metadata中的key和value长度不大于255个字节</span>。</p>
    <p id="zh-cn_topic_0058762427_p618213246557"><a name="zh-cn_topic_0058762427_p618213246557"></a><a name="zh-cn_topic_0058762427_p618213246557"></a>“metadata”字段信息说明请参见“metadata字段说明”表格，表格中列举了部分字段，您还可以根据创建磁盘的要求输入其他字段。</p>
    <div class="note" id="zh-cn_topic_0058762427_note660019322131"><a name="zh-cn_topic_0058762427_note660019322131"></a><a name="zh-cn_topic_0058762427_note660019322131"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1600173216137"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1600173216137"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1600173216137"></a>metadata里面不能有value为null的键值对。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row24630747142515"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p38669085144023"><a name="zh-cn_topic_0058762427_p38669085144023"></a><a name="zh-cn_topic_0058762427_p38669085144023"></a>source_replica</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p45188191144023"><a name="zh-cn_topic_0058762427_p45188191144023"></a><a name="zh-cn_topic_0058762427_p45188191144023"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p36364878144023"><a name="zh-cn_topic_0058762427_p36364878144023"></a><a name="zh-cn_topic_0058762427_p36364878144023"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p59874001144023"><a name="zh-cn_topic_0058762427_p59874001144023"></a><a name="zh-cn_topic_0058762427_p59874001144023"></a>该参数表示从磁盘的克隆来创建云硬盘，当前云硬盘服务不支持该功能。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row33780455142518"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p56697807144126"><a name="zh-cn_topic_0058762427_p56697807144126"></a><a name="zh-cn_topic_0058762427_p56697807144126"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p29119653144126"><a name="zh-cn_topic_0058762427_p29119653144126"></a><a name="zh-cn_topic_0058762427_p29119653144126"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p9881663144126"><a name="zh-cn_topic_0058762427_p9881663144126"></a><a name="zh-cn_topic_0058762427_p9881663144126"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p62217221144126"><a name="zh-cn_topic_0058762427_p62217221144126"></a><a name="zh-cn_topic_0058762427_p62217221144126"></a>一致性组ID，该参数表示此云硬盘属于该一致性组，当前云硬盘服务不支持该功能。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row51354976142522"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p5688610914420"><a name="zh-cn_topic_0058762427_p5688610914420"></a><a name="zh-cn_topic_0058762427_p5688610914420"></a>OS-SCH-HNT:scheduler_hints</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p4437211714420"><a name="zh-cn_topic_0058762427_p4437211714420"></a><a name="zh-cn_topic_0058762427_p4437211714420"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p3737173814420"><a name="zh-cn_topic_0058762427_p3737173814420"></a><a name="zh-cn_topic_0058762427_p3737173814420"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p721192314420"><a name="zh-cn_topic_0058762427_p721192314420"></a><a name="zh-cn_topic_0058762427_p721192314420"></a>调度参数，当前支持dedicated_storage_id字段，表明将云硬盘创建在DSS存储池中。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row7839669175144"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p3052489817525"><a name="zh-cn_topic_0058762427_p3052489817525"></a><a name="zh-cn_topic_0058762427_p3052489817525"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p5659770517525"><a name="zh-cn_topic_0058762427_p5659770517525"></a><a name="zh-cn_topic_0058762427_p5659770517525"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p2101135517525"><a name="zh-cn_topic_0058762427_p2101135517525"></a><a name="zh-cn_topic_0058762427_p2101135517525"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p2419821017525"><a name="zh-cn_topic_0058762427_p2419821017525"></a><a name="zh-cn_topic_0058762427_p2419821017525"></a>扩展属性：共享云硬盘标志位，true为共享盘，false为普通云硬盘。</p>
    <div class="note" id="zh-cn_topic_0058762427_note1645730517525"><a name="zh-cn_topic_0058762427_note1645730517525"></a><a name="zh-cn_topic_0058762427_note1645730517525"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p45212589213213"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p45212589213213"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row46893009142655"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p16191875144233"><a name="zh-cn_topic_0058762427_p16191875144233"></a><a name="zh-cn_topic_0058762427_p16191875144233"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p36473476144233"><a name="zh-cn_topic_0058762427_p36473476144233"></a><a name="zh-cn_topic_0058762427_p36473476144233"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p1561611144233"><a name="zh-cn_topic_0058762427_p1561611144233"></a><a name="zh-cn_topic_0058762427_p1561611144233"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p59381629144233"><a name="zh-cn_topic_0058762427_p59381629144233"></a><a name="zh-cn_topic_0058762427_p59381629144233"></a>共享云硬盘标志位。默认值为false。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >不支持同时使用“source\_volid“、“snapshot\_id“和“imageRef“这三个字段中的任意两个。  

-   metadata参数说明

    <a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_table3430728295554"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_row4496975195554"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5979314595726"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5979314595726"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5979314595726"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1140655395726"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1140655395726"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1140655395726"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5151561095726"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5151561095726"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5151561095726"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="46%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1201488395726"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1201488395726"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1201488395726"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_row456195295554"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1562408795622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1562408795622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5759155095622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5759155095622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5759155095622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3440400295622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3440400295622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3440400295622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p4269864016712"><a name="zh-cn_topic_0058762427_p4269864016712"></a><a name="zh-cn_topic_0058762427_p4269864016712"></a>metadata中的表示加密功能的字段，0代表不加密，1代表加密。</p>
    <p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3526077895622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3526077895622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p3526077895622"></a>该字段不存在时，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_row247050109562"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p241272995622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p241272995622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p6121338895622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p6121338895622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p6121338895622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5933737595622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5933737595622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p5933737595622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p4159804295622"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p4159804295622"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    <div class="note" id="zh-cn_topic_0058762427_note1483983117491"><a name="zh-cn_topic_0058762427_note1483983117491"></a><a name="zh-cn_topic_0058762427_note1483983117491"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p399515405333"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p399515405333"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p399515405333"></a>请参考《密钥管理服务API参考》中的“查询密钥列表”章节通过HTTPS请求获取密钥ID。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_row60499086104915"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1478896104915"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1478896104915"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p52681767104915"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p52681767104915"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p52681767104915"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p39364763104915"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p39364763104915"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p39364763104915"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_ul14462208141855"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_ul14462208141855"></a><ul id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD (虚拟块存储设备 , Virtual Block Device)类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。<div class="note" id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_note30831239112110"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_note30831239112110"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_note30831239112110"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p9045701112110"><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p9045701112110"></a><a name="zh-cn_topic_0058762427_zh-cn_topic_0020235144_p9045701112110"></a>当shareable参数值设置为true，不指定hw:passthrough参数值时，创建的云硬盘为VBD类型共享云硬盘。</p>
    </div></div>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row6091294618292"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762427_p3500156018292"><a name="zh-cn_topic_0058762427_p3500156018292"></a><a name="zh-cn_topic_0058762427_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762427_p1655411118292"><a name="zh-cn_topic_0058762427_p1655411118292"></a><a name="zh-cn_topic_0058762427_p1655411118292"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762427_p6581460618292"><a name="zh-cn_topic_0058762427_p6581460618292"></a><a name="zh-cn_topic_0058762427_p6581460618292"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762427_p47931946183150"><a name="zh-cn_topic_0058762427_p47931946183150"></a><a name="zh-cn_topic_0058762427_p47931946183150"></a>从快照创建云硬盘时，如需使用link克隆方式，请指定该字段的值为0。</p>
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
            "availability_zone": "xxx", 
            "description": "create for api test", 
            "volume_type": "SATA", 
            "metadata": {
                "volume_owner": "openapi"
            }, 
            "consistencygroup_id": null, 
            "source_volid": null, 
            "snapshot_id": null, 
            "multiattach": false, 
            "source_replica": null, 
            "size": 40
        }, 
        "OS-SCH-HNT:scheduler_hints": {
            "dedicated_storage_id": "eddc1a3e-4145-45be-98d7-bf6f65af9767"
        }
    }
    ```


## 响应<a name="section7093323"></a>

-   响应参数

    <a name="zh-cn_topic_0058762427_table34701445142557"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762427_row12524911142557"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762427_p7884856142557"><a name="zh-cn_topic_0058762427_p7884856142557"></a><a name="zh-cn_topic_0058762427_p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762427_p34693598142557"><a name="zh-cn_topic_0058762427_p34693598142557"></a><a name="zh-cn_topic_0058762427_p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.65%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762427_p58539486142557"><a name="zh-cn_topic_0058762427_p58539486142557"></a><a name="zh-cn_topic_0058762427_p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762427_row46605684214651"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p6594039214652"><a name="zh-cn_topic_0058762427_p6594039214652"></a><a name="zh-cn_topic_0058762427_p6594039214652"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p42512970214916"><a name="zh-cn_topic_0058762427_p42512970214916"></a><a name="zh-cn_topic_0058762427_p42512970214916"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p52153745214652"><a name="zh-cn_topic_0058762427_p52153745214652"></a><a name="zh-cn_topic_0058762427_p52153745214652"></a>创建出来的云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row444782011610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p18308336144438"><a name="zh-cn_topic_0058762427_p18308336144438"></a><a name="zh-cn_topic_0058762427_p18308336144438"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p6580236144438"><a name="zh-cn_topic_0058762427_p6580236144438"></a><a name="zh-cn_topic_0058762427_p6580236144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p21928856144438"><a name="zh-cn_topic_0058762427_p21928856144438"></a><a name="zh-cn_topic_0058762427_p21928856144438"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row44077962142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p14226985144438"><a name="zh-cn_topic_0058762427_p14226985144438"></a><a name="zh-cn_topic_0058762427_p14226985144438"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p11535156144438"><a name="zh-cn_topic_0058762427_p11535156144438"></a><a name="zh-cn_topic_0058762427_p11535156144438"></a>array</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p50473003144438"><a name="zh-cn_topic_0058762427_p50473003144438"></a><a name="zh-cn_topic_0058762427_p50473003144438"></a>云硬盘URI自描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row16186817142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p19162411144438"><a name="zh-cn_topic_0058762427_p19162411144438"></a><a name="zh-cn_topic_0058762427_p19162411144438"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p8651439144438"><a name="zh-cn_topic_0058762427_p8651439144438"></a><a name="zh-cn_topic_0058762427_p8651439144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p55103877144438"><a name="zh-cn_topic_0058762427_p55103877144438"></a><a name="zh-cn_topic_0058762427_p55103877144438"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row2987651144410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p39625821144438"><a name="zh-cn_topic_0058762427_p39625821144438"></a><a name="zh-cn_topic_0058762427_p39625821144438"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p55574965144438"><a name="zh-cn_topic_0058762427_p55574965144438"></a><a name="zh-cn_topic_0058762427_p55574965144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p24889213144438"><a name="zh-cn_topic_0058762427_p24889213144438"></a><a name="zh-cn_topic_0058762427_p24889213144438"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row45785905142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p24843442144438"><a name="zh-cn_topic_0058762427_p24843442144438"></a><a name="zh-cn_topic_0058762427_p24843442144438"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p66161799144438"><a name="zh-cn_topic_0058762427_p66161799144438"></a><a name="zh-cn_topic_0058762427_p66161799144438"></a>array</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p27432950144438"><a name="zh-cn_topic_0058762427_p27432950144438"></a><a name="zh-cn_topic_0058762427_p27432950144438"></a>挂载信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row35247553142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p179170144438"><a name="zh-cn_topic_0058762427_p179170144438"></a><a name="zh-cn_topic_0058762427_p179170144438"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p14512814144438"><a name="zh-cn_topic_0058762427_p14512814144438"></a><a name="zh-cn_topic_0058762427_p14512814144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p58206487144438"><a name="zh-cn_topic_0058762427_p58206487144438"></a><a name="zh-cn_topic_0058762427_p58206487144438"></a>云硬盘所属AZ。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row27126244142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p19727534144438"><a name="zh-cn_topic_0058762427_p19727534144438"></a><a name="zh-cn_topic_0058762427_p19727534144438"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p54426427144438"><a name="zh-cn_topic_0058762427_p54426427144438"></a><a name="zh-cn_topic_0058762427_p54426427144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p5526931144438"><a name="zh-cn_topic_0058762427_p5526931144438"></a><a name="zh-cn_topic_0058762427_p5526931144438"></a>是否为可启动云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row7009490142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p2601247144438"><a name="zh-cn_topic_0058762427_p2601247144438"></a><a name="zh-cn_topic_0058762427_p2601247144438"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p9374472144438"><a name="zh-cn_topic_0058762427_p9374472144438"></a><a name="zh-cn_topic_0058762427_p9374472144438"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p34192098144438"><a name="zh-cn_topic_0058762427_p34192098144438"></a><a name="zh-cn_topic_0058762427_p34192098144438"></a>是否为加密云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row49237196142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p28651206144438"><a name="zh-cn_topic_0058762427_p28651206144438"></a><a name="zh-cn_topic_0058762427_p28651206144438"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p1296456144535"><a name="zh-cn_topic_0058762427_p1296456144535"></a><a name="zh-cn_topic_0058762427_p1296456144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p28821893144438"><a name="zh-cn_topic_0058762427_p28821893144438"></a><a name="zh-cn_topic_0058762427_p28821893144438"></a>创建云硬盘的时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row39017307142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p6085885144438"><a name="zh-cn_topic_0058762427_p6085885144438"></a><a name="zh-cn_topic_0058762427_p6085885144438"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p18611115144535"><a name="zh-cn_topic_0058762427_p18611115144535"></a><a name="zh-cn_topic_0058762427_p18611115144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p44410693144438"><a name="zh-cn_topic_0058762427_p44410693144438"></a><a name="zh-cn_topic_0058762427_p44410693144438"></a>云硬盘描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row20107664142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p28923171144438"><a name="zh-cn_topic_0058762427_p28923171144438"></a><a name="zh-cn_topic_0058762427_p28923171144438"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p22198851144535"><a name="zh-cn_topic_0058762427_p22198851144535"></a><a name="zh-cn_topic_0058762427_p22198851144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p9630579144438"><a name="zh-cn_topic_0058762427_p9630579144438"></a><a name="zh-cn_topic_0058762427_p9630579144438"></a>云硬盘类型。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row12897861142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p41370851144438"><a name="zh-cn_topic_0058762427_p41370851144438"></a><a name="zh-cn_topic_0058762427_p41370851144438"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p7354807144535"><a name="zh-cn_topic_0058762427_p7354807144535"></a><a name="zh-cn_topic_0058762427_p7354807144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p27786537144438"><a name="zh-cn_topic_0058762427_p27786537144438"></a><a name="zh-cn_topic_0058762427_p27786537144438"></a>云硬盘复制状态。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row45680217142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p56617581144438"><a name="zh-cn_topic_0058762427_p56617581144438"></a><a name="zh-cn_topic_0058762427_p56617581144438"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p25180208144535"><a name="zh-cn_topic_0058762427_p25180208144535"></a><a name="zh-cn_topic_0058762427_p25180208144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p40860550144438"><a name="zh-cn_topic_0058762427_p40860550144438"></a><a name="zh-cn_topic_0058762427_p40860550144438"></a>所属一致性组ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row47480567142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p58114746144438"><a name="zh-cn_topic_0058762427_p58114746144438"></a><a name="zh-cn_topic_0058762427_p58114746144438"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p47440982144535"><a name="zh-cn_topic_0058762427_p47440982144535"></a><a name="zh-cn_topic_0058762427_p47440982144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p52975605144438"><a name="zh-cn_topic_0058762427_p52975605144438"></a><a name="zh-cn_topic_0058762427_p52975605144438"></a>源云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row31517135142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p31619531144438"><a name="zh-cn_topic_0058762427_p31619531144438"></a><a name="zh-cn_topic_0058762427_p31619531144438"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p66078031144535"><a name="zh-cn_topic_0058762427_p66078031144535"></a><a name="zh-cn_topic_0058762427_p66078031144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p57055846144438"><a name="zh-cn_topic_0058762427_p57055846144438"></a><a name="zh-cn_topic_0058762427_p57055846144438"></a>快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row15610713142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p53325033144438"><a name="zh-cn_topic_0058762427_p53325033144438"></a><a name="zh-cn_topic_0058762427_p53325033144438"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p24360403144438"><a name="zh-cn_topic_0058762427_p24360403144438"></a><a name="zh-cn_topic_0058762427_p24360403144438"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p42403730144438"><a name="zh-cn_topic_0058762427_p42403730144438"></a><a name="zh-cn_topic_0058762427_p42403730144438"></a>元数据。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row5657368142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p42241765144438"><a name="zh-cn_topic_0058762427_p42241765144438"></a><a name="zh-cn_topic_0058762427_p42241765144438"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p66139813144438"><a name="zh-cn_topic_0058762427_p66139813144438"></a><a name="zh-cn_topic_0058762427_p66139813144438"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p17400122144438"><a name="zh-cn_topic_0058762427_p17400122144438"></a><a name="zh-cn_topic_0058762427_p17400122144438"></a>云硬盘大小。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row39412545144428"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p1113688144438"><a name="zh-cn_topic_0058762427_p1113688144438"></a><a name="zh-cn_topic_0058762427_p1113688144438"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p51894643144540"><a name="zh-cn_topic_0058762427_p51894643144540"></a><a name="zh-cn_topic_0058762427_p51894643144540"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p26218517352"><a name="zh-cn_topic_0058762427_p26218517352"></a><a name="zh-cn_topic_0058762427_p26218517352"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row25381049144431"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p26680804144438"><a name="zh-cn_topic_0058762427_p26680804144438"></a><a name="zh-cn_topic_0058762427_p26680804144438"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p39072645144540"><a name="zh-cn_topic_0058762427_p39072645144540"></a><a name="zh-cn_topic_0058762427_p39072645144540"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p42877354144438"><a name="zh-cn_topic_0058762427_p42877354144438"></a><a name="zh-cn_topic_0058762427_p42877354144438"></a>云硬盘更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row48384415144425"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p51969649144438"><a name="zh-cn_topic_0058762427_p51969649144438"></a><a name="zh-cn_topic_0058762427_p51969649144438"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p5099125121957"><a name="zh-cn_topic_0058762427_p5099125121957"></a><a name="zh-cn_topic_0058762427_p5099125121957"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p15113052144438"><a name="zh-cn_topic_0058762427_p15113052144438"></a><a name="zh-cn_topic_0058762427_p15113052144438"></a>是否为可共享云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762427_row42462677142557"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762427_p11561839144438"><a name="zh-cn_topic_0058762427_p11561839144438"></a><a name="zh-cn_topic_0058762427_p11561839144438"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762427_p64093800144438"><a name="zh-cn_topic_0058762427_p64093800144438"></a><a name="zh-cn_topic_0058762427_p64093800144438"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.65%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762427_p15283679144438"><a name="zh-cn_topic_0058762427_p15283679144438"></a><a name="zh-cn_topic_0058762427_p15283679144438"></a>是否为可共享云硬盘。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "volume": {
            "attachments": [ ], 
            "availability_zone": "xxx", 
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


## 返回值<a name="section63839913"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

