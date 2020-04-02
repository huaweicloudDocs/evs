# 创建云硬盘<a name="evs_04_3003"></a>

## 功能介绍<a name="section2630087"></a>

创建一个或多个云硬盘。支持企业项目授权功能。

## URI<a name="section23670787"></a>

-   URI格式

    POST /v3/\{project\_id\}/cloudvolumes

-   参数说明

    <a name="table35460209"></a>
    <table><thead align="left"><tr id="row34639550"><th class="cellrowborder" valign="top" width="28.822882288228826%" id="mcps1.1.4.1.1"><p id="p54340147"><a name="p54340147"></a><a name="p54340147"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.752675267526755%" id="mcps1.1.4.1.2"><p id="p39475801"><a name="p39475801"></a><a name="p39475801"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.42444244424442%" id="mcps1.1.4.1.3"><p id="p43423319"><a name="p43423319"></a><a name="p43423319"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row27627990"><td class="cellrowborder" valign="top" width="28.822882288228826%" headers="mcps1.1.4.1.1 "><p id="p23274750"><a name="p23274750"></a><a name="p23274750"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.752675267526755%" headers="mcps1.1.4.1.2 "><p id="p6206582"><a name="p6206582"></a><a name="p6206582"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.42444244424442%" headers="mcps1.1.4.1.3 "><p id="p32971110"><a name="p32971110"></a><a name="p32971110"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section11710498"></a>

