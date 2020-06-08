# 创建云硬盘<a name="evs_04_2003"></a>

## 功能介绍<a name="section2630087"></a>

本接口兼容“[创建云硬盘（废弃）](创建云硬盘（废弃）.md)”接口的功能，同时合入新功能，支持创建包周期的云硬盘。支持企业项目授权功能。

在成功调用本接口创建包周期云硬盘后：

-   如果您需要查看订单可用的优惠券，请参考[查询订单可用优惠券](https://support.huaweicloud.com/api-oce/zh-cn_topic_0092953630.html)。
-   如果您需要支付订单，请参考[支付包周期产品订单](https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html)。
-   如果您需要查询订单的资源开通详情，请参考[查询订单的资源开通详情](https://support.huaweicloud.com/api-oce/api_order_00001.html)。
-   如果您需要退订该包周期资源，请参考“[退订包周期资源](https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html)”。

## URI<a name="section23670787"></a>

-   URI格式

    POST /v2.1/\{project\_id\}/cloudvolumes

-   参数说明

    <a name="table35460209"></a>
    <table><thead align="left"><tr id="row34639550"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.4.1.1"><p id="p54340147"><a name="p54340147"></a><a name="p54340147"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.4.1.2"><p id="p39475801"><a name="p39475801"></a><a name="p39475801"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44%" id="mcps1.1.4.1.3"><p id="p43423319"><a name="p43423319"></a><a name="p43423319"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row27627990"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.1 "><p id="p23274750"><a name="p23274750"></a><a name="p23274750"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.2 "><p id="p6206582"><a name="p6206582"></a><a name="p6206582"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.1.4.1.3 "><p id="p32971110"><a name="p32971110"></a><a name="p32971110"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section11710498"></a>

-   请求参数

    <a name="table15991803151217"></a>
    <table><thead align="left"><tr id="row31790627151217"><th class="cellrowborder" valign="top" width="17.07%" id="mcps1.1.5.1.1"><p id="p24903971151217"><a name="p24903971151217"></a><a name="p24903971151217"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.93%" id="mcps1.1.5.1.2"><p id="p3955780151217"><a name="p3955780151217"></a><a name="p3955780151217"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p51982765151217"><a name="p51982765151217"></a><a name="p51982765151217"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p49854471151217"><a name="p49854471151217"></a><a name="p49854471151217"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row11680378151217"><td class="cellrowborder" valign="top" width="17.07%" headers="mcps1.1.5.1.1 "><p id="p6586541151217"><a name="p6586541151217"></a><a name="p6586541151217"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.93%" headers="mcps1.1.5.1.2 "><p id="p63747784151217"><a name="p63747784151217"></a><a name="p63747784151217"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p63296884151217"><a name="p63296884151217"></a><a name="p63296884151217"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p26773976151217"><a name="p26773976151217"></a><a name="p26773976151217"></a>待创建的云硬盘信息，请参见<a href="#li10966323">•volume参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row39639199151217"><td class="cellrowborder" valign="top" width="17.07%" headers="mcps1.1.5.1.1 "><p id="p56658571151217"><a name="p56658571151217"></a><a name="p56658571151217"></a>bssParam</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.93%" headers="mcps1.1.5.1.2 "><p id="p25941572151217"><a name="p25941572151217"></a><a name="p25941572151217"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p20892593151217"><a name="p20892593151217"></a><a name="p20892593151217"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p14578491151217"><a name="p14578491151217"></a><a name="p14578491151217"></a>按需和包周期的扩展参数，请参见<a href="#li5068387212423">•bssParam参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li10966323"></a>volume参数说明

    <a name="zh-cn_topic_0044524833_table31588048"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0044524833_row57330849"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0044524833_p13287175"><a name="zh-cn_topic_0044524833_p13287175"></a><a name="zh-cn_topic_0044524833_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0044524833_p2519427"><a name="zh-cn_topic_0044524833_p2519427"></a><a name="zh-cn_topic_0044524833_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0044524833_p2747002"><a name="zh-cn_topic_0044524833_p2747002"></a><a name="zh-cn_topic_0044524833_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49.494949494949495%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0044524833_p21180630"><a name="zh-cn_topic_0044524833_p21180630"></a><a name="zh-cn_topic_0044524833_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0044524833_row56407950"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p5641212"><a name="zh-cn_topic_0044524833_p5641212"></a><a name="zh-cn_topic_0044524833_p5641212"></a>backup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p54284994"><a name="zh-cn_topic_0044524833_p54284994"></a><a name="zh-cn_topic_0044524833_p54284994"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p35008393"><a name="zh-cn_topic_0044524833_p35008393"></a><a name="zh-cn_topic_0044524833_p35008393"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p17107576"><a name="zh-cn_topic_0044524833_p17107576"></a><a name="zh-cn_topic_0044524833_p17107576"></a>备份ID，从备份创建云硬盘时为必选。</p>
    <div class="note" id="zh-cn_topic_0044524833_note4897195216919"><a name="zh-cn_topic_0044524833_note4897195216919"></a><a name="zh-cn_topic_0044524833_note4897195216919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1678892316122"><a name="p1678892316122"></a><a name="p1678892316122"></a>获取备份ID的方法：请参见<a href="https://support.huaweicloud.com/api-cbr/ListBackups.html" target="_blank" rel="noopener noreferrer">查询所有备份</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row19750463"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p56283646"><a name="zh-cn_topic_0044524833_p56283646"></a><a name="zh-cn_topic_0044524833_p56283646"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p62681466"><a name="zh-cn_topic_0044524833_p62681466"></a><a name="zh-cn_topic_0044524833_p62681466"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p12823082184254"><a name="zh-cn_topic_0044524833_p12823082184254"></a><a name="zh-cn_topic_0044524833_p12823082184254"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p66510234184157"><a name="zh-cn_topic_0044524833_p66510234184157"></a><a name="zh-cn_topic_0044524833_p66510234184157"></a>指定要创建云硬盘的所属AZ，若指定的AZ不存在，则创建云硬盘失败。</p>
    <div class="note" id="zh-cn_topic_0044524833_note18354235112810"><a name="zh-cn_topic_0044524833_note18354235112810"></a><a name="zh-cn_topic_0044524833_note18354235112810"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p14110155594414"><a name="zh-cn_topic_0044524833_p14110155594414"></a><a name="zh-cn_topic_0044524833_p14110155594414"></a>获取AZ的方法：请参考<a href="查询所有的可用分区信息-Cinder-v2.md">查询所有的可用分区信息</a>获取。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row22709757"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p27551015"><a name="zh-cn_topic_0044524833_p27551015"></a><a name="zh-cn_topic_0044524833_p27551015"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p17039762"><a name="zh-cn_topic_0044524833_p17039762"></a><a name="zh-cn_topic_0044524833_p17039762"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p38043494"><a name="zh-cn_topic_0044524833_p38043494"></a><a name="zh-cn_topic_0044524833_p38043494"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p58865735113756"><a name="zh-cn_topic_0044524833_p58865735113756"></a><a name="zh-cn_topic_0044524833_p58865735113756"></a>云硬盘的描述。<span id="zh-cn_topic_0044524833_text62679346101929"><a name="zh-cn_topic_0044524833_text62679346101929"></a><a name="zh-cn_topic_0044524833_text62679346101929"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row17746329"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p28166553"><a name="zh-cn_topic_0044524833_p28166553"></a><a name="zh-cn_topic_0044524833_p28166553"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p66898301"><a name="zh-cn_topic_0044524833_p66898301"></a><a name="zh-cn_topic_0044524833_p66898301"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p50053294"><a name="zh-cn_topic_0044524833_p50053294"></a><a name="zh-cn_topic_0044524833_p50053294"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><div class="p" id="p27784979"><a name="p27784979"></a><a name="p27784979"></a>云硬盘大小，单位为GB，其限制如下：<a name="ul24506304547"></a><a name="ul24506304547"></a><ul id="ul24506304547"><li>系统盘：1GB-1024GB</li><li>数据盘：10GB-32768GB</li></ul>
    </div>
    <p id="p1869819398426"><a name="p1869819398426"></a><a name="p1869819398426"></a>创建空白云硬盘，size为必选，请在范围内根据需求自定义。</p>
    <p id="p433134181712"><a name="p433134181712"></a><a name="p433134181712"></a>从快照创建云硬盘时，size为必选，且云硬盘大小不能小于快照大小。</p>
    <p id="p108486266429"><a name="p108486266429"></a><a name="p108486266429"></a>从镜像创建云硬盘时，size为必选，且云硬盘大小不小于镜像属性中min_disk要求的最小云硬盘容量。</p>
    <p id="p55481787"><a name="p55481787"></a><a name="p55481787"></a>从备份创建云硬盘时，size为可选，不指定size时，云硬盘大小和备份大小一致。</p>
    <div class="note" id="zh-cn_topic_0044524833_note6528620415911"><a name="zh-cn_topic_0044524833_note6528620415911"></a><a name="zh-cn_topic_0044524833_note6528620415911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p5070492815911"><a name="zh-cn_topic_0044524833_p5070492815911"></a><a name="zh-cn_topic_0044524833_p5070492815911"></a>如果发送请求时，将参数值设置为小数，则默认取小数点前的整数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row29574043"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p46687245"><a name="zh-cn_topic_0044524833_p46687245"></a><a name="zh-cn_topic_0044524833_p46687245"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p23570516"><a name="zh-cn_topic_0044524833_p23570516"></a><a name="zh-cn_topic_0044524833_p23570516"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p30163672"><a name="zh-cn_topic_0044524833_p30163672"></a><a name="zh-cn_topic_0044524833_p30163672"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p30342314172932"><a name="zh-cn_topic_0044524833_p30342314172932"></a><a name="zh-cn_topic_0044524833_p30342314172932"></a>云硬盘名称。</p>
    <a name="zh-cn_topic_0044524833_ul46606633102055"></a><a name="zh-cn_topic_0044524833_ul46606633102055"></a><ul id="zh-cn_topic_0044524833_ul46606633102055"><li>如果为创建单个云硬盘，name为云硬盘名称。<span id="zh-cn_topic_0044524833_text2318400210216"><a name="zh-cn_topic_0044524833_text2318400210216"></a><a name="zh-cn_topic_0044524833_text2318400210216"></a>最大支持255个字节。</span></li><li>创建的云硬盘数量（count字段对应的值）大于1时，为区分不同云硬盘，创建过程中系统会自动在名称后加“-0000”的类似标记。例如：volume-0001、volume-0002。<span id="text688013214465"><a name="text688013214465"></a><a name="text688013214465"></a>最大支持250个字节。</span></li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row30068235161750"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p41087296161752"><a name="zh-cn_topic_0044524833_p41087296161752"></a><a name="zh-cn_topic_0044524833_p41087296161752"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p39736646161752"><a name="zh-cn_topic_0044524833_p39736646161752"></a><a name="zh-cn_topic_0044524833_p39736646161752"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p64551757161752"><a name="zh-cn_topic_0044524833_p64551757161752"></a><a name="zh-cn_topic_0044524833_p64551757161752"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p61309820161752"><a name="zh-cn_topic_0044524833_p61309820161752"></a><a name="zh-cn_topic_0044524833_p61309820161752"></a>快照ID，指定该参数表示创建云硬盘方式为从快照创建云硬盘。</p>
    <div class="note" id="zh-cn_topic_0044524833_note13293123112911"><a name="zh-cn_topic_0044524833_note13293123112911"></a><a name="zh-cn_topic_0044524833_note13293123112911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p129419232297"><a name="zh-cn_topic_0044524833_p129419232297"></a><a name="zh-cn_topic_0044524833_p129419232297"></a>获取快照ID的方法：请参见<a href="查询云硬盘快照详细信息列表-Cinder-v2.md">查询云硬盘快照详细信息列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row65447007"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p66716242"><a name="zh-cn_topic_0044524833_p66716242"></a><a name="zh-cn_topic_0044524833_p66716242"></a>imageRef</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p35306501"><a name="zh-cn_topic_0044524833_p35306501"></a><a name="zh-cn_topic_0044524833_p35306501"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p41254304"><a name="zh-cn_topic_0044524833_p41254304"></a><a name="zh-cn_topic_0044524833_p41254304"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p53264332"><a name="zh-cn_topic_0044524833_p53264332"></a><a name="zh-cn_topic_0044524833_p53264332"></a>IMS中镜像ID，指定该参数表示创建云硬盘方式为从镜像创建云硬盘。</p>
    <div class="note" id="zh-cn_topic_0044524833_note13789049151930"><a name="zh-cn_topic_0044524833_note13789049151930"></a><a name="zh-cn_topic_0044524833_note13789049151930"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p56992577151930"><a name="zh-cn_topic_0044524833_p56992577151930"></a><a name="zh-cn_topic_0044524833_p56992577151930"></a>不支持通过BMS的镜像创建BMS系统盘。</p>
    <p id="zh-cn_topic_0044524833_p9572163215333"><a name="zh-cn_topic_0044524833_p9572163215333"></a><a name="zh-cn_topic_0044524833_p9572163215333"></a>获取镜像ID的方法：请参见<a href="https://support.huaweicloud.com/api-ims/ims_03_0602.html" target="_blank" rel="noopener noreferrer">查询镜像列表</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row9616944"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p40774967"><a name="zh-cn_topic_0044524833_p40774967"></a><a name="zh-cn_topic_0044524833_p40774967"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p14438051"><a name="zh-cn_topic_0044524833_p14438051"></a><a name="zh-cn_topic_0044524833_p14438051"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p41198362184535"><a name="zh-cn_topic_0044524833_p41198362184535"></a><a name="zh-cn_topic_0044524833_p41198362184535"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p14380476104717"><a name="zh-cn_topic_0044524833_p14380476104717"></a><a name="zh-cn_topic_0044524833_p14380476104717"></a>云硬盘类型。</p>
    <div class="p" id="zh-cn_topic_0044524833_p112762317377"><a name="zh-cn_topic_0044524833_p112762317377"></a><a name="zh-cn_topic_0044524833_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    <p id="zh-cn_topic_0044524833_p62741351184614"><a name="zh-cn_topic_0044524833_p62741351184614"></a><a name="zh-cn_topic_0044524833_p62741351184614"></a>当指定的云硬盘类型在avaliability_zone内不存在时，则创建云硬盘失败。</p>
    <div class="note" id="zh-cn_topic_0044524833_note21808274104217"><a name="zh-cn_topic_0044524833_note21808274104217"></a><a name="zh-cn_topic_0044524833_note21808274104217"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0044524833_ul5307015718498"></a><a name="zh-cn_topic_0044524833_ul5307015718498"></a><ul id="zh-cn_topic_0044524833_ul5307015718498"><li><span id="zh-cn_topic_0044524833_text7492111913438"><a name="zh-cn_topic_0044524833_text7492111913438"></a><a name="zh-cn_topic_0044524833_text7492111913438"></a>从快照创建云硬盘时，volume_type字段必须和快照源云硬盘保持一致。</span></li><li>了解不同磁盘类型的详细信息，请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0044524691.html" target="_blank" rel="noopener noreferrer">磁盘类型及性能介绍</a>。</li></ul>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row7461047"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p365031"><a name="zh-cn_topic_0044524833_p365031"></a><a name="zh-cn_topic_0044524833_p365031"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p29567523"><a name="zh-cn_topic_0044524833_p29567523"></a><a name="zh-cn_topic_0044524833_p29567523"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p428797710293"><a name="zh-cn_topic_0044524833_p428797710293"></a><a name="zh-cn_topic_0044524833_p428797710293"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p47906786"><a name="zh-cn_topic_0044524833_p47906786"></a><a name="zh-cn_topic_0044524833_p47906786"></a>批量创云硬盘的个数。如果无该参数，表明只创建1个云硬盘，目前最多支持批量创建100个。</p>
    <p id="zh-cn_topic_0044524833_p9550502101436"><a name="zh-cn_topic_0044524833_p9550502101436"></a><a name="zh-cn_topic_0044524833_p9550502101436"></a>从备份创建云硬盘时，不支持批量创建，数量只能为<span class="parmname" id="zh-cn_topic_0044524833_parmname54941195437"><a name="zh-cn_topic_0044524833_parmname54941195437"></a><a name="zh-cn_topic_0044524833_parmname54941195437"></a>“1”</span>。</p>
    <div class="note" id="zh-cn_topic_0044524833_note57300341151148"><a name="zh-cn_topic_0044524833_note57300341151148"></a><a name="zh-cn_topic_0044524833_note57300341151148"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_zh-cn_topic_0044524833_p5070492815911"><a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_p5070492815911"></a><a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_p5070492815911"></a>如果发送请求时，将参数值设置为小数，则默认取小数点前的整数。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row2434599211437"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p1778734011437"><a name="zh-cn_topic_0044524833_p1778734011437"></a><a name="zh-cn_topic_0044524833_p1778734011437"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p3148844911437"><a name="zh-cn_topic_0044524833_p3148844911437"></a><a name="zh-cn_topic_0044524833_p3148844911437"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p42756211437"><a name="zh-cn_topic_0044524833_p42756211437"></a><a name="zh-cn_topic_0044524833_p42756211437"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p3463256011437"><a name="zh-cn_topic_0044524833_p3463256011437"></a><a name="zh-cn_topic_0044524833_p3463256011437"></a>是否为共享云硬盘。true为共享盘，false为普通云硬盘。</p>
    <div class="note" id="zh-cn_topic_0044524833_note3800959821323"><a name="zh-cn_topic_0044524833_note3800959821323"></a><a name="zh-cn_topic_0044524833_note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p45212589213213"><a name="zh-cn_topic_0044524833_p45212589213213"></a><a name="zh-cn_topic_0044524833_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row494599159816"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p424860529816"><a name="zh-cn_topic_0044524833_p424860529816"></a><a name="zh-cn_topic_0044524833_p424860529816"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p188182169816"><a name="zh-cn_topic_0044524833_p188182169816"></a><a name="zh-cn_topic_0044524833_p188182169816"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p478805289816"><a name="zh-cn_topic_0044524833_p478805289816"></a><a name="zh-cn_topic_0044524833_p478805289816"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p323873209920"><a name="zh-cn_topic_0044524833_p323873209920"></a><a name="zh-cn_topic_0044524833_p323873209920"></a>创建云硬盘的metadata信息，<span id="zh-cn_topic_0044524833_text149521944318"><a name="zh-cn_topic_0044524833_text149521944318"></a><a name="zh-cn_topic_0044524833_text149521944318"></a>metadata中的key和value长度不大于255个字节</span>。</p>
    <p id="zh-cn_topic_0044524833_p862801317585"><a name="zh-cn_topic_0044524833_p862801317585"></a><a name="zh-cn_topic_0044524833_p862801317585"></a>“metadata”字段信息说明请参见<a href="#li4145283210319">•metadata参数说明</a>，创建磁盘时仅支持表格中提供的字段。</p>
    <div class="note" id="zh-cn_topic_0044524833_note660019322131"><a name="zh-cn_topic_0044524833_note660019322131"></a><a name="zh-cn_topic_0044524833_note660019322131"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p1600173216137"><a name="zh-cn_topic_0044524833_p1600173216137"></a><a name="zh-cn_topic_0044524833_p1600173216137"></a>metadata里面不能有value为null的键值对。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row4752931910472"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p2466966510472"><a name="zh-cn_topic_0044524833_p2466966510472"></a><a name="zh-cn_topic_0044524833_p2466966510472"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p5208587610472"><a name="zh-cn_topic_0044524833_p5208587610472"></a><a name="zh-cn_topic_0044524833_p5208587610472"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p5820640710472"><a name="zh-cn_topic_0044524833_p5820640710472"></a><a name="zh-cn_topic_0044524833_p5820640710472"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><div class="p" id="zh-cn_topic_0044524833_p4531155053519"><a name="zh-cn_topic_0044524833_p4531155053519"></a><a name="zh-cn_topic_0044524833_p4531155053519"></a>创建共享云硬盘的信息。默认值为false。<a name="zh-cn_topic_0044524833_ul202952187368"></a><a name="zh-cn_topic_0044524833_ul202952187368"></a><ul id="zh-cn_topic_0044524833_ul202952187368"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    <p id="p96242024104913"><a name="p96242024104913"></a><a name="p96242024104913"></a>请参见<a href="https://support.huaweicloud.com/productdesc-evs/zh-cn_topic_0032860759.html" target="_blank" rel="noopener noreferrer">共享云硬盘及使用方法</a>了解更多信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row42399185112340"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p11781930112340"><a name="zh-cn_topic_0044524833_p11781930112340"></a><a name="zh-cn_topic_0044524833_p11781930112340"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p14812235112340"><a name="zh-cn_topic_0044524833_p14812235112340"></a><a name="zh-cn_topic_0044524833_p14812235112340"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p58940381112340"><a name="zh-cn_topic_0044524833_p58940381112340"></a><a name="zh-cn_topic_0044524833_p58940381112340"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="p7660174332112"><a name="p7660174332112"></a><a name="p7660174332112"></a>创建云硬盘的时候，给云硬盘绑定标签。</p>
    <p id="zh-cn_topic_0044524833_p41351845163840"><a name="zh-cn_topic_0044524833_p41351845163840"></a><a name="zh-cn_topic_0044524833_p41351845163840"></a>单个云硬盘最多可以创建10个标签。</p>
    <p id="zh-cn_topic_0044524833_p51240272203459"><a name="zh-cn_topic_0044524833_p51240272203459"></a><a name="zh-cn_topic_0044524833_p51240272203459"></a>标签的key需要唯一。重复的key会做去重操作，即如果有重复的key，最终只保留一个作为有效的标签。</p>
    <a name="zh-cn_topic_0044524833_ul3346152218352"></a><a name="zh-cn_topic_0044524833_ul3346152218352"></a><ul id="zh-cn_topic_0044524833_ul3346152218352"><li>标签的key：String类型，最大长度36个字符。<p id="zh-cn_topic_0044524833_p59057337203519"><a name="zh-cn_topic_0044524833_p59057337203519"></a><a name="zh-cn_topic_0044524833_p59057337203519"></a>由英文字母、数字、下划线、中划线、UNICODE字符（\u4E00-\u9FFF）组成。</p>
    </li><li>标签的value：String类型，最大长度43个字符，可以为空字符串。<p id="zh-cn_topic_0044524833_p46181786203545"><a name="zh-cn_topic_0044524833_p46181786203545"></a><a name="zh-cn_topic_0044524833_p46181786203545"></a>由英文字母、数字、下划线、点、中划线、UNICODE字符（\u4E00-\u9FFF）组成。</p>
    </li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0044524833_row179945620499"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0044524833_p39941261495"><a name="zh-cn_topic_0044524833_p39941261495"></a><a name="zh-cn_topic_0044524833_p39941261495"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0044524833_p1499413644915"><a name="zh-cn_topic_0044524833_p1499413644915"></a><a name="zh-cn_topic_0044524833_p1499413644915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0044524833_p79947634918"><a name="zh-cn_topic_0044524833_p79947634918"></a><a name="zh-cn_topic_0044524833_p79947634918"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49.494949494949495%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0044524833_p35013964916"><a name="zh-cn_topic_0044524833_p35013964916"></a><a name="zh-cn_topic_0044524833_p35013964916"></a>企业项目ID。创建云硬盘时，给云硬盘绑定企业项目ID。</p>
    <p id="zh-cn_topic_0044524833_p16244102205013"><a name="zh-cn_topic_0044524833_p16244102205013"></a><a name="zh-cn_topic_0044524833_p16244102205013"></a><span id="zh-cn_topic_0044524833_text98761511155218"><a name="zh-cn_topic_0044524833_text98761511155218"></a><a name="zh-cn_topic_0044524833_text98761511155218"></a>该参数不传，或者将该参数值设置为0，则将资源绑定给默认企业项目。</span></p>
    <div class="note" id="zh-cn_topic_0044524833_note16336122416016"><a name="zh-cn_topic_0044524833_note16336122416016"></a><a name="zh-cn_topic_0044524833_note16336122416016"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0044524833_p18336524404"><a name="zh-cn_topic_0044524833_p18336524404"></a><a name="zh-cn_topic_0044524833_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >不支持同时使用“backup\_id“、“snapshot\_id“和“imageRef“这三个字段中的任意两个。  

-   <a name="li4145283210319"></a>metadata参数说明

    <a name="table3430728295554"></a>
    <table><thead align="left"><tr id="row4496975195554"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p13311011464"><a name="p13311011464"></a><a name="p13311011464"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="p63354117469"><a name="p63354117469"></a><a name="p63354117469"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p163394117462"><a name="p163394117462"></a><a name="p163394117462"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47%" id="mcps1.1.5.1.4"><p id="p1834412114464"><a name="p1834412114464"></a><a name="p1834412114464"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row456195295554"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p1562408795622"><a name="p1562408795622"></a><a name="p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p5759155095622"><a name="p5759155095622"></a><a name="p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p3440400295622"><a name="p3440400295622"></a><a name="p3440400295622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p729227516614"><a name="p729227516614"></a><a name="p729227516614"></a>metadata中的表示加密功能的字段，0代表不加密，1代表加密。</p>
    <p id="p3526077895622"><a name="p3526077895622"></a><a name="p3526077895622"></a>该字段不存在时，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="row247050109562"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p241272995622"><a name="p241272995622"></a><a name="p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p6121338895622"><a name="p6121338895622"></a><a name="p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p5933737595622"><a name="p5933737595622"></a><a name="p5933737595622"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p4159804295622"><a name="p4159804295622"></a><a name="p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    <div class="note" id="note1483983117491"><a name="note1483983117491"></a><a name="note1483983117491"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p093935613512"><a name="evs_04_2013_p093935613512"></a><a name="evs_04_2013_p093935613512"></a>请参考<a href="https://support.huaweicloud.com/api-dew/dew_02_0017.html" target="_blank" rel="noopener noreferrer">查询密钥列表</a>，通过HTTPS请求获取密钥ID。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row60499086104915"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p1478896104915"><a name="p1478896104915"></a><a name="p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p52681767104915"><a name="p52681767104915"></a><a name="p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p39364763104915"><a name="p39364763104915"></a><a name="p39364763104915"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><a name="ul14462208141855"></a><a name="ul14462208141855"></a><ul id="ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD (虚拟块存储设备 , Virtual Block Device)类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </td>
    </tr>
    <tr id="row416151612311"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p3500156018292"><a name="p3500156018292"></a><a name="p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p1655411118292"><a name="p1655411118292"></a><a name="p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p6581460618292"><a name="p6581460618292"></a><a name="p6581460618292"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p47931946183150"><a name="p47931946183150"></a><a name="p47931946183150"></a>从快照创建云硬盘时，如需使用link克隆方式，请指定该字段的值为0。</p>
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

-   <a name="li5068387212423"></a>bssParam参数说明

    <a name="table507504371244"></a>
    <table><thead align="left"><tr id="row408191331244"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p923218148465"><a name="p923218148465"></a><a name="p923218148465"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="p122351014204616"><a name="p122351014204616"></a><a name="p122351014204616"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p023913142467"><a name="p023913142467"></a><a name="p023913142467"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="46%" id="mcps1.1.5.1.4"><p id="p20242191410468"><a name="p20242191410468"></a><a name="p20242191410468"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row652253961244"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p3445611112459"><a name="p3445611112459"></a><a name="p3445611112459"></a>chargingMode</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p3948157412459"><a name="p3948157412459"></a><a name="p3948157412459"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p4389094612459"><a name="p4389094612459"></a><a name="p4389094612459"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="ul2359814014196"></a><a name="ul2359814014196"></a><ul id="ul2359814014196"><li>功能说明：计费模式。默认值为postPaid。</li><li>取值范围<a name="ul4699861141915"></a><a name="ul4699861141915"></a><ul id="ul4699861141915"><li>prePaid：包年包月</li><li>postPaid：按需</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row324660391244"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p1087084814205"><a name="p1087084814205"></a><a name="p1087084814205"></a>periodType</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p812348714205"><a name="p812348714205"></a><a name="p812348714205"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p5402273514205"><a name="p5402273514205"></a><a name="p5402273514205"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="ul55261761142112"></a><a name="ul55261761142112"></a><ul id="ul55261761142112"><li>功能说明：订购周期单位。chargingMode为prePaid时该参数会生效，并且该参数为必选。</li><li>取值范围<a name="ul37826664142140"></a><a name="ul37826664142140"></a><ul id="ul37826664142140"><li>month：月</li><li>year：年</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row433612671244"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p55385490142235"><a name="p55385490142235"></a><a name="p55385490142235"></a>periodNum</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p57039715142235"><a name="p57039715142235"></a><a name="p57039715142235"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p56814204142235"><a name="p56814204142235"></a><a name="p56814204142235"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="ul11347758142255"></a><a name="ul11347758142255"></a><ul id="ul11347758142255"><li>功能说明：订购周期数，chargingMode为prePaid时该参数会生效，并且该参数为必选。</li><li>取值范围<a name="ul2552699014236"></a><a name="ul2552699014236"></a><ul id="ul2552699014236"><li>periodType为month时，为[1-9]</li><li>periodType为year时，为[1-1]</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row149642211244"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p6694695014241"><a name="p6694695014241"></a><a name="p6694695014241"></a>isAutoPay</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p5399388714241"><a name="p5399388714241"></a><a name="p5399388714241"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p1142869614241"><a name="p1142869614241"></a><a name="p1142869614241"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="ul5467976142421"></a><a name="ul5467976142421"></a><ul id="ul5467976142421"><li>功能说明：是否立即支付。chargingMode为PrePaid时该参数会生效。默认值为false。</li><li>取值范围<a name="ul65615094142430"></a><a name="ul65615094142430"></a><ul id="ul65615094142430"><li>false：不立即支付，创建订单暂不支付</li><li>true：立即支付，从帐户余额中自动扣费</li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="row17825308142513"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p15317605142523"><a name="p15317605142523"></a><a name="p15317605142523"></a>isAutoRenew</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p32766517142523"><a name="p32766517142523"></a><a name="p32766517142523"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p36842238142523"><a name="p36842238142523"></a><a name="p36842238142523"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="46%" headers="mcps1.1.5.1.4 "><a name="ul36539029142528"></a><a name="ul36539029142528"></a><ul id="ul36539029142528"><li>功能说明：是否自动续订。chargingMode为prePaid时该参数会生效。默认值为false。</li><li>取值范围<a name="ul43109644142559"></a><a name="ul43109644142559"></a><ul id="ul43109644142559"><li>false：不自动续订</li><li>true：自动续订，自动续订周期与订购周期相同</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "volume": {
            "name": "test_volume_3", 
            "availability_zone": "az-dc-1", 
            "volume_type": "SATA", 
            "size": 120, 
            "description": "hehehe", 
            "multiattach": true, 
            "count": 1
        }, 
        "bssParam": {
            "chargingMode": "prePaid", 
            "periodType": "year", 
            "periodNum": 1, 
            "isAutoPay": "true", 
            "isAutoRenew": "true"
        }
    }
    ```


## 响应消息<a name="section38285619"></a>

-   响应参数

    <a name="table15441099103019"></a>
    <table><thead align="left"><tr id="row54094047103019"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="p19541716103019"><a name="p19541716103019"></a><a name="p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p39375186103019"><a name="p39375186103019"></a><a name="p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="p38578950103019"><a name="p38578950103019"></a><a name="p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row11712103111213"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p33545583319"><a name="p33545583319"></a><a name="p33545583319"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p19354165810317"><a name="p19354165810317"></a><a name="p19354165810317"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p435416581936"><a name="p435416581936"></a><a name="p435416581936"></a>任务ID，创建按需云硬盘时返回该参数。</p>
    <div class="note" id="note335410589314"><a name="note335410589314"></a><a name="note335410589314"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1435514588312"><a name="p1435514588312"></a><a name="p1435514588312"></a>如果需要查询job的状态，请参考<a href="查询job的状态.md">查询job的状态</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row11017750143220"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p24400321143233"><a name="p24400321143233"></a><a name="p24400321143233"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p30268984143233"><a name="p30268984143233"></a><a name="p30268984143233"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p19678023143233"><a name="p19678023143233"></a><a name="p19678023143233"></a>订单号，创建包周期云硬盘时返回该参数。</p>
    <div class="note" id="note118971174719"><a name="note118971174719"></a><a name="note118971174719"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul869315108377"></a><a name="ul869315108377"></a><ul id="ul869315108377"><li>如果您需要支付订单，请参考<a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">支付包周期产品订单</a>。</li><li>如果您需要查询订单的资源开通详情，请参考<a href="https://support.huaweicloud.com/api-oce/api_order_00001.html" target="_blank" rel="noopener noreferrer">查询订单的资源开通详情</a>。</li><li>如果您需要退订该包周期资源，请参考“<a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">退订包周期资源</a>”。</li></ul>
    </div></div>
    </td>
    </tr>
    <tr id="row45731334253"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
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
        "job_id": "70a599e0-31e7-49b7-b260-868f441e862b"
    }
    ```

    或

    ```
    {
        "order_id": "CS1711152257C60TL"
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


## 状态码<a name="section9026257"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

