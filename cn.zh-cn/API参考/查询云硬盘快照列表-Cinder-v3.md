# 查询云硬盘快照列表<a name="evs_04_3059"></a>

## 功能介绍<a name="section5262172611544"></a>

查询云硬盘快照列表。

## URI<a name="section1511931811555"></a>

-   URI格式

    GET /v3/\{project\_id\}/snapshots

-   参数说明

    <a name="table1448127211555"></a>
    <table><thead align="left"><tr id="row3175017111555"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p2162703411555"><a name="p2162703411555"></a><a name="p2162703411555"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p695931811555"><a name="p695931811555"></a><a name="p695931811555"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p2683384611555"><a name="p2683384611555"></a><a name="p2683384611555"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2605789011555"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p3031437111555"><a name="p3031437111555"></a><a name="p3031437111555"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3954502511555"><a name="p3954502511555"></a><a name="p3954502511555"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4903046711555"><a name="p4903046711555"></a><a name="p4903046711555"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   request filter参数说明

    <a name="evs_04_2096_table633033061168"></a>
    <table><thead align="left"><tr id="evs_04_2096_row57109071168"><th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.1.5.1.1"><p id="evs_04_2096_p599303181168"><a name="evs_04_2096_p599303181168"></a><a name="evs_04_2096_p599303181168"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.2"><p id="evs_04_2096_p225175981168"><a name="evs_04_2096_p225175981168"></a><a name="evs_04_2096_p225175981168"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="evs_04_2096_p119861301168"><a name="evs_04_2096_p119861301168"></a><a name="evs_04_2096_p119861301168"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="evs_04_2096_p313524671168"><a name="evs_04_2096_p313524671168"></a><a name="evs_04_2096_p313524671168"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1869818449417"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2068_p49168107152914"><a name="evs_04_2068_p49168107152914"></a><a name="evs_04_2068_p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2068_p23193765152914"><a name="evs_04_2068_p23193765152914"></a><a name="evs_04_2068_p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2068_p66755704152914"><a name="evs_04_2068_p66755704152914"></a><a name="evs_04_2068_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2068_p38502923152914"><a name="evs_04_2068_p38502923152914"></a><a name="evs_04_2068_p38502923152914"></a><span id="text127381323152311"><a name="text127381323152311"></a><a name="text127381323152311"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2096_row137367471168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2096_p389347291168"><a name="evs_04_2096_p389347291168"></a><a name="evs_04_2096_p389347291168"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2096_p667053841168"><a name="evs_04_2096_p667053841168"></a><a name="evs_04_2096_p667053841168"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2096_p344270561168"><a name="evs_04_2096_p344270561168"></a><a name="evs_04_2096_p344270561168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2096_p371281361168"><a name="evs_04_2096_p371281361168"></a><a name="evs_04_2096_p371281361168"></a>偏移量。</p>
    <div class="note" id="evs_04_2096_note6490498915441"><a name="evs_04_2096_note6490498915441"></a><a name="evs_04_2096_note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2096_p4727398915441"><a name="evs_04_2096_p4727398915441"></a><a name="evs_04_2096_p4727398915441"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2096_row657177691168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2096_p215391011168"><a name="evs_04_2096_p215391011168"></a><a name="evs_04_2096_p215391011168"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2096_p669456211168"><a name="evs_04_2096_p669456211168"></a><a name="evs_04_2096_p669456211168"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2096_p538862341168"><a name="evs_04_2096_p538862341168"></a><a name="evs_04_2096_p538862341168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2096_p27088191168"><a name="evs_04_2096_p27088191168"></a><a name="evs_04_2096_p27088191168"></a>返回结果个数限制。</p>
    <p id="p283195819137"><a name="p283195819137"></a><a name="p283195819137"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="evs_04_2096_p14657115572511"><a name="evs_04_2096_p14657115572511"></a><a name="evs_04_2096_p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="evs_04_2096_p1233994321914"><a name="evs_04_2096_p1233994321914"></a><a name="evs_04_2096_p1233994321914"></a><strong id="evs_04_2096_b15619135183016"><a name="evs_04_2096_b15619135183016"></a><a name="evs_04_2096_b15619135183016"></a>GET /v3/<em id="evs_04_2096_i86219512306"><a name="evs_04_2096_i86219512306"></a><a name="evs_04_2096_i86219512306"></a>xxx</em>/snapshots?limit=50</strong>，表示查询第1~50个快照。<strong id="evs_04_2096_b18611337305"><a name="evs_04_2096_b18611337305"></a><a name="evs_04_2096_b18611337305"></a>GET /v3/<em id="evs_04_2096_i149081817173015"><a name="evs_04_2096_i149081817173015"></a><a name="evs_04_2096_i149081817173015"></a>xxx</em>/snapshots?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row243793751168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2096_p285723381168"><a name="evs_04_2096_p285723381168"></a><a name="evs_04_2096_p285723381168"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2096_p326580131168"><a name="evs_04_2096_p326580131168"></a><a name="evs_04_2096_p326580131168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2096_p280534011168"><a name="evs_04_2096_p280534011168"></a><a name="evs_04_2096_p280534011168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2096_p577330051168"><a name="evs_04_2096_p577330051168"></a><a name="evs_04_2096_p577330051168"></a>云硬盘快照名称，不支持模糊匹配。<span id="evs_04_2096_text36369718152549"><a name="evs_04_2096_text36369718152549"></a><a name="evs_04_2096_text36369718152549"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row288521214459"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p463319195457"><a name="p463319195457"></a><a name="p463319195457"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p1163321984520"><a name="p1163321984520"></a><a name="p1163321984520"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p663321934517"><a name="p663321934517"></a><a name="p663321934517"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><div class="p" id="p1751520421266"><a name="p1751520421266"></a><a name="p1751520421266"></a>返回结果按照降序或升序排列，默认为“desc”。<a name="ul1729318471065"></a><a name="ul1729318471065"></a><ul id="ul1729318471065"><li>降序：desc</li><li>升序：asc</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2096_row498350041168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2096_p101035441168"><a name="evs_04_2096_p101035441168"></a><a name="evs_04_2096_p101035441168"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2096_p130807691168"><a name="evs_04_2096_p130807691168"></a><a name="evs_04_2096_p130807691168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2096_p529093741168"><a name="evs_04_2096_p529093741168"></a><a name="evs_04_2096_p529093741168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2096_p578009201168"><a name="evs_04_2096_p578009201168"></a><a name="evs_04_2096_p578009201168"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row504462351168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="evs_04_2096_p596132261168"><a name="evs_04_2096_p596132261168"></a><a name="evs_04_2096_p596132261168"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="evs_04_2096_p639420261168"><a name="evs_04_2096_p639420261168"></a><a name="evs_04_2096_p639420261168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="evs_04_2096_p119216351168"><a name="evs_04_2096_p119216351168"></a><a name="evs_04_2096_p119216351168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="evs_04_2096_p261283481168"><a name="evs_04_2096_p261283481168"></a><a name="evs_04_2096_p261283481168"></a>云硬盘快照对应的卷ID。</p>
    </td>
    </tr>
    <tr id="row3561144994516"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p1355262793315"><a name="p1355262793315"></a><a name="p1355262793315"></a>name~</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p15552102720334"><a name="p15552102720334"></a><a name="p15552102720334"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p12552102719334"><a name="p12552102719334"></a><a name="p12552102719334"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p11552182715331"><a name="p11552182715331"></a><a name="p11552182715331"></a>云硬盘名模糊查询，请求版本号为3.31及以上可支持该参数。</p>
    </td>
    </tr>
    <tr id="row9561144912457"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p555232714335"><a name="p555232714335"></a><a name="p555232714335"></a>status~</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p11553122753313"><a name="p11553122753313"></a><a name="p11553122753313"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1955322717338"><a name="p1955322717338"></a><a name="p1955322717338"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p25531427163315"><a name="p25531427163315"></a><a name="p25531427163315"></a>云硬盘状态模糊查询，请求版本号为3.31及以上可支持该参数。</p>
    </td>
    </tr>
    <tr id="row16561104944515"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p1268088124912"><a name="p1268088124912"></a><a name="p1268088124912"></a>volume_id~</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p1668012820493"><a name="p1668012820493"></a><a name="p1668012820493"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1968058154912"><a name="p1968058154912"></a><a name="p1968058154912"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p768018824914"><a name="p768018824914"></a><a name="p768018824914"></a>云硬盘快照对应的卷ID模糊查询，请求版本号为3.31及以上可支持该参数。</p>
    </td>
    </tr>
    <tr id="row1561249144519"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p668115818494"><a name="p668115818494"></a><a name="p668115818494"></a>sort_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p176812811492"><a name="p176812811492"></a><a name="p176812811492"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p468111819494"><a name="p468111819494"></a><a name="p468111819494"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p2068120884920"><a name="p2068120884920"></a><a name="p2068120884920"></a>基于name做排序查询，sort_key=name， 请求版本号为3.30及以上可支持name关键字，默认按照降序排序。</p>
    </td>
    </tr>
    <tr id="row3563124984516"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p155547276337"><a name="p155547276337"></a><a name="p155547276337"></a>with_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p855442773311"><a name="p855442773311"></a><a name="p855442773311"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1055420271339"><a name="p1055420271339"></a><a name="p1055420271339"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p26217111246"><a name="p26217111246"></a><a name="p26217111246"></a>返回结果增加counts参数，表示查询结果中的快照数量。格式为with_count=true，请求版本号为3.45及以上可支持该参数。</p>
    <p id="p1459918123014"><a name="p1459918123014"></a><a name="p1459918123014"></a>该参数仅可以和表中的marker、limit、sort_key、sort_dir或者offset参数一同使用，不支持和其他过滤参数共用。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询状态为available的云硬盘快照为例。