-   请求参数

    <a name="evs_04_2013_table99446146381"></a>
    <table><thead align="left"><tr id="evs_04_2013_row14945201493812"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="evs_04_2013_p49451414203813"><a name="evs_04_2013_p49451414203813"></a><a name="evs_04_2013_p49451414203813"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="evs_04_2013_p7945514153819"><a name="evs_04_2013_p7945514153819"></a><a name="evs_04_2013_p7945514153819"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="evs_04_2013_p14945114203813"><a name="evs_04_2013_p14945114203813"></a><a name="evs_04_2013_p14945114203813"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.494949494949495%" id="mcps1.1.5.1.4"><p id="evs_04_2013_p4946111443810"><a name="evs_04_2013_p4946111443810"></a><a name="evs_04_2013_p4946111443810"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row11946111410383"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p11946214173818"><a name="evs_04_2013_p11946214173818"></a><a name="evs_04_2013_p11946214173818"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p394615141385"><a name="evs_04_2013_p394615141385"></a><a name="evs_04_2013_p394615141385"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p1494601423811"><a name="evs_04_2013_p1494601423811"></a><a name="evs_04_2013_p1494601423811"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p9946141418386"><a name="evs_04_2013_p9946141418386"></a><a name="evs_04_2013_p9946141418386"></a>待创建的云硬盘信息，请参见<a href="#evs_04_2013_li10966323">•volume参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2013_li10966323"></a>volume参数说明

    <a name="evs_04_2013_table31588048"></a>
    <table><thead align="left"><tr id="evs_04_2013_row57330849"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="evs_04_2013_p13287175"><a name="evs_04_2013_p13287175"></a><a name="evs_04_2013_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="evs_04_2013_p2519427"><a name="evs_04_2013_p2519427"></a><a name="evs_04_2013_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="evs_04_2013_p2747002"><a name="evs_04_2013_p2747002"></a><a name="evs_04_2013_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.494949494949495%" id="mcps1.1.5.1.4"><p id="evs_04_2013_p21180630"><a name="evs_04_2013_p21180630"></a><a name="evs_04_2013_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row56407950"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p5641212"><a name="evs_04_2013_p5641212"></a><a name="evs_04_2013_p5641212"></a>backup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p54284994"><a name="evs_04_2013_p54284994"></a><a name="evs_04_2013_p54284994"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p35008393"><a name="evs_04_2013_p35008393"></a><a name="evs_04_2013_p35008393"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p17107576"><a name="evs_04_2013_p17107576"></a><a name="evs_04_2013_p17107576"></a>备份ID，从备份创建云硬盘时为必选。</p>
    <div class="note" id="evs_04_2013_note4897195216919"><a name="evs_04_2013_note4897195216919"></a><a name="evs_04_2013_note4897195216919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p1678892316122"><a name="evs_04_2013_p1678892316122"></a><a name="evs_04_2013_p1678892316122"></a>获取备份ID的方法：请参见<a href="https://support.huaweicloud.com/api-cbr/ListBackups.html" target="_blank" rel="noopener noreferrer">查询所有备份</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row19750463"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p56283646"><a name="evs_04_2013_p56283646"></a><a name="evs_04_2013_p56283646"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p62681466"><a name="evs_04_2013_p62681466"></a><a name="evs_04_2013_p62681466"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p12823082184254"><a name="evs_04_2013_p12823082184254"></a><a name="evs_04_2013_p12823082184254"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p66510234184157"><a name="evs_04_2013_p66510234184157"></a><a name="evs_04_2013_p66510234184157"></a>指定要创建云硬盘的所属AZ，若指定的AZ不存在，则创建云硬盘失败。</p>
    <div class="note" id="evs_04_2013_note18354235112810"><a name="evs_04_2013_note18354235112810"></a><a name="evs_04_2013_note18354235112810"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p14110155594414"><a name="evs_04_2013_p14110155594414"></a><a name="evs_04_2013_p14110155594414"></a>获取AZ的方法：请参考<a href="查询所有的可用分区信息-Cinder-v2.md">查询所有的可用分区信息</a>获取。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row22709757"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p27551015"><a name="evs_04_2013_p27551015"></a><a name="evs_04_2013_p27551015"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p17039762"><a name="evs_04_2013_p17039762"></a><a name="evs_04_2013_p17039762"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p38043494"><a name="evs_04_2013_p38043494"></a><a name="evs_04_2013_p38043494"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p58865735113756"><a name="evs_04_2013_p58865735113756"></a><a name="evs_04_2013_p58865735113756"></a>云硬盘的描述。<span id="evs_04_2013_text62679346101929"><a name="evs_04_2013_text62679346101929"></a><a name="evs_04_2013_text62679346101929"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2013_row17746329"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p28166553"><a name="evs_04_2013_p28166553"></a><a name="evs_04_2013_p28166553"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p66898301"><a name="evs_04_2013_p66898301"></a><a name="evs_04_2013_p66898301"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p50053294"><a name="evs_04_2013_p50053294"></a><a name="evs_04_2013_p50053294"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><div class="p" id="evs_04_2013_p27784979"><a name="evs_04_2013_p27784979"></a><a name="evs_04_2013_p27784979"></a>云硬盘大小，单位为GB，其限制如下：<a name="evs_04_2013_ul24506304547"></a><a name="evs_04_2013_ul24506304547"></a><ul id="evs_04_2013_ul24506304547"><li>系统盘：1GB-1024GB</li><li>数据盘：10GB-32768GB</li></ul>
    </div>
    <p id="evs_04_2013_p1869819398426"><a name="evs_04_2013_p1869819398426"></a><a name="evs_04_2013_p1869819398426"></a>创建空白云硬盘，size为必选，请在范围内根据需求自定义。</p>
    <p id="evs_04_2013_p433134181712"><a name="evs_04_2013_p433134181712"></a><a name="evs_04_2013_p433134181712"></a>从快照创建云硬盘时，size为必选，且云硬盘大小不能小于快照大小。</p>
    <p id="evs_04_2013_p108486266429"><a name="evs_04_2013_p108486266429"></a><a name="evs_04_2013_p108486266429"></a>从镜像创建云硬盘时，size为必选，且云硬盘大小不小于镜像属性中min_disk要求的最小云硬盘容量。</p>
    <p id="evs_04_2013_p55481787"><a name="evs_04_2013_p55481787"></a><a name="evs_04_2013_p55481787"></a>从备份创建云硬盘时，size为可选，不指定size时，云硬盘大小和备份大小一致。</p>
    <div class="note" id="evs_04_2013_note6528620415911"><a name="evs_04_2013_note6528620415911"></a><a name="evs_04_2013_note6528620415911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p5070492815911"><a name="evs_04_2013_p5070492815911"></a><a name="evs_04_2013_p5070492815911"></a>如果发送请求时，将参数值设置为小数，则默认取小数点前的整数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row29574043"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p46687245"><a name="evs_04_2013_p46687245"></a><a name="evs_04_2013_p46687245"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p23570516"><a name="evs_04_2013_p23570516"></a><a name="evs_04_2013_p23570516"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p30163672"><a name="evs_04_2013_p30163672"></a><a name="evs_04_2013_p30163672"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p30342314172932"><a name="evs_04_2013_p30342314172932"></a><a name="evs_04_2013_p30342314172932"></a>云硬盘名称。</p>
    <a name="evs_04_2013_ul46606633102055"></a><a name="evs_04_2013_ul46606633102055"></a><ul id="evs_04_2013_ul46606633102055"><li>如果为创建单个云硬盘，name为云硬盘名称。<span id="evs_04_2013_text2318400210216"><a name="evs_04_2013_text2318400210216"></a><a name="evs_04_2013_text2318400210216"></a>最大支持255个字节。</span></li><li>创建的云硬盘数量（count字段对应的值）大于1时，为区分不同云硬盘，创建过程中系统会自动在名称后加“-0000”的类似标记。例如：volume-0001、volume-0002。<span id="evs_04_2013_text688013214465"><a name="evs_04_2013_text688013214465"></a><a name="evs_04_2013_text688013214465"></a>最大支持250个字节。</span></li></ul>
    </td>
    </tr>
    <tr id="evs_04_2013_row30068235161750"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p41087296161752"><a name="evs_04_2013_p41087296161752"></a><a name="evs_04_2013_p41087296161752"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p39736646161752"><a name="evs_04_2013_p39736646161752"></a><a name="evs_04_2013_p39736646161752"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p64551757161752"><a name="evs_04_2013_p64551757161752"></a><a name="evs_04_2013_p64551757161752"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p61309820161752"><a name="evs_04_2013_p61309820161752"></a><a name="evs_04_2013_p61309820161752"></a>快照ID，指定该参数表示创建云硬盘方式为从快照创建云硬盘。</p>
    <div class="note" id="evs_04_2013_note13293123112911"><a name="evs_04_2013_note13293123112911"></a><a name="evs_04_2013_note13293123112911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p129419232297"><a name="evs_04_2013_p129419232297"></a><a name="evs_04_2013_p129419232297"></a>获取快照ID的方法：请参见<a href="查询云硬盘快照详细信息列表-Cinder-v2.md">查询云硬盘快照详细信息列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row65447007"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p66716242"><a name="evs_04_2013_p66716242"></a><a name="evs_04_2013_p66716242"></a>imageRef</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p35306501"><a name="evs_04_2013_p35306501"></a><a name="evs_04_2013_p35306501"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p41254304"><a name="evs_04_2013_p41254304"></a><a name="evs_04_2013_p41254304"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p53264332"><a name="evs_04_2013_p53264332"></a><a name="evs_04_2013_p53264332"></a>IMS中镜像ID，指定该参数表示创建云硬盘方式为从镜像创建云硬盘。</p>
    <div class="note" id="evs_04_2013_note13789049151930"><a name="evs_04_2013_note13789049151930"></a><a name="evs_04_2013_note13789049151930"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p56992577151930"><a name="evs_04_2013_p56992577151930"></a><a name="evs_04_2013_p56992577151930"></a>不支持通过BMS的镜像创建BMS系统盘。</p>
    <p id="evs_04_2013_p9572163215333"><a name="evs_04_2013_p9572163215333"></a><a name="evs_04_2013_p9572163215333"></a>获取镜像ID的方法：请参见<a href="https://support.huaweicloud.com/api-ims/ims_03_0602.html" target="_blank" rel="noopener noreferrer">查询镜像列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row9616944"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p40774967"><a name="evs_04_2013_p40774967"></a><a name="evs_04_2013_p40774967"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p14438051"><a name="evs_04_2013_p14438051"></a><a name="evs_04_2013_p14438051"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p41198362184535"><a name="evs_04_2013_p41198362184535"></a><a name="evs_04_2013_p41198362184535"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p14380476104717"><a name="evs_04_2013_p14380476104717"></a><a name="evs_04_2013_p14380476104717"></a>云硬盘类型。</p>
    <div class="p" id="evs_04_2013_p112762317377"><a name="evs_04_2013_p112762317377"></a><a name="evs_04_2013_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="evs_04_2013_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="evs_04_2013_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="evs_04_2013_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    <p id="evs_04_2013_p62741351184614"><a name="evs_04_2013_p62741351184614"></a><a name="evs_04_2013_p62741351184614"></a>当指定的云硬盘类型在avaliability_zone内不存在时，则创建云硬盘失败。</p>
    <div class="note" id="evs_04_2013_note21808274104217"><a name="evs_04_2013_note21808274104217"></a><a name="evs_04_2013_note21808274104217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="evs_04_2013_ul5307015718498"></a><a name="evs_04_2013_ul5307015718498"></a><ul id="evs_04_2013_ul5307015718498"><li><span id="evs_04_2013_text7492111913438"><a name="evs_04_2013_text7492111913438"></a><a name="evs_04_2013_text7492111913438"></a>从快照创建云硬盘时，volume_type字段必须和快照源云硬盘保持一致。</span></li><li>了解不同磁盘类型的详细信息，请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0044524691.html" target="_blank" rel="noopener noreferrer">磁盘类型及性能介绍</a>。</li></ul>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row7461047"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p365031"><a name="evs_04_2013_p365031"></a><a name="evs_04_2013_p365031"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p29567523"><a name="evs_04_2013_p29567523"></a><a name="evs_04_2013_p29567523"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p428797710293"><a name="evs_04_2013_p428797710293"></a><a name="evs_04_2013_p428797710293"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p47906786"><a name="evs_04_2013_p47906786"></a><a name="evs_04_2013_p47906786"></a>批量创云硬盘的个数。如果无该参数，表明只创建1个云硬盘，目前最多支持批量创建100个。</p>
    <p id="evs_04_2013_p9550502101436"><a name="evs_04_2013_p9550502101436"></a><a name="evs_04_2013_p9550502101436"></a>从备份创建云硬盘时，不支持批量创建，数量只能为<span class="parmname" id="evs_04_2013_parmname54941195437"><a name="evs_04_2013_parmname54941195437"></a><a name="evs_04_2013_parmname54941195437"></a>“1”</span>。</p>
    <div class="note" id="evs_04_2013_note57300341151148"><a name="evs_04_2013_note57300341151148"></a><a name="evs_04_2013_note57300341151148"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_evs_04_2013_p5070492815911"><a name="evs_04_2013_evs_04_2013_p5070492815911"></a><a name="evs_04_2013_evs_04_2013_p5070492815911"></a>如果发送请求时，将参数值设置为小数，则默认取小数点前的整数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row2434599211437"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p1778734011437"><a name="evs_04_2013_p1778734011437"></a><a name="evs_04_2013_p1778734011437"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p3148844911437"><a name="evs_04_2013_p3148844911437"></a><a name="evs_04_2013_p3148844911437"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p42756211437"><a name="evs_04_2013_p42756211437"></a><a name="evs_04_2013_p42756211437"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p3463256011437"><a name="evs_04_2013_p3463256011437"></a><a name="evs_04_2013_p3463256011437"></a>是否为共享云硬盘。true为共享盘，false为普通云硬盘。</p>
    <div class="note" id="evs_04_2013_note3800959821323"><a name="evs_04_2013_note3800959821323"></a><a name="evs_04_2013_note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p45212589213213"><a name="evs_04_2013_p45212589213213"></a><a name="evs_04_2013_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row494599159816"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p424860529816"><a name="evs_04_2013_p424860529816"></a><a name="evs_04_2013_p424860529816"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p188182169816"><a name="evs_04_2013_p188182169816"></a><a name="evs_04_2013_p188182169816"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p478805289816"><a name="evs_04_2013_p478805289816"></a><a name="evs_04_2013_p478805289816"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p323873209920"><a name="evs_04_2013_p323873209920"></a><a name="evs_04_2013_p323873209920"></a>创建云硬盘的metadata信息，<span id="evs_04_2013_text149521944318"><a name="evs_04_2013_text149521944318"></a><a name="evs_04_2013_text149521944318"></a>metadata中的key和value长度不大于255个字节</span>。</p>
    <p id="evs_04_2013_p862801317585"><a name="evs_04_2013_p862801317585"></a><a name="evs_04_2013_p862801317585"></a>“metadata”字段信息说明请参见<a href="#evs_04_2013_li4145283210319">•metadata参数说明</a>，创建磁盘时仅支持表格中提供的字段。</p>
    <div class="note" id="evs_04_2013_note660019322131"><a name="evs_04_2013_note660019322131"></a><a name="evs_04_2013_note660019322131"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p1600173216137"><a name="evs_04_2013_p1600173216137"></a><a name="evs_04_2013_p1600173216137"></a>metadata里面不能有value为null的键值对。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row4752931910472"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p2466966510472"><a name="evs_04_2013_p2466966510472"></a><a name="evs_04_2013_p2466966510472"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p5208587610472"><a name="evs_04_2013_p5208587610472"></a><a name="evs_04_2013_p5208587610472"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p5820640710472"><a name="evs_04_2013_p5820640710472"></a><a name="evs_04_2013_p5820640710472"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><div class="p" id="evs_04_2013_p4531155053519"><a name="evs_04_2013_p4531155053519"></a><a name="evs_04_2013_p4531155053519"></a>创建共享云硬盘的信息。默认值为false。<a name="evs_04_2013_ul202952187368"></a><a name="evs_04_2013_ul202952187368"></a><ul id="evs_04_2013_ul202952187368"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    <p id="evs_04_2013_p96242024104913"><a name="evs_04_2013_p96242024104913"></a><a name="evs_04_2013_p96242024104913"></a>请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0032860759.html" target="_blank" rel="noopener noreferrer">共享云硬盘及使用方法</a>了解更多信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2013_row179945620499"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p39941261495"><a name="evs_04_2013_p39941261495"></a><a name="evs_04_2013_p39941261495"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p1499413644915"><a name="evs_04_2013_p1499413644915"></a><a name="evs_04_2013_p1499413644915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p79947634918"><a name="evs_04_2013_p79947634918"></a><a name="evs_04_2013_p79947634918"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p35013964916"><a name="evs_04_2013_p35013964916"></a><a name="evs_04_2013_p35013964916"></a>企业项目ID。创建云硬盘时，给云硬盘绑定企业项目ID。</p>
    <p id="evs_04_2013_p16244102205013"><a name="evs_04_2013_p16244102205013"></a><a name="evs_04_2013_p16244102205013"></a><span id="evs_04_2013_text98761511155218"><a name="evs_04_2013_text98761511155218"></a><a name="evs_04_2013_text98761511155218"></a>该参数不传，或者将该参数值设置为0，则将资源绑定给默认企业项目。</span></p>
    <div class="note" id="evs_04_2013_note16336122416016"><a name="evs_04_2013_note16336122416016"></a><a name="evs_04_2013_note16336122416016"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p18336524404"><a name="evs_04_2013_p18336524404"></a><a name="evs_04_2013_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >不支持同时使用“backup\_id“、“snapshot\_id“和“imageRef“这三个字段中的任意两个。  

