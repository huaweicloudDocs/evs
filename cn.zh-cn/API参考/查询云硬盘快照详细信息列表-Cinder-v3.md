# 查询云硬盘快照详细信息列表<a name="ZH-CN_TOPIC_0102702649"></a>

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
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section35052604111140"></a>

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
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762430_p23193765152914"><a name="zh-cn_topic_0058762430_p23193765152914"></a><a name="zh-cn_topic_0058762430_p23193765152914"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762430_p66755704152914"><a name="zh-cn_topic_0058762430_p66755704152914"></a><a name="zh-cn_topic_0058762430_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762430_p38502923152914"><a name="zh-cn_topic_0058762430_p38502923152914"></a><a name="zh-cn_topic_0058762430_p38502923152914"></a>取值为上一页数据的最后一条记录的id，返回值为该项后面的项。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row23759995111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p45511467111140"><a name="zh-cn_topic_0051408627_p45511467111140"></a><a name="zh-cn_topic_0051408627_p45511467111140"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p62550228111140"><a name="zh-cn_topic_0051408627_p62550228111140"></a><a name="zh-cn_topic_0051408627_p62550228111140"></a>int</p>
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
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p61890592111140"><a name="zh-cn_topic_0051408627_p61890592111140"></a><a name="zh-cn_topic_0051408627_p61890592111140"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p47082066111140"><a name="zh-cn_topic_0051408627_p47082066111140"></a><a name="zh-cn_topic_0051408627_p47082066111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p55551025111140"><a name="zh-cn_topic_0051408627_p55551025111140"></a><a name="zh-cn_topic_0051408627_p55551025111140"></a>返回结果个数限制，值为大于0的整数。默认值为1000。</p>
    <p id="zh-cn_topic_0051408627_p14657115572511"><a name="zh-cn_topic_0051408627_p14657115572511"></a><a name="zh-cn_topic_0051408627_p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="zh-cn_topic_0051408627_p1233994321914"><a name="zh-cn_topic_0051408627_p1233994321914"></a><a name="zh-cn_topic_0051408627_p1233994321914"></a><strong id="zh-cn_topic_0051408627_b15619135183016"><a name="zh-cn_topic_0051408627_b15619135183016"></a><a name="zh-cn_topic_0051408627_b15619135183016"></a>GET /v2/<em id="zh-cn_topic_0051408627_i86219512306"><a name="zh-cn_topic_0051408627_i86219512306"></a><a name="zh-cn_topic_0051408627_i86219512306"></a>xxx</em>/snapshots/detail?limit=50</strong>，表示查询第1~50个快照。<strong id="zh-cn_topic_0051408627_b18611337305"><a name="zh-cn_topic_0051408627_b18611337305"></a><a name="zh-cn_topic_0051408627_b18611337305"></a>GET /v2/<em id="zh-cn_topic_0051408627_i149081817173015"><a name="zh-cn_topic_0051408627_i149081817173015"></a><a name="zh-cn_topic_0051408627_i149081817173015"></a>xxx</em>/snapshots/detail?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row30197180111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p30052553111140"><a name="zh-cn_topic_0051408627_p30052553111140"></a><a name="zh-cn_topic_0051408627_p30052553111140"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p18337718111140"><a name="zh-cn_topic_0051408627_p18337718111140"></a><a name="zh-cn_topic_0051408627_p18337718111140"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p8960171111140"><a name="zh-cn_topic_0051408627_p8960171111140"></a><a name="zh-cn_topic_0051408627_p8960171111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p54685265111140"><a name="zh-cn_topic_0051408627_p54685265111140"></a><a name="zh-cn_topic_0051408627_p54685265111140"></a>云硬盘快照名称。最大支持255个字节。</p>
    </td>
    </tr>
    <tr id="row475111724717"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p463319195457"><a name="p463319195457"></a><a name="p463319195457"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p1163321984520"><a name="p1163321984520"></a><a name="p1163321984520"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p663321934517"><a name="p663321934517"></a><a name="p663321934517"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p063361915456"><a name="p063361915456"></a><a name="p063361915456"></a>降序或升序，默认为“desc”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row22405342111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p2893391111140"><a name="zh-cn_topic_0051408627_p2893391111140"></a><a name="zh-cn_topic_0051408627_p2893391111140"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p33038150111140"><a name="zh-cn_topic_0051408627_p33038150111140"></a><a name="zh-cn_topic_0051408627_p33038150111140"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p58844456111140"><a name="zh-cn_topic_0051408627_p58844456111140"></a><a name="zh-cn_topic_0051408627_p58844456111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p1671647111140"><a name="zh-cn_topic_0051408627_p1671647111140"></a><a name="zh-cn_topic_0051408627_p1671647111140"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row15044830111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408627_p10671727111140"><a name="zh-cn_topic_0051408627_p10671727111140"></a><a name="zh-cn_topic_0051408627_p10671727111140"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408627_p59103560111140"><a name="zh-cn_topic_0051408627_p59103560111140"></a><a name="zh-cn_topic_0051408627_p59103560111140"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408627_p22659090111140"><a name="zh-cn_topic_0051408627_p22659090111140"></a><a name="zh-cn_topic_0051408627_p22659090111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408627_p23447029111140"><a name="zh-cn_topic_0051408627_p23447029111140"></a><a name="zh-cn_topic_0051408627_p23447029111140"></a>云硬盘快照对应的云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    无


