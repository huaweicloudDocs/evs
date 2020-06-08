# 创建云硬盘快照<a name="evs_04_2093"></a>

## 功能介绍<a name="section17386310104128"></a>

创建云硬盘快照。

## URI<a name="section48475837104128"></a>

-   URI格式

    POST /v2/\{project\_id\}/snapshots

-   参数说明

    <a name="table28484833104128"></a>
    <table><thead align="left"><tr id="row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p5384679104128"><a name="p5384679104128"></a><a name="p5384679104128"></a>参数</p>
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
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section33377962104128"></a>

-   请求参数

    <a name="table1572462410119"></a>
    <table><thead align="left"><tr id="row2724724141119"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p20724132431116"><a name="p20724132431116"></a><a name="p20724132431116"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p3724122431120"><a name="p3724122431120"></a><a name="p3724122431120"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p15724192491114"><a name="p15724192491114"></a><a name="p15724192491114"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p0724324121113"><a name="p0724324121113"></a><a name="p0724324121113"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row147241024121113"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p187251024171111"><a name="p187251024171111"></a><a name="p187251024171111"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p67255248118"><a name="p67255248118"></a><a name="p67255248118"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p127251724191119"><a name="p127251724191119"></a><a name="p127251724191119"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p16725122411114"><a name="p16725122411114"></a><a name="p16725122411114"></a>待创建的快照信息，请参见<a href="#li39126135104128">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li39126135104128"></a>snapshot参数说明

    <a name="table16590896104128"></a>
    <table><thead align="left"><tr id="row60389002104128"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p59671014104128"><a name="p59671014104128"></a><a name="p59671014104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p1513999104128"><a name="p1513999104128"></a><a name="p1513999104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p55525100104128"><a name="p55525100104128"></a><a name="p55525100104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p1239270104128"><a name="p1239270104128"></a><a name="p1239270104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12756475104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p26641549104128"><a name="p26641549104128"></a><a name="p26641549104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p10481847104128"><a name="p10481847104128"></a><a name="p10481847104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p43723298104128"><a name="p43723298104128"></a><a name="p43723298104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p51926262104128"><a name="p51926262104128"></a><a name="p51926262104128"></a>创建快照源云硬盘的ID。</p>
    <p id="p75131646112520"><a name="p75131646112520"></a><a name="p75131646112520"></a>通过<a href="查询所有云硬盘详情-Cinder-v3.md">查询所有云硬盘详情</a>获取。</p>
    </td>
    </tr>
    <tr id="row64683174104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p4845737104128"><a name="p4845737104128"></a><a name="p4845737104128"></a>force</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p56960425104128"><a name="p56960425104128"></a><a name="p56960425104128"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p50391693104128"><a name="p50391693104128"></a><a name="p50391693104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p32530251113919"><a name="p32530251113919"></a><a name="p32530251113919"></a>强制创快照标示，默认为false。</p>
    <a name="ul60750582141455"></a><a name="ul60750582141455"></a><ul id="ul60750582141455"><li>当force标记为false时，云硬盘处于挂载状态时，不能强制创建快照。</li><li>当force标记为true时，即使云硬盘处于挂载状态时，仍可以创建快照。</li></ul>
    </td>
    </tr>
    <tr id="row26995886104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p39183164104128"><a name="p39183164104128"></a><a name="p39183164104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p19719755104128"><a name="p19719755104128"></a><a name="p19719755104128"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p53796355104128"><a name="p53796355104128"></a><a name="p53796355104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p62537483104128"><a name="p62537483104128"></a><a name="p62537483104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="row25966436104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p22906600104128"><a name="p22906600104128"></a><a name="p22906600104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p43495312104128"><a name="p43495312104128"></a><a name="p43495312104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p33459397104128"><a name="p33459397104128"></a><a name="p33459397104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p25856622104128"><a name="p25856622104128"></a><a name="p25856622104128"></a>云硬盘快照描述，可以为null。<span id="text59690989152428"><a name="text59690989152428"></a><a name="text59690989152428"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row31383010104128"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p58995861104128"><a name="p58995861104128"></a><a name="p58995861104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p13935408104128"><a name="p13935408104128"></a><a name="p13935408104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p55026268104128"><a name="p55026268104128"></a><a name="p55026268104128"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p27942720104128"><a name="p27942720104128"></a><a name="p27942720104128"></a>云硬盘快照名称。<span id="text26279838152439"><a name="text26279838152439"></a><a name="text26279838152439"></a>最大支持255个字节。</span></p>
    <div class="note" id="note12652884103214"><a name="note12652884103214"></a><a name="note12652884103214"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p46767097103214"><a name="p46767097103214"></a><a name="p46767097103214"></a>对云硬盘创建备份时，同时会创建以autobk_snapshot_为名称前缀的快照，云硬盘控制台对此类快照会有操作限制。因此建议不要创建以autobk_snapshot_为名称前缀的快照，避免影响快照的正常使用。</p>
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


