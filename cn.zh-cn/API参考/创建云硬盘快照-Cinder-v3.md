# 创建云硬盘快照<a name="ZH-CN_TOPIC_0102674799"></a>

## 功能介绍<a name="section17386310104128"></a>

创建云硬盘快照。

## URI<a name="section48475837104128"></a>

-   URI格式

    POST /v3/\{project\_id\}/snapshots

-   参数说明

    <a name="table28484833104128"></a>
    <table><thead align="left"><tr id="row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p5384679104128"><a name="p5384679104128"></a><a name="p5384679104128"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p33505894104128"><a name="p33505894104128"></a><a name="p33505894104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p29622926104128"><a name="p29622926104128"></a><a name="p29622926104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50646790104128"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p8749302104128"><a name="p8749302104128"></a><a name="p8749302104128"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p37604871104128"><a name="p37604871104128"></a><a name="p37604871104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p26095712104128"><a name="p26095712104128"></a><a name="p26095712104128"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section33377962104128"></a>

-   请求参数

    <a name="zh-cn_topic_0051408624_table16590896104128"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408624_row60389002104128"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0051408624_p59671014104128"><a name="zh-cn_topic_0051408624_p59671014104128"></a><a name="zh-cn_topic_0051408624_p59671014104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0051408624_p1513999104128"><a name="zh-cn_topic_0051408624_p1513999104128"></a><a name="zh-cn_topic_0051408624_p1513999104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0051408624_p55525100104128"><a name="zh-cn_topic_0051408624_p55525100104128"></a><a name="zh-cn_topic_0051408624_p55525100104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0051408624_p1239270104128"><a name="zh-cn_topic_0051408624_p1239270104128"></a><a name="zh-cn_topic_0051408624_p1239270104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408624_row33272036104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p10680399104128"><a name="zh-cn_topic_0051408624_p10680399104128"></a><a name="zh-cn_topic_0051408624_p10680399104128"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p59805966104128"><a name="zh-cn_topic_0051408624_p59805966104128"></a><a name="zh-cn_topic_0051408624_p59805966104128"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p12445066104128"><a name="zh-cn_topic_0051408624_p12445066104128"></a><a name="zh-cn_topic_0051408624_p12445066104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p1417386104128"><a name="zh-cn_topic_0051408624_p1417386104128"></a><a name="zh-cn_topic_0051408624_p1417386104128"></a>待创建的快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row12756475104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p26641549104128"><a name="zh-cn_topic_0051408624_p26641549104128"></a><a name="zh-cn_topic_0051408624_p26641549104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p10481847104128"><a name="zh-cn_topic_0051408624_p10481847104128"></a><a name="zh-cn_topic_0051408624_p10481847104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p43723298104128"><a name="zh-cn_topic_0051408624_p43723298104128"></a><a name="zh-cn_topic_0051408624_p43723298104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p51926262104128"><a name="zh-cn_topic_0051408624_p51926262104128"></a><a name="zh-cn_topic_0051408624_p51926262104128"></a>创建快照源云硬盘UUID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row64683174104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p4845737104128"><a name="zh-cn_topic_0051408624_p4845737104128"></a><a name="zh-cn_topic_0051408624_p4845737104128"></a>force</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p56960425104128"><a name="zh-cn_topic_0051408624_p56960425104128"></a><a name="zh-cn_topic_0051408624_p56960425104128"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p50391693104128"><a name="zh-cn_topic_0051408624_p50391693104128"></a><a name="zh-cn_topic_0051408624_p50391693104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p32530251113919"><a name="zh-cn_topic_0051408624_p32530251113919"></a><a name="zh-cn_topic_0051408624_p32530251113919"></a>强制创快照标示，默认为false。</p>
    <a name="zh-cn_topic_0051408624_ul60750582141455"></a><a name="zh-cn_topic_0051408624_ul60750582141455"></a><ul id="zh-cn_topic_0051408624_ul60750582141455"><li>当force标记为false时，云硬盘处于挂载状态时，不能强制创建快照。</li><li>当force标记为true时，即使云硬盘处于挂载状态时，仍可以创建快照。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row26995886104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p39183164104128"><a name="zh-cn_topic_0051408624_p39183164104128"></a><a name="zh-cn_topic_0051408624_p39183164104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p19719755104128"><a name="zh-cn_topic_0051408624_p19719755104128"></a><a name="zh-cn_topic_0051408624_p19719755104128"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p53796355104128"><a name="zh-cn_topic_0051408624_p53796355104128"></a><a name="zh-cn_topic_0051408624_p53796355104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p62537483104128"><a name="zh-cn_topic_0051408624_p62537483104128"></a><a name="zh-cn_topic_0051408624_p62537483104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row25966436104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p22906600104128"><a name="zh-cn_topic_0051408624_p22906600104128"></a><a name="zh-cn_topic_0051408624_p22906600104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p43495312104128"><a name="zh-cn_topic_0051408624_p43495312104128"></a><a name="zh-cn_topic_0051408624_p43495312104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p33459397104128"><a name="zh-cn_topic_0051408624_p33459397104128"></a><a name="zh-cn_topic_0051408624_p33459397104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p25856622104128"><a name="zh-cn_topic_0051408624_p25856622104128"></a><a name="zh-cn_topic_0051408624_p25856622104128"></a>云硬盘快照描述，可以为null。<span id="zh-cn_topic_0051408624_text59690989152428"><a name="zh-cn_topic_0051408624_text59690989152428"></a><a name="zh-cn_topic_0051408624_text59690989152428"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row31383010104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408624_p58995861104128"><a name="zh-cn_topic_0051408624_p58995861104128"></a><a name="zh-cn_topic_0051408624_p58995861104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408624_p13935408104128"><a name="zh-cn_topic_0051408624_p13935408104128"></a><a name="zh-cn_topic_0051408624_p13935408104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408624_p55026268104128"><a name="zh-cn_topic_0051408624_p55026268104128"></a><a name="zh-cn_topic_0051408624_p55026268104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408624_p27942720104128"><a name="zh-cn_topic_0051408624_p27942720104128"></a><a name="zh-cn_topic_0051408624_p27942720104128"></a>云硬盘快照名称。<span id="zh-cn_topic_0051408624_text26279838152439"><a name="zh-cn_topic_0051408624_text26279838152439"></a><a name="zh-cn_topic_0051408624_text26279838152439"></a>最大支持255个字节。</span></p>
    <div class="note" id="zh-cn_topic_0051408624_note12652884103214"><a name="zh-cn_topic_0051408624_note12652884103214"></a><a name="zh-cn_topic_0051408624_note12652884103214"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0051408624_p46767097103214"><a name="zh-cn_topic_0051408624_p46767097103214"></a><a name="zh-cn_topic_0051408624_p46767097103214"></a>通过VBS对云硬盘创建备份时，同时会创建以autobk_snapshot_为名称前缀的快照，云硬盘控制台对此类快照会有操作限制。因此建议不要创建以autobk_snapshot_为名称前缀的快照，避免影响快照的正常使用。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "snapshot": {
            "name": "snap-001", 
            "description": "Daily backup", 
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635", 
            "force": false, 
            "metadata": { }
        }
    }
    ```


## 响应<a name="section26860493104128"></a>

-   响应参数

    <a name="zh-cn_topic_0051408624_table3822335104128"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408624_row44730354104128"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408624_p66388932104128"><a name="zh-cn_topic_0051408624_p66388932104128"></a><a name="zh-cn_topic_0051408624_p66388932104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408624_p8794435104128"><a name="zh-cn_topic_0051408624_p8794435104128"></a><a name="zh-cn_topic_0051408624_p8794435104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408624_p53776742104128"><a name="zh-cn_topic_0051408624_p53776742104128"></a><a name="zh-cn_topic_0051408624_p53776742104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408624_row60948826104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p37907867104128"><a name="zh-cn_topic_0051408624_p37907867104128"></a><a name="zh-cn_topic_0051408624_p37907867104128"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p50638352104128"><a name="zh-cn_topic_0051408624_p50638352104128"></a><a name="zh-cn_topic_0051408624_p50638352104128"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p49352120104128"><a name="zh-cn_topic_0051408624_p49352120104128"></a><a name="zh-cn_topic_0051408624_p49352120104128"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row41515896104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p7344400104128"><a name="zh-cn_topic_0051408624_p7344400104128"></a><a name="zh-cn_topic_0051408624_p7344400104128"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p58025504104128"><a name="zh-cn_topic_0051408624_p58025504104128"></a><a name="zh-cn_topic_0051408624_p58025504104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p63859146104128"><a name="zh-cn_topic_0051408624_p63859146104128"></a><a name="zh-cn_topic_0051408624_p63859146104128"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row37861410104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p46875355104128"><a name="zh-cn_topic_0051408624_p46875355104128"></a><a name="zh-cn_topic_0051408624_p46875355104128"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p38807409104128"><a name="zh-cn_topic_0051408624_p38807409104128"></a><a name="zh-cn_topic_0051408624_p38807409104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p4381265104128"><a name="zh-cn_topic_0051408624_p4381265104128"></a><a name="zh-cn_topic_0051408624_p4381265104128"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row39431393104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p39826261104128"><a name="zh-cn_topic_0051408624_p39826261104128"></a><a name="zh-cn_topic_0051408624_p39826261104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p4701738104128"><a name="zh-cn_topic_0051408624_p4701738104128"></a><a name="zh-cn_topic_0051408624_p4701738104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p45139478104128"><a name="zh-cn_topic_0051408624_p45139478104128"></a><a name="zh-cn_topic_0051408624_p45139478104128"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row3602118104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p23336160104128"><a name="zh-cn_topic_0051408624_p23336160104128"></a><a name="zh-cn_topic_0051408624_p23336160104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p11180798104128"><a name="zh-cn_topic_0051408624_p11180798104128"></a><a name="zh-cn_topic_0051408624_p11180798104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p7230824104128"><a name="zh-cn_topic_0051408624_p7230824104128"></a><a name="zh-cn_topic_0051408624_p7230824104128"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row65077419104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p36779556104128"><a name="zh-cn_topic_0051408624_p36779556104128"></a><a name="zh-cn_topic_0051408624_p36779556104128"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p26354021104128"><a name="zh-cn_topic_0051408624_p26354021104128"></a><a name="zh-cn_topic_0051408624_p26354021104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p36300897104128"><a name="zh-cn_topic_0051408624_p36300897104128"></a><a name="zh-cn_topic_0051408624_p36300897104128"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row58272623104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p22462033104128"><a name="zh-cn_topic_0051408624_p22462033104128"></a><a name="zh-cn_topic_0051408624_p22462033104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p7485408104128"><a name="zh-cn_topic_0051408624_p7485408104128"></a><a name="zh-cn_topic_0051408624_p7485408104128"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p55185187104128"><a name="zh-cn_topic_0051408624_p55185187104128"></a><a name="zh-cn_topic_0051408624_p55185187104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row26904637104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p31791970104128"><a name="zh-cn_topic_0051408624_p31791970104128"></a><a name="zh-cn_topic_0051408624_p31791970104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p25012792104128"><a name="zh-cn_topic_0051408624_p25012792104128"></a><a name="zh-cn_topic_0051408624_p25012792104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p27759637104128"><a name="zh-cn_topic_0051408624_p27759637104128"></a><a name="zh-cn_topic_0051408624_p27759637104128"></a>快照所属的云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row48510149104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p37007959104128"><a name="zh-cn_topic_0051408624_p37007959104128"></a><a name="zh-cn_topic_0051408624_p37007959104128"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p44854718104128"><a name="zh-cn_topic_0051408624_p44854718104128"></a><a name="zh-cn_topic_0051408624_p44854718104128"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p19441706104128"><a name="zh-cn_topic_0051408624_p19441706104128"></a><a name="zh-cn_topic_0051408624_p19441706104128"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408624_row40757631104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408624_p13033849104128"><a name="zh-cn_topic_0051408624_p13033849104128"></a><a name="zh-cn_topic_0051408624_p13033849104128"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408624_p49108876104128"><a name="zh-cn_topic_0051408624_p49108876104128"></a><a name="zh-cn_topic_0051408624_p49108876104128"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408624_p13680922104128"><a name="zh-cn_topic_0051408624_p13680922104128"></a><a name="zh-cn_topic_0051408624_p13680922104128"></a>快照更新时间。</p>
    </td>
    </tr>
    <tr id="row178831721104211"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p5139827184211"><a name="p5139827184211"></a><a name="p5139827184211"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p181391727194219"><a name="p181391727194219"></a><a name="p181391727194219"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p14842212163011"><a name="p14842212163011"></a><a name="p14842212163011"></a>预留属性。</p>
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
            "id": "ffa9bc5e-1172-4021-acaf-cdcd78a9584d", 
            "name": "snap-001",
            "user_id”:”48d70679b8644035846b2cb53633c256",  
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


## 返回值<a name="section10171239104128"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

