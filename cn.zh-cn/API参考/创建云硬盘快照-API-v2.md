# 创建云硬盘快照<a name="evs_04_2016"></a>

## 功能介绍<a name="section29798282112049"></a>

创建云硬盘快照。支持企业项目授权功能。

## URI<a name="section56404342112049"></a>

-   URI格式

    POST /v2/\{project\_id\}/cloudsnapshots


-   参数说明

    <a name="evs_04_2093_table28484833104128"></a>
    <table><thead align="left"><tr id="evs_04_2093_row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="evs_04_2093_p5384679104128"><a name="evs_04_2093_p5384679104128"></a><a name="evs_04_2093_p5384679104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="evs_04_2093_p33505894104128"><a name="evs_04_2093_p33505894104128"></a><a name="evs_04_2093_p33505894104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="evs_04_2093_p29622926104128"><a name="evs_04_2093_p29622926104128"></a><a name="evs_04_2093_p29622926104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_row50646790104128"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p8749302104128"><a name="evs_04_2093_p8749302104128"></a><a name="evs_04_2093_p8749302104128"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p37604871104128"><a name="evs_04_2093_p37604871104128"></a><a name="evs_04_2093_p37604871104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p26095712104128"><a name="evs_04_2093_p26095712104128"></a><a name="evs_04_2093_p26095712104128"></a>项目ID。</p>
    <p id="evs_04_2093_p55811451337"><a name="evs_04_2093_p55811451337"></a><a name="evs_04_2093_p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section54272198112126"></a>

-   请求参数

    <a name="evs_04_2093_table1572462410119"></a>
    <table><thead align="left"><tr id="evs_04_2093_row2724724141119"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2093_p20724132431116"><a name="evs_04_2093_p20724132431116"></a><a name="evs_04_2093_p20724132431116"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2093_p3724122431120"><a name="evs_04_2093_p3724122431120"></a><a name="evs_04_2093_p3724122431120"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="evs_04_2093_p15724192491114"><a name="evs_04_2093_p15724192491114"></a><a name="evs_04_2093_p15724192491114"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="evs_04_2093_p0724324121113"><a name="evs_04_2093_p0724324121113"></a><a name="evs_04_2093_p0724324121113"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_row147241024121113"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p187251024171111"><a name="evs_04_2093_p187251024171111"></a><a name="evs_04_2093_p187251024171111"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p67255248118"><a name="evs_04_2093_p67255248118"></a><a name="evs_04_2093_p67255248118"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p127251724191119"><a name="evs_04_2093_p127251724191119"></a><a name="evs_04_2093_p127251724191119"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p16725122411114"><a name="evs_04_2093_p16725122411114"></a><a name="evs_04_2093_p16725122411114"></a>待创建的快照信息，请参见<a href="#evs_04_2093_li39126135104128">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2093_li39126135104128"></a>snapshot参数说明

    <a name="evs_04_2093_table16590896104128"></a>
    <table><thead align="left"><tr id="evs_04_2093_row60389002104128"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2093_p59671014104128"><a name="evs_04_2093_p59671014104128"></a><a name="evs_04_2093_p59671014104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2093_p1513999104128"><a name="evs_04_2093_p1513999104128"></a><a name="evs_04_2093_p1513999104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="evs_04_2093_p55525100104128"><a name="evs_04_2093_p55525100104128"></a><a name="evs_04_2093_p55525100104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="evs_04_2093_p1239270104128"><a name="evs_04_2093_p1239270104128"></a><a name="evs_04_2093_p1239270104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_row12756475104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p26641549104128"><a name="evs_04_2093_p26641549104128"></a><a name="evs_04_2093_p26641549104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p10481847104128"><a name="evs_04_2093_p10481847104128"></a><a name="evs_04_2093_p10481847104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p43723298104128"><a name="evs_04_2093_p43723298104128"></a><a name="evs_04_2093_p43723298104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p51926262104128"><a name="evs_04_2093_p51926262104128"></a><a name="evs_04_2093_p51926262104128"></a>创建快照源云硬盘的ID。</p>
    <p id="evs_04_2093_p75131646112520"><a name="evs_04_2093_p75131646112520"></a><a name="evs_04_2093_p75131646112520"></a>通过<a href="查询所有云硬盘详情-Cinder-v3.md">查询所有云硬盘详情</a>获取。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row64683174104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p4845737104128"><a name="evs_04_2093_p4845737104128"></a><a name="evs_04_2093_p4845737104128"></a>force</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p56960425104128"><a name="evs_04_2093_p56960425104128"></a><a name="evs_04_2093_p56960425104128"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p50391693104128"><a name="evs_04_2093_p50391693104128"></a><a name="evs_04_2093_p50391693104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p32530251113919"><a name="evs_04_2093_p32530251113919"></a><a name="evs_04_2093_p32530251113919"></a>强制创快照标示，默认为false。</p>
    <a name="evs_04_2093_ul60750582141455"></a><a name="evs_04_2093_ul60750582141455"></a><ul id="evs_04_2093_ul60750582141455"><li>当force标记为false时，云硬盘处于挂载状态时，不能强制创建快照。</li><li>当force标记为true时，即使云硬盘处于挂载状态时，仍可以创建快照。</li></ul>
    </td>
    </tr>
    <tr id="evs_04_2093_row26995886104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p39183164104128"><a name="evs_04_2093_p39183164104128"></a><a name="evs_04_2093_p39183164104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p19719755104128"><a name="evs_04_2093_p19719755104128"></a><a name="evs_04_2093_p19719755104128"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p53796355104128"><a name="evs_04_2093_p53796355104128"></a><a name="evs_04_2093_p53796355104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p62537483104128"><a name="evs_04_2093_p62537483104128"></a><a name="evs_04_2093_p62537483104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row25966436104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p22906600104128"><a name="evs_04_2093_p22906600104128"></a><a name="evs_04_2093_p22906600104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p43495312104128"><a name="evs_04_2093_p43495312104128"></a><a name="evs_04_2093_p43495312104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p33459397104128"><a name="evs_04_2093_p33459397104128"></a><a name="evs_04_2093_p33459397104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p25856622104128"><a name="evs_04_2093_p25856622104128"></a><a name="evs_04_2093_p25856622104128"></a>云硬盘快照描述，可以为null。<span id="evs_04_2093_text59690989152428"><a name="evs_04_2093_text59690989152428"></a><a name="evs_04_2093_text59690989152428"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2093_row31383010104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2093_p58995861104128"><a name="evs_04_2093_p58995861104128"></a><a name="evs_04_2093_p58995861104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2093_p13935408104128"><a name="evs_04_2093_p13935408104128"></a><a name="evs_04_2093_p13935408104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="evs_04_2093_p55026268104128"><a name="evs_04_2093_p55026268104128"></a><a name="evs_04_2093_p55026268104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="evs_04_2093_p27942720104128"><a name="evs_04_2093_p27942720104128"></a><a name="evs_04_2093_p27942720104128"></a>云硬盘快照名称。<span id="evs_04_2093_text26279838152439"><a name="evs_04_2093_text26279838152439"></a><a name="evs_04_2093_text26279838152439"></a>最大支持255个字节。</span></p>
    <div class="note" id="evs_04_2093_note12652884103214"><a name="evs_04_2093_note12652884103214"></a><a name="evs_04_2093_note12652884103214"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2093_p46767097103214"><a name="evs_04_2093_p46767097103214"></a><a name="evs_04_2093_p46767097103214"></a>对云硬盘创建备份时，同时会创建以autobk_snapshot_为名称前缀的快照，云硬盘控制台对此类快照会有操作限制。因此建议不要创建以autobk_snapshot_为名称前缀的快照，避免影响快照的正常使用。</p>
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