-   <a name="evs_04_2013_li4145283210319"></a>metadata参数说明

    <a name="evs_04_2013_table3430728295554"></a>
    <table><thead align="left"><tr id="evs_04_2013_row4496975195554"><th class="cellrowborder" valign="top" width="17.04%" id="mcps1.1.5.1.1"><p id="evs_04_2013_p8809200174410"><a name="evs_04_2013_p8809200174410"></a><a name="evs_04_2013_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.96%" id="mcps1.1.5.1.2"><p id="evs_04_2013_p168135017449"><a name="evs_04_2013_p168135017449"></a><a name="evs_04_2013_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="evs_04_2013_p1381850154410"><a name="evs_04_2013_p1381850154410"></a><a name="evs_04_2013_p1381850154410"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="evs_04_2013_p1282213034412"><a name="evs_04_2013_p1282213034412"></a><a name="evs_04_2013_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row456195295554"><td class="cellrowborder" valign="top" width="17.04%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p1562408795622"><a name="evs_04_2013_p1562408795622"></a><a name="evs_04_2013_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p5759155095622"><a name="evs_04_2013_p5759155095622"></a><a name="evs_04_2013_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p3440400295622"><a name="evs_04_2013_p3440400295622"></a><a name="evs_04_2013_p3440400295622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p729227516614"><a name="evs_04_2013_p729227516614"></a><a name="evs_04_2013_p729227516614"></a>metadata中的表示加密功能的字段，0代表不加密，1代表加密。</p>
    <p id="evs_04_2013_p3526077895622"><a name="evs_04_2013_p3526077895622"></a><a name="evs_04_2013_p3526077895622"></a>该字段不存在时，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="evs_04_2013_row247050109562"><td class="cellrowborder" valign="top" width="17.04%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p241272995622"><a name="evs_04_2013_p241272995622"></a><a name="evs_04_2013_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p6121338895622"><a name="evs_04_2013_p6121338895622"></a><a name="evs_04_2013_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p5933737595622"><a name="evs_04_2013_p5933737595622"></a><a name="evs_04_2013_p5933737595622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p4159804295622"><a name="evs_04_2013_p4159804295622"></a><a name="evs_04_2013_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    <div class="note" id="evs_04_2013_note16994174013320"><a name="evs_04_2013_note16994174013320"></a><a name="evs_04_2013_note16994174013320"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p093935613512"><a name="evs_04_2013_p093935613512"></a><a name="evs_04_2013_p093935613512"></a>请参考<a href="https://support.huaweicloud.com/api-dew/dew_02_0017.html" target="_blank" rel="noopener noreferrer">查询密钥列表</a>，通过HTTPS请求获取密钥ID。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row60499086104915"><td class="cellrowborder" valign="top" width="17.04%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p1478896104915"><a name="evs_04_2013_p1478896104915"></a><a name="evs_04_2013_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p52681767104915"><a name="evs_04_2013_p52681767104915"></a><a name="evs_04_2013_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p39364763104915"><a name="evs_04_2013_p39364763104915"></a><a name="evs_04_2013_p39364763104915"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><a name="evs_04_2013_ul14462208141855"></a><a name="evs_04_2013_ul14462208141855"></a><ul id="evs_04_2013_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD (虚拟块存储设备 , Virtual Block Device)类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </td>
    </tr>
    <tr id="evs_04_2013_row991210132288"><td class="cellrowborder" valign="top" width="17.04%" headers="mcps1.1.5.1.1 "><p id="evs_04_2013_p3500156018292"><a name="evs_04_2013_p3500156018292"></a><a name="evs_04_2013_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.96%" headers="mcps1.1.5.1.2 "><p id="evs_04_2013_p1655411118292"><a name="evs_04_2013_p1655411118292"></a><a name="evs_04_2013_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2013_p6581460618292"><a name="evs_04_2013_p6581460618292"></a><a name="evs_04_2013_p6581460618292"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2013_p47931946183150"><a name="evs_04_2013_p47931946183150"></a><a name="evs_04_2013_p47931946183150"></a>从快照创建云硬盘时，如需使用link克隆方式，请指定该字段的值为0。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >创建磁盘时， “metadata”仅支持以上表格中提供的字段。  
    >-   如果是从快照创建云硬盘，则不支持传入“\_\_system\_\_encrypted“和“\_\_system\_\_cmkid“字段，创建出来的云硬盘与快照源云硬盘的加密属性一致。  
    >-   如果是从镜像创建云硬盘，则不支持传入“\_\_system\_\_encrypted“和“\_\_system\_\_cmkid“字段，创建出来的云硬盘与镜像的加密属性一致。  
    >-   如果是从快照创建云硬盘，则不支持传入“hw:passthrough“字段，创建出来的云硬盘的设备类型与快照源云硬盘保持一致。  
    >-   如果是从镜像创建云硬盘，则不支持传入“hw:passthrough“字段，创建出来的云硬盘的设备类型为VBD类型。  

