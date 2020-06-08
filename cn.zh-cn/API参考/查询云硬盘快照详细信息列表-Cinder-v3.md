# 查询云硬盘快照详细信息列表<a name="evs_04_3060"></a>

## 功能介绍<a name="section63129217111110"></a>

查询云硬盘快照详细列表信息。

## URI<a name="section21460443111127"></a>

-   URI格式

    GET /v3/\{project\_id\}/snapshots/detail

-   参数说明

    <a name="table9361875111127"></a>
    <table><thead align="left"><tr id="row34794340111127"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p66878179111127"><a name="p66878179111127"></a><a name="p66878179111127"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p48423414111127"><a name="p48423414111127"></a><a name="p48423414111127"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p147761015152112"><a name="p147761015152112"></a><a name="p147761015152112"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12660986111127"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p18906939111127"><a name="p18906939111127"></a><a name="p18906939111127"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p55067056111127"><a name="p55067056111127"></a><a name="p55067056111127"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p31246529111127"><a name="p31246529111127"></a><a name="p31246529111127"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   request filter参数说明

    <a name="zh-cn_topic_0051408627_table49657902111140"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408627_row47265217111140"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0051408627_p3277402111140"><a name="zh-cn_topic_0051408627_p3277402111140"></a><a name="zh-cn_topic_0051408627_p3277402111140"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0051408627_p64143015111140"><a name="zh-cn_topic_0051408627_p64143015111140"></a><a name="zh-cn_topic_0051408627_p64143015111140"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0051408627_p28201745111140"><a name="zh-cn_topic_0051408627_p28201745111140"></a><a name="zh-cn_topic_0051408627_p28201745111140"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0051408627_p2639999111140"><a name="zh-cn_topic_0051408627_p2639999111140"></a><a name="zh-cn_topic_0051408627_p2639999111140"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19129165444110"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762430_p49168107152914"><a name="zh-cn_topic_0058762430_p49168107152914"></a><a name="zh-cn_topic_0058762430_p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762430_p23193765152914"><a name="zh-cn_topic_0058762430_p23193765152914"></a><a name="zh-cn_topic_0058762430_p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762430_p66755704152914"><a name="zh-cn_topic_0058762430_p66755704152914"></a><a name="zh-cn_topic_0058762430_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762430_p38502923152914"><a name="zh-cn_topic_0058762430_p38502923152914"></a><a name="zh-cn_topic_0058762430_p38502923152914"></a><span id="text127381323152311"><a name="text127381323152311"></a><a name="text127381323152311"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row23759995111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p45511467111140"><a name="zh-cn_topic_0051408627_p45511467111140"></a><a name="zh-cn_topic_0051408627_p45511467111140"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p62550228111140"><a name="zh-cn_topic_0051408627_p62550228111140"></a><a name="zh-cn_topic_0051408627_p62550228111140"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p33403677111140"><a name="zh-cn_topic_0051408627_p33403677111140"></a><a name="zh-cn_topic_0051408627_p33403677111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p21343278111140"><a name="zh-cn_topic_0051408627_p21343278111140"></a><a name="zh-cn_topic_0051408627_p21343278111140"></a>偏移量。</p>
    <div class="note" id="zh-cn_topic_0051408627_note6490498915441"><a name="zh-cn_topic_0051408627_note6490498915441"></a><a name="zh-cn_topic_0051408627_note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0051408627_p4727398915441"><a name="zh-cn_topic_0051408627_p4727398915441"></a><a name="zh-cn_topic_0051408627_p4727398915441"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row57871777111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p57102386111140"><a name="zh-cn_topic_0051408627_p57102386111140"></a><a name="zh-cn_topic_0051408627_p57102386111140"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p61890592111140"><a name="zh-cn_topic_0051408627_p61890592111140"></a><a name="zh-cn_topic_0051408627_p61890592111140"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p47082066111140"><a name="zh-cn_topic_0051408627_p47082066111140"></a><a name="zh-cn_topic_0051408627_p47082066111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p55551025111140"><a name="zh-cn_topic_0051408627_p55551025111140"></a><a name="zh-cn_topic_0051408627_p55551025111140"></a>返回结果个数限制。</p>
    <p id="p12396191941414"><a name="p12396191941414"></a><a name="p12396191941414"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="zh-cn_topic_0051408627_p14657115572511"><a name="zh-cn_topic_0051408627_p14657115572511"></a><a name="zh-cn_topic_0051408627_p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="zh-cn_topic_0051408627_p1233994321914"><a name="zh-cn_topic_0051408627_p1233994321914"></a><a name="zh-cn_topic_0051408627_p1233994321914"></a><strong id="zh-cn_topic_0051408627_b15619135183016"><a name="zh-cn_topic_0051408627_b15619135183016"></a><a name="zh-cn_topic_0051408627_b15619135183016"></a>GET /v3/<em id="zh-cn_topic_0051408627_i86219512306"><a name="zh-cn_topic_0051408627_i86219512306"></a><a name="zh-cn_topic_0051408627_i86219512306"></a>xxx</em>/snapshots/detail?limit=50</strong>，表示查询第1~50个快照。<strong id="zh-cn_topic_0051408627_b18611337305"><a name="zh-cn_topic_0051408627_b18611337305"></a><a name="zh-cn_topic_0051408627_b18611337305"></a>GET /v3/<em id="zh-cn_topic_0051408627_i149081817173015"><a name="zh-cn_topic_0051408627_i149081817173015"></a><a name="zh-cn_topic_0051408627_i149081817173015"></a>xxx</em>/snapshots/detail?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row30197180111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p30052553111140"><a name="zh-cn_topic_0051408627_p30052553111140"></a><a name="zh-cn_topic_0051408627_p30052553111140"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p18337718111140"><a name="zh-cn_topic_0051408627_p18337718111140"></a><a name="zh-cn_topic_0051408627_p18337718111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p8960171111140"><a name="zh-cn_topic_0051408627_p8960171111140"></a><a name="zh-cn_topic_0051408627_p8960171111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p54685265111140"><a name="zh-cn_topic_0051408627_p54685265111140"></a><a name="zh-cn_topic_0051408627_p54685265111140"></a>云硬盘快照名称。最大支持255个字节。</p>
    </td>
    </tr>
    <tr id="row475111724717"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p463319195457"><a name="p463319195457"></a><a name="p463319195457"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p1163321984520"><a name="p1163321984520"></a><a name="p1163321984520"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p663321934517"><a name="p663321934517"></a><a name="p663321934517"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><div class="p" id="p2030231013183"><a name="p2030231013183"></a><a name="p2030231013183"></a>返回结果按照降序或升序排列，默认为“desc”。<a name="ul66131813171815"></a><a name="ul66131813171815"></a><ul id="ul66131813171815"><li>降序：desc</li><li>升序：asc</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row22405342111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p2893391111140"><a name="zh-cn_topic_0051408627_p2893391111140"></a><a name="zh-cn_topic_0051408627_p2893391111140"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p33038150111140"><a name="zh-cn_topic_0051408627_p33038150111140"></a><a name="zh-cn_topic_0051408627_p33038150111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p58844456111140"><a name="zh-cn_topic_0051408627_p58844456111140"></a><a name="zh-cn_topic_0051408627_p58844456111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p1671647111140"><a name="zh-cn_topic_0051408627_p1671647111140"></a><a name="zh-cn_topic_0051408627_p1671647111140"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row15044830111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p10671727111140"><a name="zh-cn_topic_0051408627_p10671727111140"></a><a name="zh-cn_topic_0051408627_p10671727111140"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p59103560111140"><a name="zh-cn_topic_0051408627_p59103560111140"></a><a name="zh-cn_topic_0051408627_p59103560111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p22659090111140"><a name="zh-cn_topic_0051408627_p22659090111140"></a><a name="zh-cn_topic_0051408627_p22659090111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p23447029111140"><a name="zh-cn_topic_0051408627_p23447029111140"></a><a name="zh-cn_topic_0051408627_p23447029111140"></a>云硬盘快照对应的云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询状态为available的云硬盘快照为例。

