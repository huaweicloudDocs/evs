# 查询云硬盘快照详细信息列表<a name="zh-cn_topic_0051408627"></a>

## 功能介绍<a name="section63129217111110"></a>

查询云硬盘快照详细列表信息。

## URI<a name="section21460443111127"></a>

-   URI格式

    GET /v2/\{project\_id\}/snapshots/detail

-   参数说明

    <a name="table9361875111127"></a>
    <table><thead align="left"><tr id="row34794340111127"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p1481016775815"><a name="p1481016775815"></a><a name="p1481016775815"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p48423414111127"><a name="p48423414111127"></a><a name="p48423414111127"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p29982470111127"><a name="p29982470111127"></a><a name="p29982470111127"></a>描述</p>
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

    <a name="table49657902111140"></a>
    <table><thead align="left"><tr id="row47265217111140"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="p3277402111140"><a name="p3277402111140"></a><a name="p3277402111140"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="p64143015111140"><a name="p64143015111140"></a><a name="p64143015111140"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p28201745111140"><a name="p28201745111140"></a><a name="p28201745111140"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="p2639999111140"><a name="p2639999111140"></a><a name="p2639999111140"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15925102920245"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762430_p49168107152914"><a name="zh-cn_topic_0058762430_p49168107152914"></a><a name="zh-cn_topic_0058762430_p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762430_p23193765152914"><a name="zh-cn_topic_0058762430_p23193765152914"></a><a name="zh-cn_topic_0058762430_p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762430_p66755704152914"><a name="zh-cn_topic_0058762430_p66755704152914"></a><a name="zh-cn_topic_0058762430_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762430_p38502923152914"><a name="zh-cn_topic_0058762430_p38502923152914"></a><a name="zh-cn_topic_0058762430_p38502923152914"></a><span id="text127381323152311"><a name="text127381323152311"></a><a name="text127381323152311"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="row23759995111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p45511467111140"><a name="p45511467111140"></a><a name="p45511467111140"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p62550228111140"><a name="p62550228111140"></a><a name="p62550228111140"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p33403677111140"><a name="p33403677111140"></a><a name="p33403677111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p21343278111140"><a name="p21343278111140"></a><a name="p21343278111140"></a>偏移量。</p>
    <div class="note" id="note6490498915441"><a name="note6490498915441"></a><a name="note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p4727398915441"><a name="p4727398915441"></a><a name="p4727398915441"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row57871777111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p57102386111140"><a name="p57102386111140"></a><a name="p57102386111140"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p61890592111140"><a name="p61890592111140"></a><a name="p61890592111140"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p47082066111140"><a name="p47082066111140"></a><a name="p47082066111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p55551025111140"><a name="p55551025111140"></a><a name="p55551025111140"></a>返回结果个数限制。</p>
    <p id="p8961131111161"><a name="p8961131111161"></a><a name="p8961131111161"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="p14657115572511"><a name="p14657115572511"></a><a name="p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="p1233994321914"><a name="p1233994321914"></a><a name="p1233994321914"></a><strong id="b15619135183016"><a name="b15619135183016"></a><a name="b15619135183016"></a>GET /v2/<em id="i86219512306"><a name="i86219512306"></a><a name="i86219512306"></a>xxx</em>/snapshots/detail?limit=50</strong>，表示查询第1~50个快照。<strong id="b18611337305"><a name="b18611337305"></a><a name="b18611337305"></a>GET /v2/<em id="i149081817173015"><a name="i149081817173015"></a><a name="i149081817173015"></a>xxx</em>/snapshots/detail?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="row30197180111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p30052553111140"><a name="p30052553111140"></a><a name="p30052553111140"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p18337718111140"><a name="p18337718111140"></a><a name="p18337718111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p8960171111140"><a name="p8960171111140"></a><a name="p8960171111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p54685265111140"><a name="p54685265111140"></a><a name="p54685265111140"></a>云硬盘快照名称。最大支持255个字节。</p>
    </td>
    </tr>
    <tr id="row22405342111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p2893391111140"><a name="p2893391111140"></a><a name="p2893391111140"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p33038150111140"><a name="p33038150111140"></a><a name="p33038150111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p58844456111140"><a name="p58844456111140"></a><a name="p58844456111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p1671647111140"><a name="p1671647111140"></a><a name="p1671647111140"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row15044830111140"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p10671727111140"><a name="p10671727111140"></a><a name="p10671727111140"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="p59103560111140"><a name="p59103560111140"></a><a name="p59103560111140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p22659090111140"><a name="p22659090111140"></a><a name="p22659090111140"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="p23447029111140"><a name="p23447029111140"></a><a name="p23447029111140"></a>云硬盘快照对应的云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询状态为available的云硬盘快照为例。

-   请求样例

    ```
    GET https://{endpoint}/v2/{project_id}/snapshots/detail?status=available
    ```


## 响应消息<a name="section3672851111434"></a>

