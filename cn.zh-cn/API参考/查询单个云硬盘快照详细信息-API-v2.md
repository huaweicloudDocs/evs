# 查询单个云硬盘快照详细信息<a name="evs_04_2019"></a>

## 功能介绍<a name="section30030484111731"></a>

查询单个云硬盘快照信息。支持企业项目授权功能。

## URI<a name="section14733765111731"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudsnapshots/\{snapshot\_id\}

-   参数说明

    <a name="evs_04_2098_table66271751111731"></a>
    <table><thead align="left"><tr id="evs_04_2098_row56106054111731"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="evs_04_2098_p48296540111731"><a name="evs_04_2098_p48296540111731"></a><a name="evs_04_2098_p48296540111731"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="evs_04_2098_p19705674111731"><a name="evs_04_2098_p19705674111731"></a><a name="evs_04_2098_p19705674111731"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="evs_04_2098_p52655801111731"><a name="evs_04_2098_p52655801111731"></a><a name="evs_04_2098_p52655801111731"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2098_row37261521111731"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p65393209111731"><a name="evs_04_2098_p65393209111731"></a><a name="evs_04_2098_p65393209111731"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p62358553111731"><a name="evs_04_2098_p62358553111731"></a><a name="evs_04_2098_p62358553111731"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p17878042111731"><a name="evs_04_2098_p17878042111731"></a><a name="evs_04_2098_p17878042111731"></a>项目ID。</p>
    <p id="evs_04_2098_p55811451337"><a name="evs_04_2098_p55811451337"></a><a name="evs_04_2098_p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row26684654111731"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p13973379111731"><a name="evs_04_2098_p13973379111731"></a><a name="evs_04_2098_p13973379111731"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p58101900111731"><a name="evs_04_2098_p58101900111731"></a><a name="evs_04_2098_p58101900111731"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p8633458111731"><a name="evs_04_2098_p8633458111731"></a><a name="evs_04_2098_p8633458111731"></a>快照ID</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section28221468111731"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v2/{project_id}/cloudsnapshots/f9faf7df-fdc1-4093-9ef3-5cba06eef995
    ```


## 响应消息<a name="section63055193111836"></a>

-   响应参数

    <a name="evs_04_2098_table12298112761311"></a>
    <table><thead align="left"><tr id="evs_04_2098_row3298122761310"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2098_p1129817277138"><a name="evs_04_2098_p1129817277138"></a><a name="evs_04_2098_p1129817277138"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2098_p102981727131315"><a name="evs_04_2098_p102981727131315"></a><a name="evs_04_2098_p102981727131315"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2098_p1829872710136"><a name="evs_04_2098_p1829872710136"></a><a name="evs_04_2098_p1829872710136"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2098_row1029817278135"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p72986273130"><a name="evs_04_2098_p72986273130"></a><a name="evs_04_2098_p72986273130"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p3299527151313"><a name="evs_04_2098_p3299527151313"></a><a name="evs_04_2098_p3299527151313"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p102991727171313"><a name="evs_04_2098_p102991727171313"></a><a name="evs_04_2098_p102991727171313"></a>快照信息，请参见<a href="#evs_04_2098_li64773086111836">•snapshot参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row1148619118454"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p129522216412"><a name="evs_04_2098_p129522216412"></a><a name="evs_04_2098_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p1595262111415"><a name="evs_04_2098_p1595262111415"></a><a name="evs_04_2098_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p109527215417"><a name="evs_04_2098_p109527215417"></a><a name="evs_04_2098_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2098_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2098_li64773086111836"></a>snapshot参数说明

    <a name="evs_04_2098_table46086870111836"></a>
    <table><thead align="left"><tr id="evs_04_2098_row56202297111836"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2098_p56092213111836"><a name="evs_04_2098_p56092213111836"></a><a name="evs_04_2098_p56092213111836"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2098_p47175401111836"><a name="evs_04_2098_p47175401111836"></a><a name="evs_04_2098_p47175401111836"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2098_p11730844111836"><a name="evs_04_2098_p11730844111836"></a><a name="evs_04_2098_p11730844111836"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2098_row15559516111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p52361272111836"><a name="evs_04_2098_p52361272111836"></a><a name="evs_04_2098_p52361272111836"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p13404600111836"><a name="evs_04_2098_p13404600111836"></a><a name="evs_04_2098_p13404600111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p34969797111836"><a name="evs_04_2098_p34969797111836"></a><a name="evs_04_2098_p34969797111836"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row46292725111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p58723264111836"><a name="evs_04_2098_p58723264111836"></a><a name="evs_04_2098_p58723264111836"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p58963956111836"><a name="evs_04_2098_p58963956111836"></a><a name="evs_04_2098_p58963956111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p47023540111836"><a name="evs_04_2098_p47023540111836"></a><a name="evs_04_2098_p47023540111836"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row20558679111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p54640283111836"><a name="evs_04_2098_p54640283111836"></a><a name="evs_04_2098_p54640283111836"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p63786796111836"><a name="evs_04_2098_p63786796111836"></a><a name="evs_04_2098_p63786796111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p14293074111836"><a name="evs_04_2098_p14293074111836"></a><a name="evs_04_2098_p14293074111836"></a>云硬盘快照名称。</p>
    <p id="evs_04_2098_p1338613133449"><a name="evs_04_2098_p1338613133449"></a><a name="evs_04_2098_p1338613133449"></a>名称以autobk_snapshot_为前缀的快照是创建云硬盘备份时系统自动创建的，请不要进行“删除云硬盘快照”和“回滚快照到云硬盘”操作。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row61528809111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p17777665111836"><a name="evs_04_2098_p17777665111836"></a><a name="evs_04_2098_p17777665111836"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p30704745111836"><a name="evs_04_2098_p30704745111836"></a><a name="evs_04_2098_p30704745111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p60132426111836"><a name="evs_04_2098_p60132426111836"></a><a name="evs_04_2098_p60132426111836"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row4320926111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p14450739111836"><a name="evs_04_2098_p14450739111836"></a><a name="evs_04_2098_p14450739111836"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p29659196111836"><a name="evs_04_2098_p29659196111836"></a><a name="evs_04_2098_p29659196111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p45391308111836"><a name="evs_04_2098_p45391308111836"></a><a name="evs_04_2098_p45391308111836"></a>云硬盘快照创建时间。</p>
    <p id="evs_04_2098_p1559945216131"><a name="evs_04_2098_p1559945216131"></a><a name="evs_04_2098_p1559945216131"></a><span id="evs_04_2098_text462016291416"><a name="evs_04_2098_text462016291416"></a><a name="evs_04_2098_text462016291416"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2098_row3737236411149"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p80695711149"><a name="evs_04_2098_p80695711149"></a><a name="evs_04_2098_p80695711149"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p6536351711149"><a name="evs_04_2098_p6536351711149"></a><a name="evs_04_2098_p6536351711149"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p2439511411149"><a name="evs_04_2098_p2439511411149"></a><a name="evs_04_2098_p2439511411149"></a>云硬盘快照更新时间。</p>
    <p id="evs_04_2098_p4282185140"><a name="evs_04_2098_p4282185140"></a><a name="evs_04_2098_p4282185140"></a><span id="evs_04_2098_text106095811141"><a name="evs_04_2098_text106095811141"></a><a name="evs_04_2098_text106095811141"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2098_row5868590111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p5593786111836"><a name="evs_04_2098_p5593786111836"></a><a name="evs_04_2098_p5593786111836"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p50443518111836"><a name="evs_04_2098_p50443518111836"></a><a name="evs_04_2098_p50443518111836"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p46118865111836"><a name="evs_04_2098_p46118865111836"></a><a name="evs_04_2098_p46118865111836"></a>云硬盘快照的元数据信息。</p>
    <p id="evs_04_2098_p771812911458"><a name="evs_04_2098_p771812911458"></a><a name="evs_04_2098_p771812911458"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row12416602111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p66220711111836"><a name="evs_04_2098_p66220711111836"></a><a name="evs_04_2098_p66220711111836"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p62277393111836"><a name="evs_04_2098_p62277393111836"></a><a name="evs_04_2098_p62277393111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p43213914111836"><a name="evs_04_2098_p43213914111836"></a><a name="evs_04_2098_p43213914111836"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row53380907111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p28886228111836"><a name="evs_04_2098_p28886228111836"></a><a name="evs_04_2098_p28886228111836"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p58083101111836"><a name="evs_04_2098_p58083101111836"></a><a name="evs_04_2098_p58083101111836"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p39095984111836"><a name="evs_04_2098_p39095984111836"></a><a name="evs_04_2098_p39095984111836"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_row16319538111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p46814240111836"><a name="evs_04_2098_p46814240111836"></a><a name="evs_04_2098_p46814240111836"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p33857106111836"><a name="evs_04_2098_p33857106111836"></a><a name="evs_04_2098_p33857106111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_p6137764111836"><a name="evs_04_2098_p6137764111836"></a><a name="evs_04_2098_p6137764111836"></a>租户ID。<span id="evs_04_2098_text19941457165313"><a name="evs_04_2098_text19941457165313"></a><a name="evs_04_2098_text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2098_row55239881111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_p45245366111836"><a name="evs_04_2098_p45245366111836"></a><a name="evs_04_2098_p45245366111836"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_p40996011111836"><a name="evs_04_2098_p40996011111836"></a><a name="evs_04_2098_p40996011111836"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_zh-cn_topic_0123550104_p170219911618"><a name="evs_04_2098_zh-cn_topic_0123550104_p170219911618"></a><a name="evs_04_2098_zh-cn_topic_0123550104_p170219911618"></a><span id="evs_04_2098_text4730642777"><a name="evs_04_2098_text4730642777"></a><a name="evs_04_2098_text4730642777"></a>预留属性。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2098_li0419202382514"></a>error参数说明

    <a name="evs_04_2098_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2098_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2098_evs_04_2013_p19541716103019"><a name="evs_04_2098_evs_04_2013_p19541716103019"></a><a name="evs_04_2098_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2098_evs_04_2013_p39375186103019"><a name="evs_04_2098_evs_04_2013_p39375186103019"></a><a name="evs_04_2098_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2098_evs_04_2013_p38578950103019"><a name="evs_04_2098_evs_04_2013_p38578950103019"></a><a name="evs_04_2098_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2098_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_evs_04_2013_p46815658103019"><a name="evs_04_2098_evs_04_2013_p46815658103019"></a><a name="evs_04_2098_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_evs_04_2013_p33971979103019"><a name="evs_04_2098_evs_04_2013_p33971979103019"></a><a name="evs_04_2098_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_evs_04_2013_p21623243103019"><a name="evs_04_2098_evs_04_2013_p21623243103019"></a><a name="evs_04_2098_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2098_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2098_evs_04_2013_p59870541103019"><a name="evs_04_2098_evs_04_2013_p59870541103019"></a><a name="evs_04_2098_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2098_evs_04_2013_p17675690103019"><a name="evs_04_2098_evs_04_2013_p17675690103019"></a><a name="evs_04_2098_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2098_evs_04_2013_p6087468103019"><a name="evs_04_2098_evs_04_2013_p6087468103019"></a><a name="evs_04_2098_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2098_evs_04_2013_p54787218103019"><a name="evs_04_2098_evs_04_2013_p54787218103019"></a><a name="evs_04_2098_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "snapshot": {
            "status": "available",
            "os-extended-snapshot-attributes:progress": "100%",
            "description": "daily backup",
            "created_at": "2013-02-25t04:13:17.000000",
            "metadata": {},
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635",
            "os-extended-snapshot-attributes:project_id": "0c2eba2c5af04d3f9e9d0d410b371fde",
            "size": 1,
            "id": "2bb856e1-b3d8-4432-a858-09e4ce939389",
            "name": "snap-001",
            "updated_at": null
    
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


## 状态码<a name="section38811440112026"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