## 响应消息<a name="section26860493104128"></a>

-   响应参数

    <a name="table6828747432"></a>
    <table><thead align="left"><tr id="row382812473312"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p198297471937"><a name="p198297471937"></a><a name="p198297471937"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p2082911475318"><a name="p2082911475318"></a><a name="p2082911475318"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p182916473314"><a name="p182916473314"></a><a name="p182916473314"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row168291947832"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p982919471312"><a name="p982919471312"></a><a name="p982919471312"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p08292471734"><a name="p08292471734"></a><a name="p08292471734"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p208298477312"><a name="p208298477312"></a><a name="p208298477312"></a>快照信息，请参见<a href="#li52620487104128">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row5943559134615"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li52620487104128"></a>snapshot参数说明

    <a name="table3822335104128"></a>
    <table><thead align="left"><tr id="row44730354104128"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p66388932104128"><a name="p66388932104128"></a><a name="p66388932104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p8794435104128"><a name="p8794435104128"></a><a name="p8794435104128"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p53776742104128"><a name="p53776742104128"></a><a name="p53776742104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row41515896104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p7344400104128"><a name="p7344400104128"></a><a name="p7344400104128"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p58025504104128"><a name="p58025504104128"></a><a name="p58025504104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p63859146104128"><a name="p63859146104128"></a><a name="p63859146104128"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row37861410104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p46875355104128"><a name="p46875355104128"></a><a name="p46875355104128"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p38807409104128"><a name="p38807409104128"></a><a name="p38807409104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p4381265104128"><a name="p4381265104128"></a><a name="p4381265104128"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row39431393104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p39826261104128"><a name="p39826261104128"></a><a name="p39826261104128"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p4701738104128"><a name="p4701738104128"></a><a name="p4701738104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p45139478104128"><a name="p45139478104128"></a><a name="p45139478104128"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row3602118104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p23336160104128"><a name="p23336160104128"></a><a name="p23336160104128"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p11180798104128"><a name="p11180798104128"></a><a name="p11180798104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p7230824104128"><a name="p7230824104128"></a><a name="p7230824104128"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row65077419104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p36779556104128"><a name="p36779556104128"></a><a name="p36779556104128"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p26354021104128"><a name="p26354021104128"></a><a name="p26354021104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p36300897104128"><a name="p36300897104128"></a><a name="p36300897104128"></a>云硬盘快照创建时间。</p>
    <p id="p1277514183418"><a name="p1277514183418"></a><a name="p1277514183418"></a><span id="text56625358415"><a name="text56625358415"></a><a name="text56625358415"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row58272623104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p22462033104128"><a name="p22462033104128"></a><a name="p22462033104128"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p7485408104128"><a name="p7485408104128"></a><a name="p7485408104128"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p55185187104128"><a name="p55185187104128"></a><a name="p55185187104128"></a>云硬盘快照的元数据信息。</p>
    </td>
    </tr>
    <tr id="row26904637104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p31791970104128"><a name="p31791970104128"></a><a name="p31791970104128"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p25012792104128"><a name="p25012792104128"></a><a name="p25012792104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p27759637104128"><a name="p27759637104128"></a><a name="p27759637104128"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row48510149104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p37007959104128"><a name="p37007959104128"></a><a name="p37007959104128"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p44854718104128"><a name="p44854718104128"></a><a name="p44854718104128"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p19441706104128"><a name="p19441706104128"></a><a name="p19441706104128"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="row40757631104128"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p13033849104128"><a name="p13033849104128"></a><a name="p13033849104128"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p49108876104128"><a name="p49108876104128"></a><a name="p49108876104128"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p13680922104128"><a name="p13680922104128"></a><a name="p13680922104128"></a>快照更新时间。</p>
    <p id="p24641261550"><a name="p24641261550"></a><a name="p24641261550"></a><span id="text123011106519"><a name="text123011106519"></a><a name="text123011106519"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
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


## 状态码<a name="section10171239104128"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

