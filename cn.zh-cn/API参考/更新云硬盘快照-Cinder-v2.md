# 更新云硬盘快照<a name="ZH-CN_TOPIC_0058626631"></a>

## 功能介绍<a name="section4805694511340"></a>

更新云硬盘快照。

## URI<a name="section268627411340"></a>

-   URI格式

    PUT /v2/\{project\_id\}/snapshots/\{snapshot\_id\}

-   参数说明

    <a name="table5655293911340"></a>
    <table><thead align="left"><tr id="row4718979611340"><th class="cellrowborder" valign="top" width="28.54%" id="mcps1.1.4.1.1"><p id="p6427715211340"><a name="p6427715211340"></a><a name="p6427715211340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.56%" id="mcps1.1.4.1.2"><p id="p3906685711340"><a name="p3906685711340"></a><a name="p3906685711340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1029885411340"><a name="p1029885411340"></a><a name="p1029885411340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2890086411340"><td class="cellrowborder" valign="top" width="28.54%" headers="mcps1.1.4.1.1 "><p id="p5926863811340"><a name="p5926863811340"></a><a name="p5926863811340"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.56%" headers="mcps1.1.4.1.2 "><p id="p3603037711340"><a name="p3603037711340"></a><a name="p3603037711340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p3277940011340"><a name="p3277940011340"></a><a name="p3277940011340"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row2657914711340"><td class="cellrowborder" valign="top" width="28.54%" headers="mcps1.1.4.1.1 "><p id="p542726811340"><a name="p542726811340"></a><a name="p542726811340"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.56%" headers="mcps1.1.4.1.2 "><p id="p3695552511340"><a name="p3695552511340"></a><a name="p3695552511340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4060754311340"><a name="p4060754311340"></a><a name="p4060754311340"></a>快照ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section87667311340"></a>