-   请求样例

    ```
    {
        "volume": {
            "backup_id": null, 
            "count": 1, 
            "availability_zone": "az-dc-1", 
            "description": "test_volume_1", 
            "size": 120, 
            "name": "test_volume_1", 
            "volume_type": "SSD", 
            "metadata": {
                "__system__encrypted": "1", 
                "__system__cmkid": "37b0d52e-c249-40d6-83cb-2b93f22445bd"
            }
        }
    }
    ```


## 响应消息<a name="section38285619"></a>

-   响应参数

    <a name="evs_04_2013_table735313581437"></a>
    <table><thead align="left"><tr id="evs_04_2013_row153536585313"><th class="cellrowborder" valign="top" width="21.157884211578843%" id="mcps1.1.4.1.1"><p id="evs_04_2013_p123541158732"><a name="evs_04_2013_p123541158732"></a><a name="evs_04_2013_p123541158732"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.197880211978802%" id="mcps1.1.4.1.2"><p id="evs_04_2013_p1435411581320"><a name="evs_04_2013_p1435411581320"></a><a name="evs_04_2013_p1435411581320"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2013_p13541058036"><a name="evs_04_2013_p13541058036"></a><a name="evs_04_2013_p13541058036"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row1135495819312"><td class="cellrowborder" valign="top" width="21.157884211578843%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p33545583319"><a name="evs_04_2013_p33545583319"></a><a name="evs_04_2013_p33545583319"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.197880211978802%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p19354165810317"><a name="evs_04_2013_p19354165810317"></a><a name="evs_04_2013_p19354165810317"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p435416581936"><a name="evs_04_2013_p435416581936"></a><a name="evs_04_2013_p435416581936"></a>正常返回时返回的任务ID。</p>
    <div class="note" id="evs_04_2013_note335410589314"><a name="evs_04_2013_note335410589314"></a><a name="evs_04_2013_note335410589314"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p1435514588312"><a name="evs_04_2013_p1435514588312"></a><a name="evs_04_2013_p1435514588312"></a>如果需要查询job的状态，请参考<a href="查询job的状态.md">查询job的状态</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row195162113414"><td class="cellrowborder" valign="top" width="21.157884211578843%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p129522216412"><a name="evs_04_2013_p129522216412"></a><a name="evs_04_2013_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.197880211978802%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p1595262111415"><a name="evs_04_2013_p1595262111415"></a><a name="evs_04_2013_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p109527215417"><a name="evs_04_2013_p109527215417"></a><a name="evs_04_2013_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2013_li24688256">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2013_li24688256"></a>error参数说明

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
        "job_id": "70a599e0-31e7-49b7-b260-868f441e862b"
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


## 状态码<a name="section8169161010338"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

