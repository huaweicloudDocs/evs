# 更新云硬盘快照<a name="evs_04_3058"></a>

## 功能介绍<a name="section4805694511340"></a>

更新云硬盘快照。

## URI<a name="section268627411340"></a>

-   URI格式

    PUT /v3/\{project\_id\}/snapshots/\{snapshot\_id\}

-   参数说明

    <a name="table5655293911340"></a>
    <table><thead align="left"><tr id="row4718979611340"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p6427715211340"><a name="p6427715211340"></a><a name="p6427715211340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p3906685711340"><a name="p3906685711340"></a><a name="p3906685711340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1029885411340"><a name="p1029885411340"></a><a name="p1029885411340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2890086411340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p5926863811340"><a name="p5926863811340"></a><a name="p5926863811340"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3603037711340"><a name="p3603037711340"></a><a name="p3603037711340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p3277940011340"><a name="p3277940011340"></a><a name="p3277940011340"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row2657914711340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p542726811340"><a name="p542726811340"></a><a name="p542726811340"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3695552511340"><a name="p3695552511340"></a><a name="p3695552511340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4060754311340"><a name="p4060754311340"></a><a name="p4060754311340"></a>快照ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section87667311340"></a>

-   请求参数

    <a name="evs_04_2095_table741545961616"></a>
    <table><thead align="left"><tr id="evs_04_2095_row8415125912161"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2095_p15415175914166"><a name="evs_04_2095_p15415175914166"></a><a name="evs_04_2095_p15415175914166"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2095_p16415155919169"><a name="evs_04_2095_p16415155919169"></a><a name="evs_04_2095_p16415155919169"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="evs_04_2095_p1741511599167"><a name="evs_04_2095_p1741511599167"></a><a name="evs_04_2095_p1741511599167"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.1.5.1.4"><p id="evs_04_2095_p7415059161614"><a name="evs_04_2095_p7415059161614"></a><a name="evs_04_2095_p7415059161614"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2095_row3416259191613"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2095_p16416195961611"><a name="evs_04_2095_p16416195961611"></a><a name="evs_04_2095_p16416195961611"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2095_p94161059141619"><a name="evs_04_2095_p94161059141619"></a><a name="evs_04_2095_p94161059141619"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="evs_04_2095_p841615914166"><a name="evs_04_2095_p841615914166"></a><a name="evs_04_2095_p841615914166"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="evs_04_2095_p15416155911161"><a name="evs_04_2095_p15416155911161"></a><a name="evs_04_2095_p15416155911161"></a>待更新的快照信息，请参见<a href="#evs_04_2095_li143506387236">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2095_li143506387236"></a>snapshot参数说明

    <a name="evs_04_2095_table16590896104128"></a>
    <table><thead align="left"><tr id="evs_04_2095_row60389002104128"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2095_p59671014104128"><a name="evs_04_2095_p59671014104128"></a><a name="evs_04_2095_p59671014104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2095_p1513999104128"><a name="evs_04_2095_p1513999104128"></a><a name="evs_04_2095_p1513999104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="evs_04_2095_p55525100104128"><a name="evs_04_2095_p55525100104128"></a><a name="evs_04_2095_p55525100104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="42%" id="mcps1.1.5.1.4"><p id="evs_04_2095_p1239270104128"><a name="evs_04_2095_p1239270104128"></a><a name="evs_04_2095_p1239270104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2095_row33272036104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2095_p43959720162736"><a name="evs_04_2095_p43959720162736"></a><a name="evs_04_2095_p43959720162736"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2095_p3967568162736"><a name="evs_04_2095_p3967568162736"></a><a name="evs_04_2095_p3967568162736"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="evs_04_2095_p52937605162736"><a name="evs_04_2095_p52937605162736"></a><a name="evs_04_2095_p52937605162736"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="evs_04_2095_p60087598162736"><a name="evs_04_2095_p60087598162736"></a><a name="evs_04_2095_p60087598162736"></a>云硬盘快照名称。<span id="evs_04_2095_text464413115259"><a name="evs_04_2095_text464413115259"></a><a name="evs_04_2095_text464413115259"></a>最大支持255个字节。</span></p>
    <div class="note" id="evs_04_2095_note154651827114612"><a name="evs_04_2095_note154651827114612"></a><a name="evs_04_2095_note154651827114612"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2095_evs_04_2093_p46767097103214"><a name="evs_04_2095_evs_04_2093_p46767097103214"></a><a name="evs_04_2095_evs_04_2093_p46767097103214"></a>对云硬盘创建备份时，同时会创建以autobk_snapshot_为名称前缀的快照，云硬盘控制台对此类快照会有操作限制。因此建议不要创建以autobk_snapshot_为名称前缀的快照，避免影响快照的正常使用。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2095_row12756475104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2095_p48879957162736"><a name="evs_04_2095_p48879957162736"></a><a name="evs_04_2095_p48879957162736"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2095_p66962416162736"><a name="evs_04_2095_p66962416162736"></a><a name="evs_04_2095_p66962416162736"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="evs_04_2095_p55246620162736"><a name="evs_04_2095_p55246620162736"></a><a name="evs_04_2095_p55246620162736"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="42%" headers="mcps1.1.5.1.4 "><p id="evs_04_2095_p45791232162736"><a name="evs_04_2095_p45791232162736"></a><a name="evs_04_2095_p45791232162736"></a>云硬盘快照描述。<span id="evs_04_2095_text40796911152514"><a name="evs_04_2095_text40796911152514"></a><a name="evs_04_2095_text40796911152514"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "snapshot": {
            "name": "snap-001", 
            "description": "Daily backup"
        }
    }
    ```


## 响应消息<a name="section5147449911340"></a>

-   响应参数

    <a name="evs_04_2095_table5724531817"></a>
    <table><thead align="left"><tr id="evs_04_2095_row473553186"><th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.1"><p id="evs_04_2095_p1373105313817"><a name="evs_04_2095_p1373105313817"></a><a name="evs_04_2095_p1373105313817"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.2"><p id="evs_04_2095_p11731053784"><a name="evs_04_2095_p11731053784"></a><a name="evs_04_2095_p11731053784"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.24467553244675%" id="mcps1.1.4.1.3"><p id="evs_04_2095_p4736536811"><a name="evs_04_2095_p4736536811"></a><a name="evs_04_2095_p4736536811"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2095_row197316531287"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p18731553886"><a name="evs_04_2095_p18731553886"></a><a name="evs_04_2095_p18731553886"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p14731953385"><a name="evs_04_2095_p14731953385"></a><a name="evs_04_2095_p14731953385"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p3731053387"><a name="evs_04_2095_p3731053387"></a><a name="evs_04_2095_p3731053387"></a>快照信息，请参见<a href="#evs_04_2095_li8366143102514">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row9804140716"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p129522216412"><a name="evs_04_2095_p129522216412"></a><a name="evs_04_2095_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p1595262111415"><a name="evs_04_2095_p1595262111415"></a><a name="evs_04_2095_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p109527215417"><a name="evs_04_2095_p109527215417"></a><a name="evs_04_2095_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2095_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2095_li8366143102514"></a>snapshot参数说明

    <a name="evs_04_2095_table251963102518"></a>
    <table><thead align="left"><tr id="evs_04_2095_row18517183132513"><th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.1"><p id="evs_04_2095_p17515931252"><a name="evs_04_2095_p17515931252"></a><a name="evs_04_2095_p17515931252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.2"><p id="evs_04_2095_p7515173192517"><a name="evs_04_2095_p7515173192517"></a><a name="evs_04_2095_p7515173192517"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.24467553244675%" id="mcps1.1.4.1.3"><p id="evs_04_2095_p05179317252"><a name="evs_04_2095_p05179317252"></a><a name="evs_04_2095_p05179317252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2095_row351716312517"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p8517838253"><a name="evs_04_2095_p8517838253"></a><a name="evs_04_2095_p8517838253"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p125173352512"><a name="evs_04_2095_p125173352512"></a><a name="evs_04_2095_p125173352512"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p1251783102517"><a name="evs_04_2095_p1251783102517"></a><a name="evs_04_2095_p1251783102517"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row451813317253"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1451818312254"><a name="evs_04_2095_p1451818312254"></a><a name="evs_04_2095_p1451818312254"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p115184372510"><a name="evs_04_2095_p115184372510"></a><a name="evs_04_2095_p115184372510"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p151812362515"><a name="evs_04_2095_p151812362515"></a><a name="evs_04_2095_p151812362515"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row16518132257"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1051853182512"><a name="evs_04_2095_p1051853182512"></a><a name="evs_04_2095_p1051853182512"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p205185362515"><a name="evs_04_2095_p205185362515"></a><a name="evs_04_2095_p205185362515"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p1651863172513"><a name="evs_04_2095_p1651863172513"></a><a name="evs_04_2095_p1651863172513"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row5518163152514"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1751813313259"><a name="evs_04_2095_p1751813313259"></a><a name="evs_04_2095_p1751813313259"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p155189382519"><a name="evs_04_2095_p155189382519"></a><a name="evs_04_2095_p155189382519"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p165181362512"><a name="evs_04_2095_p165181362512"></a><a name="evs_04_2095_p165181362512"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row5518137256"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p125182382518"><a name="evs_04_2095_p125182382518"></a><a name="evs_04_2095_p125182382518"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p951813311252"><a name="evs_04_2095_p951813311252"></a><a name="evs_04_2095_p951813311252"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p115181317254"><a name="evs_04_2095_p115181317254"></a><a name="evs_04_2095_p115181317254"></a>云硬盘快照创建时间。</p>
    <p id="evs_04_2095_p10500514493"><a name="evs_04_2095_p10500514493"></a><a name="evs_04_2095_p10500514493"></a><span id="evs_04_2095_text859662881020"><a name="evs_04_2095_text859662881020"></a><a name="evs_04_2095_text859662881020"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2095_row10519133253"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1951843112514"><a name="evs_04_2095_p1951843112514"></a><a name="evs_04_2095_p1951843112514"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p13519163112515"><a name="evs_04_2095_p13519163112515"></a><a name="evs_04_2095_p13519163112515"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p251915313258"><a name="evs_04_2095_p251915313258"></a><a name="evs_04_2095_p251915313258"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row165197362511"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1451913102511"><a name="evs_04_2095_p1451913102511"></a><a name="evs_04_2095_p1451913102511"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p1351963112514"><a name="evs_04_2095_p1351963112514"></a><a name="evs_04_2095_p1351963112514"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p551913316258"><a name="evs_04_2095_p551913316258"></a><a name="evs_04_2095_p551913316258"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row10519163192515"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1351923142514"><a name="evs_04_2095_p1351923142514"></a><a name="evs_04_2095_p1351923142514"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p65190317252"><a name="evs_04_2095_p65190317252"></a><a name="evs_04_2095_p65190317252"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p1451963122512"><a name="evs_04_2095_p1451963122512"></a><a name="evs_04_2095_p1451963122512"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_row25191735255"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_p1951903192520"><a name="evs_04_2095_p1951903192520"></a><a name="evs_04_2095_p1951903192520"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_p165198313255"><a name="evs_04_2095_p165198313255"></a><a name="evs_04_2095_p165198313255"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_p95191639256"><a name="evs_04_2095_p95191639256"></a><a name="evs_04_2095_p95191639256"></a>云硬盘快照上次更新时间。</p>
    <p id="evs_04_2095_p972113371011"><a name="evs_04_2095_p972113371011"></a><a name="evs_04_2095_p972113371011"></a><span id="evs_04_2095_text140163851010"><a name="evs_04_2095_text140163851010"></a><a name="evs_04_2095_text140163851010"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2095_li0419202382514"></a>error参数说明

    <a name="evs_04_2095_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2095_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2095_evs_04_2013_p19541716103019"><a name="evs_04_2095_evs_04_2013_p19541716103019"></a><a name="evs_04_2095_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2095_evs_04_2013_p39375186103019"><a name="evs_04_2095_evs_04_2013_p39375186103019"></a><a name="evs_04_2095_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2095_evs_04_2013_p38578950103019"><a name="evs_04_2095_evs_04_2013_p38578950103019"></a><a name="evs_04_2095_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2095_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_evs_04_2013_p46815658103019"><a name="evs_04_2095_evs_04_2013_p46815658103019"></a><a name="evs_04_2095_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_evs_04_2013_p33971979103019"><a name="evs_04_2095_evs_04_2013_p33971979103019"></a><a name="evs_04_2095_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_evs_04_2013_p21623243103019"><a name="evs_04_2095_evs_04_2013_p21623243103019"></a><a name="evs_04_2095_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2095_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2095_evs_04_2013_p59870541103019"><a name="evs_04_2095_evs_04_2013_p59870541103019"></a><a name="evs_04_2095_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2095_evs_04_2013_p17675690103019"><a name="evs_04_2095_evs_04_2013_p17675690103019"></a><a name="evs_04_2095_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2095_evs_04_2013_p6087468103019"><a name="evs_04_2095_evs_04_2013_p6087468103019"></a><a name="evs_04_2095_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2095_evs_04_2013_p54787218103019"><a name="evs_04_2095_evs_04_2013_p54787218103019"></a><a name="evs_04_2095_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "snapshot": {
            "status": "available", 
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


## 状态码<a name="section1751558211340"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