## 响应<a name="section3672851111434"></a>

-   响应参数

    <a name="zh-cn_topic_0051408627_table5493760111434"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408627_row9951929111434"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408627_p799881111434"><a name="zh-cn_topic_0051408627_p799881111434"></a><a name="zh-cn_topic_0051408627_p799881111434"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408627_p64790373111434"><a name="zh-cn_topic_0051408627_p64790373111434"></a><a name="zh-cn_topic_0051408627_p64790373111434"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408627_p22098020111434"><a name="zh-cn_topic_0051408627_p22098020111434"></a><a name="zh-cn_topic_0051408627_p22098020111434"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408627_row53717437104420"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p44332405104423"><a name="zh-cn_topic_0051408627_p44332405104423"></a><a name="zh-cn_topic_0051408627_p44332405104423"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p34155089104423"><a name="zh-cn_topic_0051408627_p34155089104423"></a><a name="zh-cn_topic_0051408627_p34155089104423"></a>list&lt;map&lt;string,string&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p15042660104423"><a name="zh-cn_topic_0051408627_p15042660104423"></a><a name="zh-cn_topic_0051408627_p15042660104423"></a>云硬盘快照列表查询位置标记，与响应body中的snapshots同级，当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row45109206111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p29967093111434"><a name="zh-cn_topic_0051408627_p29967093111434"></a><a name="zh-cn_topic_0051408627_p29967093111434"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p11415464111434"><a name="zh-cn_topic_0051408627_p11415464111434"></a><a name="zh-cn_topic_0051408627_p11415464111434"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p3370988111434"><a name="zh-cn_topic_0051408627_p3370988111434"></a><a name="zh-cn_topic_0051408627_p3370988111434"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row30338895111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p41531445111434"><a name="zh-cn_topic_0051408627_p41531445111434"></a><a name="zh-cn_topic_0051408627_p41531445111434"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p8603891111434"><a name="zh-cn_topic_0051408627_p8603891111434"></a><a name="zh-cn_topic_0051408627_p8603891111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p11580698111434"><a name="zh-cn_topic_0051408627_p11580698111434"></a><a name="zh-cn_topic_0051408627_p11580698111434"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row37117420111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p53721059111434"><a name="zh-cn_topic_0051408627_p53721059111434"></a><a name="zh-cn_topic_0051408627_p53721059111434"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p56438551111434"><a name="zh-cn_topic_0051408627_p56438551111434"></a><a name="zh-cn_topic_0051408627_p56438551111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p53733716111434"><a name="zh-cn_topic_0051408627_p53733716111434"></a><a name="zh-cn_topic_0051408627_p53733716111434"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row13841398111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p47411481111434"><a name="zh-cn_topic_0051408627_p47411481111434"></a><a name="zh-cn_topic_0051408627_p47411481111434"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p15124732111434"><a name="zh-cn_topic_0051408627_p15124732111434"></a><a name="zh-cn_topic_0051408627_p15124732111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p46466595111434"><a name="zh-cn_topic_0051408627_p46466595111434"></a><a name="zh-cn_topic_0051408627_p46466595111434"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row15546175111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p51280630111434"><a name="zh-cn_topic_0051408627_p51280630111434"></a><a name="zh-cn_topic_0051408627_p51280630111434"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p60090386111434"><a name="zh-cn_topic_0051408627_p60090386111434"></a><a name="zh-cn_topic_0051408627_p60090386111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p55561368111434"><a name="zh-cn_topic_0051408627_p55561368111434"></a><a name="zh-cn_topic_0051408627_p55561368111434"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row30290270111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p37592805111434"><a name="zh-cn_topic_0051408627_p37592805111434"></a><a name="zh-cn_topic_0051408627_p37592805111434"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p25118356111434"><a name="zh-cn_topic_0051408627_p25118356111434"></a><a name="zh-cn_topic_0051408627_p25118356111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p49277837111434"><a name="zh-cn_topic_0051408627_p49277837111434"></a><a name="zh-cn_topic_0051408627_p49277837111434"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row62090946113559"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p4553543411364"><a name="zh-cn_topic_0051408627_p4553543411364"></a><a name="zh-cn_topic_0051408627_p4553543411364"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p6449156711364"><a name="zh-cn_topic_0051408627_p6449156711364"></a><a name="zh-cn_topic_0051408627_p6449156711364"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p778860311364"><a name="zh-cn_topic_0051408627_p778860311364"></a><a name="zh-cn_topic_0051408627_p778860311364"></a>云硬盘快照更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row40847350111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p20301014111434"><a name="zh-cn_topic_0051408627_p20301014111434"></a><a name="zh-cn_topic_0051408627_p20301014111434"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p33769410111434"><a name="zh-cn_topic_0051408627_p33769410111434"></a><a name="zh-cn_topic_0051408627_p33769410111434"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p34744289111434"><a name="zh-cn_topic_0051408627_p34744289111434"></a><a name="zh-cn_topic_0051408627_p34744289111434"></a>云硬盘快照的元数据信息。</p>
    <p id="p1678772717473"><a name="p1678772717473"></a><a name="p1678772717473"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row44263150111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p28545410111434"><a name="zh-cn_topic_0051408627_p28545410111434"></a><a name="zh-cn_topic_0051408627_p28545410111434"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p30476837111434"><a name="zh-cn_topic_0051408627_p30476837111434"></a><a name="zh-cn_topic_0051408627_p30476837111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p41227967111434"><a name="zh-cn_topic_0051408627_p41227967111434"></a><a name="zh-cn_topic_0051408627_p41227967111434"></a>快照所属的云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row35507385111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p57525930111434"><a name="zh-cn_topic_0051408627_p57525930111434"></a><a name="zh-cn_topic_0051408627_p57525930111434"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p29088719111434"><a name="zh-cn_topic_0051408627_p29088719111434"></a><a name="zh-cn_topic_0051408627_p29088719111434"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p60586455111434"><a name="zh-cn_topic_0051408627_p60586455111434"></a><a name="zh-cn_topic_0051408627_p60586455111434"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row8407183111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p9893207111434"><a name="zh-cn_topic_0051408627_p9893207111434"></a><a name="zh-cn_topic_0051408627_p9893207111434"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p63152279111434"><a name="zh-cn_topic_0051408627_p63152279111434"></a><a name="zh-cn_topic_0051408627_p63152279111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p11980193111434"><a name="zh-cn_topic_0051408627_p11980193111434"></a><a name="zh-cn_topic_0051408627_p11980193111434"></a>租户ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408627_row40712881111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408627_p9409050111434"><a name="zh-cn_topic_0051408627_p9409050111434"></a><a name="zh-cn_topic_0051408627_p9409050111434"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408627_p23935584111434"><a name="zh-cn_topic_0051408627_p23935584111434"></a><a name="zh-cn_topic_0051408627_p23935584111434"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408627_p6625696111434"><a name="zh-cn_topic_0051408627_p6625696111434"></a><a name="zh-cn_topic_0051408627_p6625696111434"></a>快照进度。</p>
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
                "updated_at": null
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
                "updated_at": null
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


## 返回值<a name="section7038241111643"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