-   请求样例

    ```
    GET https://{endpoint}/v3/{project_id}/snapshots?status=available
    ```


## 响应消息<a name="section539031881175"></a>

-   响应参数

    <a name="table16791124318811"></a>
    <table><thead align="left"><tr id="row279119431881"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p147912431813"><a name="p147912431813"></a><a name="p147912431813"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p6791134320813"><a name="p6791134320813"></a><a name="p6791134320813"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p147911943187"><a name="p147911943187"></a><a name="p147911943187"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row11792943087"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p279264316818"><a name="p279264316818"></a><a name="p279264316818"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p1379218434810"><a name="p1379218434810"></a><a name="p1379218434810"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p879218431681"><a name="p879218431681"></a><a name="p879218431681"></a>快照信息，请参见<a href="#evs_04_2096_li367387041175">•snapshots参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row19562135513816"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p147911431788"><a name="p147911431788"></a><a name="p147911431788"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p1279210431813"><a name="p1279210431813"></a><a name="p1279210431813"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p163671041196"><a name="p163671041196"></a><a name="p163671041196"></a>云硬盘快照列表查询位置标记。当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="row1579418431988"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p1779412431788"><a name="p1779412431788"></a><a name="p1779412431788"></a>count</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2010_p159017261855"><a name="evs_04_2010_p159017261855"></a><a name="evs_04_2010_p159017261855"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p57949436815"><a name="p57949436815"></a><a name="p57949436815"></a>查询返回结果的数量。</p>
    </td>
    </tr>
    <tr id="row67494216911"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2010_p1595262111415"><a name="evs_04_2010_p1595262111415"></a><a name="evs_04_2010_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2096_li367387041175"></a>snapshots参数说明

    <a name="evs_04_2096_table622128841175"></a>
    <table><thead align="left"><tr id="evs_04_2096_row535860991175"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2096_p455067371175"><a name="evs_04_2096_p455067371175"></a><a name="evs_04_2096_p455067371175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2096_p621670471175"><a name="evs_04_2096_p621670471175"></a><a name="evs_04_2096_p621670471175"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2096_p574320291175"><a name="evs_04_2096_p574320291175"></a><a name="evs_04_2096_p574320291175"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2096_row505356201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p668534581175"><a name="evs_04_2096_p668534581175"></a><a name="evs_04_2096_p668534581175"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p464210281175"><a name="evs_04_2096_p464210281175"></a><a name="evs_04_2096_p464210281175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p283450141175"><a name="evs_04_2096_p283450141175"></a><a name="evs_04_2096_p283450141175"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row537785391175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p610943921175"><a name="evs_04_2096_p610943921175"></a><a name="evs_04_2096_p610943921175"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p496987011175"><a name="evs_04_2096_p496987011175"></a><a name="evs_04_2096_p496987011175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p583203691175"><a name="evs_04_2096_p583203691175"></a><a name="evs_04_2096_p583203691175"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row551212811175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p356388081175"><a name="evs_04_2096_p356388081175"></a><a name="evs_04_2096_p356388081175"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p10622981175"><a name="evs_04_2096_p10622981175"></a><a name="evs_04_2096_p10622981175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p575287091175"><a name="evs_04_2096_p575287091175"></a><a name="evs_04_2096_p575287091175"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row479963371175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p624980901175"><a name="evs_04_2096_p624980901175"></a><a name="evs_04_2096_p624980901175"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p291805641175"><a name="evs_04_2096_p291805641175"></a><a name="evs_04_2096_p291805641175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p592057221175"><a name="evs_04_2096_p592057221175"></a><a name="evs_04_2096_p592057221175"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row630894511175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p99718891175"><a name="evs_04_2096_p99718891175"></a><a name="evs_04_2096_p99718891175"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p24167171175"><a name="evs_04_2096_p24167171175"></a><a name="evs_04_2096_p24167171175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p183889601175"><a name="evs_04_2096_p183889601175"></a><a name="evs_04_2096_p183889601175"></a>云硬盘快照创建时间。</p>
    <p id="p181121789819"><a name="p181121789819"></a><a name="p181121789819"></a><span id="text1271511210811"><a name="text1271511210811"></a><a name="text1271511210811"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2096_row312829201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p508885661175"><a name="evs_04_2096_p508885661175"></a><a name="evs_04_2096_p508885661175"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p283331481175"><a name="evs_04_2096_p283331481175"></a><a name="evs_04_2096_p283331481175"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p22339381175"><a name="evs_04_2096_p22339381175"></a><a name="evs_04_2096_p22339381175"></a>云硬盘快照的元数据信息。</p>
    <p id="p1678772717473"><a name="p1678772717473"></a><a name="p1678772717473"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row201054491175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p179286481175"><a name="evs_04_2096_p179286481175"></a><a name="evs_04_2096_p179286481175"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p429343721175"><a name="evs_04_2096_p429343721175"></a><a name="evs_04_2096_p429343721175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p365124961175"><a name="evs_04_2096_p365124961175"></a><a name="evs_04_2096_p365124961175"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row601770151175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p425000331175"><a name="evs_04_2096_p425000331175"></a><a name="evs_04_2096_p425000331175"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p199506681175"><a name="evs_04_2096_p199506681175"></a><a name="evs_04_2096_p199506681175"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p340521631175"><a name="evs_04_2096_p340521631175"></a><a name="evs_04_2096_p340521631175"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="evs_04_2096_row380340191175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2096_p608567071175"><a name="evs_04_2096_p608567071175"></a><a name="evs_04_2096_p608567071175"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2096_p304462151175"><a name="evs_04_2096_p304462151175"></a><a name="evs_04_2096_p304462151175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2096_p416400291175"><a name="evs_04_2096_p416400291175"></a><a name="evs_04_2096_p416400291175"></a>快照更新时间。</p>
    <p id="p133850207816"><a name="p133850207816"></a><a name="p133850207816"></a><span id="text186649201488"><a name="text186649201488"></a><a name="text186649201488"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
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
    <p id="evs_04_2013_p54787218103019"><a name="evs_04_2013_p54787218103019"></a><a name="evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "count": 4, 
        "snapshots": [
            {
                "created_at": "2016-02-16T16:54:14.981520", 
                "description": null, 
                "id": "b836dc3d-4e10-4ea4-a34c-8f6b0460a583", 
                "metadata": { }, 
                "name": "test01", 
                "size": 1, 
                "status": "available", 
                "volume_id": "ba5730ea-8621-4ae8-b702-ff0ffc12c209", 
                "updated_at": null
            }, 
            {
                "created_at": "2016-02-16T16:54:19.475397", 
                "description": null, 
                "id": "83be494d-329e-4a78-8ac5-9af900f48b95", 
                "metadata": { }, 
                "name": "test02", 
                "size": 1, 
                "status": "available", 
                "volume_id": "ba5730ea-8621-4ae8-b702-ff0ffc12c209", 
                "updated_at": null
            }, 
            {
                "created_at": "2016-02-16T16:54:24.367414", 
                "description": null, 
                "id": "dd360f46-7593-4d35-8f2c-5566fd0bd79e", 
                "metadata": { }, 
                "name": "test03", 
                "size": 1, 
                "status": "available", 
                "volume_id": "ba5730ea-8621-4ae8-b702-ff0ffc12c209", 
                "updated_at": null
            }, 
            {
                "created_at": "2016-02-16T16:54:29.766740", 
                "description": null, 
                "id": "4c29796a-8cf4-4482-9afc-e66da9a81240", 
                "metadata": { }, 
                "name": "test04", 
                "size": 1, 
                "status": "available", 
                "volume_id": "ba5730ea-8621-4ae8-b702-ff0ffc12c209", 
                "updated_at": null
            }
        ], 
        "snapshots_links": null
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


## 状态码<a name="section4644965111956"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