-   请求样例

    ```
    GET https://{endpoint}/v3/{project_id}/snapshots/detail?status=available
    ```


## 响应消息<a name="section3672851111434"></a>

-   响应参数

    <a name="table410874917199"></a>
    <table><thead align="left"><tr id="row191081949171912"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p910894918193"><a name="p910894918193"></a><a name="p910894918193"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p10108124917198"><a name="p10108124917198"></a><a name="p10108124917198"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p21092049111914"><a name="p21092049111914"></a><a name="p21092049111914"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row210984917198"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p1110918496191"><a name="p1110918496191"></a><a name="p1110918496191"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p71092049171917"><a name="p71092049171917"></a><a name="p71092049171917"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1510954919191"><a name="p1510954919191"></a><a name="p1510954919191"></a>快照信息，请参见<a href="#zh-cn_topic_0051408627_li60262741111434">•snapshots参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row423792912203"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p13109154941914"><a name="p13109154941914"></a><a name="p13109154941914"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p19109154931910"><a name="p19109154931910"></a><a name="p19109154931910"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p9109649111919"><a name="p9109649111919"></a><a name="p9109649111919"></a>云硬盘快照列表查询位置标记。当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="row41117491194"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p611224941917"><a name="p611224941917"></a><a name="p611224941917"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1911211493192"><a name="p1911211493192"></a><a name="p1911211493192"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p6112184910193"><a name="p6112184910193"></a><a name="p6112184910193"></a>查询返回结果的数量。</p>
    </td>
    </tr>
    <tr id="row203891619182012"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="zh-cn_topic_0051408627_li60262741111434"></a>snapshots参数说明

    <a name="zh-cn_topic_0051408627_table5493760111434"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408627_row9951929111434"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408627_p799881111434"><a name="zh-cn_topic_0051408627_p799881111434"></a><a name="zh-cn_topic_0051408627_p799881111434"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408627_p64790373111434"><a name="zh-cn_topic_0051408627_p64790373111434"></a><a name="zh-cn_topic_0051408627_p64790373111434"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408627_p22098020111434"><a name="zh-cn_topic_0051408627_p22098020111434"></a><a name="zh-cn_topic_0051408627_p22098020111434"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408627_row30338895111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p41531445111434"><a name="zh-cn_topic_0051408627_p41531445111434"></a><a name="zh-cn_topic_0051408627_p41531445111434"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p8603891111434"><a name="zh-cn_topic_0051408627_p8603891111434"></a><a name="zh-cn_topic_0051408627_p8603891111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p11580698111434"><a name="zh-cn_topic_0051408627_p11580698111434"></a><a name="zh-cn_topic_0051408627_p11580698111434"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row37117420111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p53721059111434"><a name="zh-cn_topic_0051408627_p53721059111434"></a><a name="zh-cn_topic_0051408627_p53721059111434"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p56438551111434"><a name="zh-cn_topic_0051408627_p56438551111434"></a><a name="zh-cn_topic_0051408627_p56438551111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p53733716111434"><a name="zh-cn_topic_0051408627_p53733716111434"></a><a name="zh-cn_topic_0051408627_p53733716111434"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row13841398111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p47411481111434"><a name="zh-cn_topic_0051408627_p47411481111434"></a><a name="zh-cn_topic_0051408627_p47411481111434"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p15124732111434"><a name="zh-cn_topic_0051408627_p15124732111434"></a><a name="zh-cn_topic_0051408627_p15124732111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p46466595111434"><a name="zh-cn_topic_0051408627_p46466595111434"></a><a name="zh-cn_topic_0051408627_p46466595111434"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row15546175111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p51280630111434"><a name="zh-cn_topic_0051408627_p51280630111434"></a><a name="zh-cn_topic_0051408627_p51280630111434"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p60090386111434"><a name="zh-cn_topic_0051408627_p60090386111434"></a><a name="zh-cn_topic_0051408627_p60090386111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p55561368111434"><a name="zh-cn_topic_0051408627_p55561368111434"></a><a name="zh-cn_topic_0051408627_p55561368111434"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row30290270111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p37592805111434"><a name="zh-cn_topic_0051408627_p37592805111434"></a><a name="zh-cn_topic_0051408627_p37592805111434"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p25118356111434"><a name="zh-cn_topic_0051408627_p25118356111434"></a><a name="zh-cn_topic_0051408627_p25118356111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p49277837111434"><a name="zh-cn_topic_0051408627_p49277837111434"></a><a name="zh-cn_topic_0051408627_p49277837111434"></a>云硬盘快照创建时间。</p>
    <p id="p191521633192117"><a name="p191521633192117"></a><a name="p191521633192117"></a><span id="text152359383212"><a name="text152359383212"></a><a name="text152359383212"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row62090946113559"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p4553543411364"><a name="zh-cn_topic_0051408627_p4553543411364"></a><a name="zh-cn_topic_0051408627_p4553543411364"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p6449156711364"><a name="zh-cn_topic_0051408627_p6449156711364"></a><a name="zh-cn_topic_0051408627_p6449156711364"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p778860311364"><a name="zh-cn_topic_0051408627_p778860311364"></a><a name="zh-cn_topic_0051408627_p778860311364"></a>云硬盘快照更新时间。</p>
    <p id="p17722194212116"><a name="p17722194212116"></a><a name="p17722194212116"></a><span id="text1096915422211"><a name="text1096915422211"></a><a name="text1096915422211"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row40847350111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p20301014111434"><a name="zh-cn_topic_0051408627_p20301014111434"></a><a name="zh-cn_topic_0051408627_p20301014111434"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p33769410111434"><a name="zh-cn_topic_0051408627_p33769410111434"></a><a name="zh-cn_topic_0051408627_p33769410111434"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p34744289111434"><a name="zh-cn_topic_0051408627_p34744289111434"></a><a name="zh-cn_topic_0051408627_p34744289111434"></a>云硬盘快照的元数据信息。</p>
    <p id="p1678772717473"><a name="p1678772717473"></a><a name="p1678772717473"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row44263150111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p28545410111434"><a name="zh-cn_topic_0051408627_p28545410111434"></a><a name="zh-cn_topic_0051408627_p28545410111434"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p30476837111434"><a name="zh-cn_topic_0051408627_p30476837111434"></a><a name="zh-cn_topic_0051408627_p30476837111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p41227967111434"><a name="zh-cn_topic_0051408627_p41227967111434"></a><a name="zh-cn_topic_0051408627_p41227967111434"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row35507385111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p57525930111434"><a name="zh-cn_topic_0051408627_p57525930111434"></a><a name="zh-cn_topic_0051408627_p57525930111434"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p29088719111434"><a name="zh-cn_topic_0051408627_p29088719111434"></a><a name="zh-cn_topic_0051408627_p29088719111434"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p60586455111434"><a name="zh-cn_topic_0051408627_p60586455111434"></a><a name="zh-cn_topic_0051408627_p60586455111434"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row8407183111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p9893207111434"><a name="zh-cn_topic_0051408627_p9893207111434"></a><a name="zh-cn_topic_0051408627_p9893207111434"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p63152279111434"><a name="zh-cn_topic_0051408627_p63152279111434"></a><a name="zh-cn_topic_0051408627_p63152279111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p11980193111434"><a name="zh-cn_topic_0051408627_p11980193111434"></a><a name="zh-cn_topic_0051408627_p11980193111434"></a>租户ID。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row40712881111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p9409050111434"><a name="zh-cn_topic_0051408627_p9409050111434"></a><a name="zh-cn_topic_0051408627_p9409050111434"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p23935584111434"><a name="zh-cn_topic_0051408627_p23935584111434"></a><a name="zh-cn_topic_0051408627_p23935584111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p6625696111434"><a name="zh-cn_topic_0051408627_p6625696111434"></a><a name="zh-cn_topic_0051408627_p6625696111434"></a><span id="text4730642777"><a name="text4730642777"></a><a name="text4730642777"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="row11295723102014"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p95423280203"><a name="p95423280203"></a><a name="p95423280203"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1354218288209"><a name="p1354218288209"></a><a name="p1354218288209"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p845483673211"><a name="p845483673211"></a><a name="p845483673211"></a>预留属性。</p>
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
        
        "snapshots": [
            {
                "status": "available", 
                "os-extended-snapshot-attributes:progress": "100%", 
                "description": null, 
                "created_at": "2013-06-19T07:15:29.000000", 
                "metadata": { }, 
                "volume_id": "ae11e59c-bd56-434a-a00c-04757e1c066d", 
                "os-extended-snapshot-attributes:project_id": "d6c277ba8820452e83df36f33c9fa561", 
                "size": 5, 
                "id": "6cd26877-3ca3-4f4e-ae2a-38cc3d6183fa", 
                "name": "name_xx2-snap", 
                "updated_at": null, 
                "user_id": "48d70679b8644035846b2cb53633c256"
            }, 
            {
                "status": "available", 
                "os-extended-snapshot-attributes:progress": "100%", 
                "description": null, 
                "created_at": "2013-06-19T09:08:08.000000", 
                "metadata": { }, 
                "volume_id": "ae11e59c-bd56-434a-a00c-04757e1c066d", 
                "os-extended-snapshot-attributes:project_id": "d6c277ba8820452e83df36f33c9fa561", 
                "size": 5, 
                "id": "b3253e26-5c37-48dd-8bf2-8795dd1e848f", 
                "name": "name_xx2-snap", 
                "updated_at": null, 
                "user_id": "48d70679b8644035846b2cb53633c256"
            }
        ]
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


## 状态码<a name="section7038241111643"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