## 响应消息<a name="section50618846112239"></a>

-   响应参数

    <a name="evs_04_2093_table6828747432"></a>
    <table><thead align="left"><tr id="evs_04_2093_row382812473312"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="evs_04_2093_p198297471937"><a name="evs_04_2093_p198297471937"></a><a name="evs_04_2093_p198297471937"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2093_p2082911475318"><a name="evs_04_2093_p2082911475318"></a><a name="evs_04_2093_p2082911475318"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2093_p182916473314"><a name="evs_04_2093_p182916473314"></a><a name="evs_04_2093_p182916473314"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_row168291947832"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p982919471312"><a name="evs_04_2093_p982919471312"></a><a name="evs_04_2093_p982919471312"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p08292471734"><a name="evs_04_2093_p08292471734"></a><a name="evs_04_2093_p08292471734"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p208298477312"><a name="evs_04_2093_p208298477312"></a><a name="evs_04_2093_p208298477312"></a>快照信息，请参见<a href="#evs_04_2093_li52620487104128">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row5943559134615"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p129522216412"><a name="evs_04_2093_p129522216412"></a><a name="evs_04_2093_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p1595262111415"><a name="evs_04_2093_p1595262111415"></a><a name="evs_04_2093_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p109527215417"><a name="evs_04_2093_p109527215417"></a><a name="evs_04_2093_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2093_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2093_li52620487104128"></a>snapshot参数说明

    <a name="evs_04_2093_table3822335104128"></a>
    <table><thead align="left"><tr id="evs_04_2093_row44730354104128"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="evs_04_2093_p66388932104128"><a name="evs_04_2093_p66388932104128"></a><a name="evs_04_2093_p66388932104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2093_p8794435104128"><a name="evs_04_2093_p8794435104128"></a><a name="evs_04_2093_p8794435104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2093_p53776742104128"><a name="evs_04_2093_p53776742104128"></a><a name="evs_04_2093_p53776742104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_row41515896104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p7344400104128"><a name="evs_04_2093_p7344400104128"></a><a name="evs_04_2093_p7344400104128"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p58025504104128"><a name="evs_04_2093_p58025504104128"></a><a name="evs_04_2093_p58025504104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p63859146104128"><a name="evs_04_2093_p63859146104128"></a><a name="evs_04_2093_p63859146104128"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row37861410104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p46875355104128"><a name="evs_04_2093_p46875355104128"></a><a name="evs_04_2093_p46875355104128"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p38807409104128"><a name="evs_04_2093_p38807409104128"></a><a name="evs_04_2093_p38807409104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p4381265104128"><a name="evs_04_2093_p4381265104128"></a><a name="evs_04_2093_p4381265104128"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row39431393104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p39826261104128"><a name="evs_04_2093_p39826261104128"></a><a name="evs_04_2093_p39826261104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p4701738104128"><a name="evs_04_2093_p4701738104128"></a><a name="evs_04_2093_p4701738104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p45139478104128"><a name="evs_04_2093_p45139478104128"></a><a name="evs_04_2093_p45139478104128"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row3602118104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p23336160104128"><a name="evs_04_2093_p23336160104128"></a><a name="evs_04_2093_p23336160104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p11180798104128"><a name="evs_04_2093_p11180798104128"></a><a name="evs_04_2093_p11180798104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p7230824104128"><a name="evs_04_2093_p7230824104128"></a><a name="evs_04_2093_p7230824104128"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row65077419104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p36779556104128"><a name="evs_04_2093_p36779556104128"></a><a name="evs_04_2093_p36779556104128"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p26354021104128"><a name="evs_04_2093_p26354021104128"></a><a name="evs_04_2093_p26354021104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p36300897104128"><a name="evs_04_2093_p36300897104128"></a><a name="evs_04_2093_p36300897104128"></a>云硬盘快照创建时间。</p>
    <p id="evs_04_2093_p1277514183418"><a name="evs_04_2093_p1277514183418"></a><a name="evs_04_2093_p1277514183418"></a><span id="evs_04_2093_text56625358415"><a name="evs_04_2093_text56625358415"></a><a name="evs_04_2093_text56625358415"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2093_row58272623104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p22462033104128"><a name="evs_04_2093_p22462033104128"></a><a name="evs_04_2093_p22462033104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p7485408104128"><a name="evs_04_2093_p7485408104128"></a><a name="evs_04_2093_p7485408104128"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p55185187104128"><a name="evs_04_2093_p55185187104128"></a><a name="evs_04_2093_p55185187104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row26904637104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p31791970104128"><a name="evs_04_2093_p31791970104128"></a><a name="evs_04_2093_p31791970104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p25012792104128"><a name="evs_04_2093_p25012792104128"></a><a name="evs_04_2093_p25012792104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p27759637104128"><a name="evs_04_2093_p27759637104128"></a><a name="evs_04_2093_p27759637104128"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row48510149104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p37007959104128"><a name="evs_04_2093_p37007959104128"></a><a name="evs_04_2093_p37007959104128"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p44854718104128"><a name="evs_04_2093_p44854718104128"></a><a name="evs_04_2093_p44854718104128"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p19441706104128"><a name="evs_04_2093_p19441706104128"></a><a name="evs_04_2093_p19441706104128"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_row40757631104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_p13033849104128"><a name="evs_04_2093_p13033849104128"></a><a name="evs_04_2093_p13033849104128"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_p49108876104128"><a name="evs_04_2093_p49108876104128"></a><a name="evs_04_2093_p49108876104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_p13680922104128"><a name="evs_04_2093_p13680922104128"></a><a name="evs_04_2093_p13680922104128"></a>快照更新时间。</p>
    <p id="evs_04_2093_p24641261550"><a name="evs_04_2093_p24641261550"></a><a name="evs_04_2093_p24641261550"></a><span id="evs_04_2093_text123011106519"><a name="evs_04_2093_text123011106519"></a><a name="evs_04_2093_text123011106519"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2093_li0419202382514"></a>error参数说明

    <a name="evs_04_2093_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2093_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2093_evs_04_2013_p19541716103019"><a name="evs_04_2093_evs_04_2013_p19541716103019"></a><a name="evs_04_2093_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2093_evs_04_2013_p39375186103019"><a name="evs_04_2093_evs_04_2013_p39375186103019"></a><a name="evs_04_2093_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2093_evs_04_2013_p38578950103019"><a name="evs_04_2093_evs_04_2013_p38578950103019"></a><a name="evs_04_2093_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2093_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_evs_04_2013_p46815658103019"><a name="evs_04_2093_evs_04_2013_p46815658103019"></a><a name="evs_04_2093_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_evs_04_2013_p33971979103019"><a name="evs_04_2093_evs_04_2013_p33971979103019"></a><a name="evs_04_2093_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_evs_04_2013_p21623243103019"><a name="evs_04_2093_evs_04_2013_p21623243103019"></a><a name="evs_04_2093_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2093_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2093_evs_04_2013_p59870541103019"><a name="evs_04_2093_evs_04_2013_p59870541103019"></a><a name="evs_04_2093_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2093_evs_04_2013_p17675690103019"><a name="evs_04_2093_evs_04_2013_p17675690103019"></a><a name="evs_04_2093_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2093_evs_04_2013_p6087468103019"><a name="evs_04_2093_evs_04_2013_p6087468103019"></a><a name="evs_04_2093_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2093_evs_04_2013_p54787218103019"><a name="evs_04_2093_evs_04_2013_p54787218103019"></a><a name="evs_04_2093_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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


## 状态码<a name="section16529200112352"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