-   响应参数

    <a name="table1216812421519"></a>
    <table><thead align="left"><tr id="row191683423115"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p816844211113"><a name="p816844211113"></a><a name="p816844211113"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p316813421914"><a name="p316813421914"></a><a name="p316813421914"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p71681426114"><a name="p71681426114"></a><a name="p71681426114"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row19169242411"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p91690422118"><a name="p91690422118"></a><a name="p91690422118"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p816964217110"><a name="p816964217110"></a><a name="p816964217110"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p19169114217115"><a name="p19169114217115"></a><a name="p19169114217115"></a>快照信息，请参见<a href="#li60262741111434">•snapshots参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row5430105519414"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p41699425112"><a name="p41699425112"></a><a name="p41699425112"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1116954219116"><a name="p1116954219116"></a><a name="p1116954219116"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p171691426114"><a name="p171691426114"></a><a name="p171691426114"></a>云硬盘快照列表查询位置标记。当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="row2016914421012"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li60262741111434"></a>snapshots参数说明

    <a name="table5493760111434"></a>
    <table><thead align="left"><tr id="row9951929111434"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p799881111434"><a name="p799881111434"></a><a name="p799881111434"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.38%" id="mcps1.1.4.1.2"><p id="p64790373111434"><a name="p64790373111434"></a><a name="p64790373111434"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.19%" id="mcps1.1.4.1.3"><p id="p22098020111434"><a name="p22098020111434"></a><a name="p22098020111434"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row30338895111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p41531445111434"><a name="p41531445111434"></a><a name="p41531445111434"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p8603891111434"><a name="p8603891111434"></a><a name="p8603891111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p11580698111434"><a name="p11580698111434"></a><a name="p11580698111434"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row37117420111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p53721059111434"><a name="p53721059111434"></a><a name="p53721059111434"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p56438551111434"><a name="p56438551111434"></a><a name="p56438551111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p53733716111434"><a name="p53733716111434"></a><a name="p53733716111434"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row13841398111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p47411481111434"><a name="p47411481111434"></a><a name="p47411481111434"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p15124732111434"><a name="p15124732111434"></a><a name="p15124732111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p46466595111434"><a name="p46466595111434"></a><a name="p46466595111434"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row15546175111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p51280630111434"><a name="p51280630111434"></a><a name="p51280630111434"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p60090386111434"><a name="p60090386111434"></a><a name="p60090386111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p55561368111434"><a name="p55561368111434"></a><a name="p55561368111434"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row30290270111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p37592805111434"><a name="p37592805111434"></a><a name="p37592805111434"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p25118356111434"><a name="p25118356111434"></a><a name="p25118356111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p49277837111434"><a name="p49277837111434"></a><a name="p49277837111434"></a>云硬盘快照创建时间。</p>
    <p id="p122996220414"><a name="p122996220414"></a><a name="p122996220414"></a><span id="text1292720311749"><a name="text1292720311749"></a><a name="text1292720311749"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row62090946113559"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p4553543411364"><a name="p4553543411364"></a><a name="p4553543411364"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p6449156711364"><a name="p6449156711364"></a><a name="p6449156711364"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p778860311364"><a name="p778860311364"></a><a name="p778860311364"></a>云硬盘快照更新时间。</p>
    <p id="p932912241842"><a name="p932912241842"></a><a name="p932912241842"></a><span id="text1710311361547"><a name="text1710311361547"></a><a name="text1710311361547"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row40847350111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p20301014111434"><a name="p20301014111434"></a><a name="p20301014111434"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p33769410111434"><a name="p33769410111434"></a><a name="p33769410111434"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p34744289111434"><a name="p34744289111434"></a><a name="p34744289111434"></a>云硬盘快照的元数据信息。</p>
    <p id="p1961415054619"><a name="p1961415054619"></a><a name="p1961415054619"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="row44263150111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p28545410111434"><a name="p28545410111434"></a><a name="p28545410111434"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p30476837111434"><a name="p30476837111434"></a><a name="p30476837111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p41227967111434"><a name="p41227967111434"></a><a name="p41227967111434"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row35507385111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p57525930111434"><a name="p57525930111434"></a><a name="p57525930111434"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p29088719111434"><a name="p29088719111434"></a><a name="p29088719111434"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p60586455111434"><a name="p60586455111434"></a><a name="p60586455111434"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="row8407183111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p9893207111434"><a name="p9893207111434"></a><a name="p9893207111434"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p63152279111434"><a name="p63152279111434"></a><a name="p63152279111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p11980193111434"><a name="p11980193111434"></a><a name="p11980193111434"></a>租户ID。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="row40712881111434"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p9409050111434"><a name="p9409050111434"></a><a name="p9409050111434"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.38%" headers="mcps1.1.4.1.2 "><p id="p23935584111434"><a name="p23935584111434"></a><a name="p23935584111434"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.19%" headers="mcps1.1.4.1.3 "><p id="p6625696111434"><a name="p6625696111434"></a><a name="p6625696111434"></a><span id="text4730642777"><a name="text4730642777"></a><a name="text4730642777"></a>预留属性。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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


## 状态码<a name="section7038241111643"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