-   请求参数

    <a name="table16590896104128"></a>
    <table><thead align="left"><tr id="row60389002104128"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p59671014104128"><a name="p59671014104128"></a><a name="p59671014104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p1513999104128"><a name="p1513999104128"></a><a name="p1513999104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="p55525100104128"><a name="p55525100104128"></a><a name="p55525100104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.1.5.1.4"><p id="p1239270104128"><a name="p1239270104128"></a><a name="p1239270104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row49575616223342"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p26354398223356"><a name="p26354398223356"></a><a name="p26354398223356"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p54331513223356"><a name="p54331513223356"></a><a name="p54331513223356"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p38776445223356"><a name="p38776445223356"></a><a name="p38776445223356"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="p53884304223356"><a name="p53884304223356"></a><a name="p53884304223356"></a>待更新的快照信息。</p>
    </td>
    </tr>
    <tr id="row33272036104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p43959720162736"><a name="p43959720162736"></a><a name="p43959720162736"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p3967568162736"><a name="p3967568162736"></a><a name="p3967568162736"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p52937605162736"><a name="p52937605162736"></a><a name="p52937605162736"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="p60087598162736"><a name="p60087598162736"></a><a name="p60087598162736"></a>云硬盘快照名称。<span id="text464413115259"><a name="text464413115259"></a><a name="text464413115259"></a>最大支持255个字节。</span></p>
    <div class="note" id="note154651827114612"><a name="note154651827114612"></a><a name="note154651827114612"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0051408624_p46767097103214"><a name="zh-cn_topic_0051408624_p46767097103214"></a><a name="zh-cn_topic_0051408624_p46767097103214"></a>通过VBS对云硬盘创建备份时，同时会创建以autobk_snapshot_为名称前缀的快照，云硬盘控制台对此类快照会有操作限制。因此建议不要创建以autobk_snapshot_为名称前缀的快照，避免影响快照的正常使用。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row12756475104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p48879957162736"><a name="p48879957162736"></a><a name="p48879957162736"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p66962416162736"><a name="p66962416162736"></a><a name="p66962416162736"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p55246620162736"><a name="p55246620162736"></a><a name="p55246620162736"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="p45791232162736"><a name="p45791232162736"></a><a name="p45791232162736"></a>云硬盘快照描述。<span id="text40796911152514"><a name="text40796911152514"></a><a name="text40796911152514"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row26493997162819"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p12659426162825"><a name="p12659426162825"></a><a name="p12659426162825"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p18780582162825"><a name="p18780582162825"></a><a name="p18780582162825"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p44832203162825"><a name="p44832203162825"></a><a name="p44832203162825"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="p7529849162825"><a name="p7529849162825"></a><a name="p7529849162825"></a>同name，name和display_name任意指定一个即可（若两个都指定，则以name为主）。<span id="text13486246152521"><a name="text13486246152521"></a><a name="text13486246152521"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row40792854162816"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p53442063162825"><a name="p53442063162825"></a><a name="p53442063162825"></a>display_description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p33839865162825"><a name="p33839865162825"></a><a name="p33839865162825"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p56674535162825"><a name="p56674535162825"></a><a name="p56674535162825"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="p27234626162825"><a name="p27234626162825"></a><a name="p27234626162825"></a>同description，description和display_ description任意指定一个即可。<span id="text22531078152526"><a name="text22531078152526"></a><a name="text22531078152526"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "snapshot": {
            "name": "name_xx3", 
            "description": "hello"
        }
    }
    ```


## 响应<a name="section5147449911340"></a>

-   响应参数

    <a name="table251963102518"></a>
    <table><thead align="left"><tr id="row18517183132513"><th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.1"><p id="p17515931252"><a name="p17515931252"></a><a name="p17515931252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.2"><p id="p7515173192517"><a name="p7515173192517"></a><a name="p7515173192517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.24467553244675%" id="mcps1.1.4.1.3"><p id="p05179317252"><a name="p05179317252"></a><a name="p05179317252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row551719372519"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p135171634254"><a name="p135171634254"></a><a name="p135171634254"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p55178310254"><a name="p55178310254"></a><a name="p55178310254"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p551733112512"><a name="p551733112512"></a><a name="p551733112512"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="row351716312517"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p8517838253"><a name="p8517838253"></a><a name="p8517838253"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p125173352512"><a name="p125173352512"></a><a name="p125173352512"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p1251783102517"><a name="p1251783102517"></a><a name="p1251783102517"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row451813317253"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1451818312254"><a name="p1451818312254"></a><a name="p1451818312254"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p115184372510"><a name="p115184372510"></a><a name="p115184372510"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p151812362515"><a name="p151812362515"></a><a name="p151812362515"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row16518132257"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1051853182512"><a name="p1051853182512"></a><a name="p1051853182512"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p205185362515"><a name="p205185362515"></a><a name="p205185362515"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p1651863172513"><a name="p1651863172513"></a><a name="p1651863172513"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row5518163152514"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1751813313259"><a name="p1751813313259"></a><a name="p1751813313259"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p155189382519"><a name="p155189382519"></a><a name="p155189382519"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p165181362512"><a name="p165181362512"></a><a name="p165181362512"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row5518137256"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p125182382518"><a name="p125182382518"></a><a name="p125182382518"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p951813311252"><a name="p951813311252"></a><a name="p951813311252"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p115181317254"><a name="p115181317254"></a><a name="p115181317254"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="row10519133253"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1951843112514"><a name="p1951843112514"></a><a name="p1951843112514"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p13519163112515"><a name="p13519163112515"></a><a name="p13519163112515"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p251915313258"><a name="p251915313258"></a><a name="p251915313258"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="row165197362511"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1451913102511"><a name="p1451913102511"></a><a name="p1451913102511"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p1351963112514"><a name="p1351963112514"></a><a name="p1351963112514"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p551913316258"><a name="p551913316258"></a><a name="p551913316258"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row10519163192515"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1351923142514"><a name="p1351923142514"></a><a name="p1351923142514"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p65190317252"><a name="p65190317252"></a><a name="p65190317252"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p1451963122512"><a name="p1451963122512"></a><a name="p1451963122512"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="row25191735255"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="p1951903192520"><a name="p1951903192520"></a><a name="p1951903192520"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="p165198313255"><a name="p165198313255"></a><a name="p165198313255"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="p95191639256"><a name="p95191639256"></a><a name="p95191639256"></a>云硬盘快照更新时间。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "snapshot": {
            "status": "creating", 
            "description": "Daily backup", 
            "created_at": "2013-02-25T03:56:53.081642", 
            "metadata": { }, 
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635", 
            "size": 1, 
            "id": "f9faf7df-fdc1-4093-9ef3-5cba06eef995", 
            "name": "snap-001", 
            "updated_at": "2013-02-25T03:56:53.081642"
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

    ```
    {
        "itemNotFound": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 返回值<a name="section1751558211340"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

