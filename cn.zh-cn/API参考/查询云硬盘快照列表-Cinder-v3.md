# 查询云硬盘快照列表<a name="ZH-CN_TOPIC_0102698940"></a>

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
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section282395511168"></a>

-   request filter参数说明

    <a name="zh-cn_topic_0051408626_table633033061168"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408626_row57109071168"><th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0051408626_p599303181168"><a name="zh-cn_topic_0051408626_p599303181168"></a><a name="zh-cn_topic_0051408626_p599303181168"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0051408626_p225175981168"><a name="zh-cn_topic_0051408626_p225175981168"></a><a name="zh-cn_topic_0051408626_p225175981168"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0051408626_p119861301168"><a name="zh-cn_topic_0051408626_p119861301168"></a><a name="zh-cn_topic_0051408626_p119861301168"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0051408626_p313524671168"><a name="zh-cn_topic_0051408626_p313524671168"></a><a name="zh-cn_topic_0051408626_p313524671168"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1869818449417"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762430_p49168107152914"><a name="zh-cn_topic_0058762430_p49168107152914"></a><a name="zh-cn_topic_0058762430_p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762430_p23193765152914"><a name="zh-cn_topic_0058762430_p23193765152914"></a><a name="zh-cn_topic_0058762430_p23193765152914"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762430_p66755704152914"><a name="zh-cn_topic_0058762430_p66755704152914"></a><a name="zh-cn_topic_0058762430_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762430_p38502923152914"><a name="zh-cn_topic_0058762430_p38502923152914"></a><a name="zh-cn_topic_0058762430_p38502923152914"></a>取值为上一页数据的最后一条记录的id，返回值为该项后面的项。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row137367471168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408626_p389347291168"><a name="zh-cn_topic_0051408626_p389347291168"></a><a name="zh-cn_topic_0051408626_p389347291168"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408626_p667053841168"><a name="zh-cn_topic_0051408626_p667053841168"></a><a name="zh-cn_topic_0051408626_p667053841168"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408626_p344270561168"><a name="zh-cn_topic_0051408626_p344270561168"></a><a name="zh-cn_topic_0051408626_p344270561168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408626_p371281361168"><a name="zh-cn_topic_0051408626_p371281361168"></a><a name="zh-cn_topic_0051408626_p371281361168"></a>偏移量。</p>
    <div class="note" id="zh-cn_topic_0051408626_note6490498915441"><a name="zh-cn_topic_0051408626_note6490498915441"></a><a name="zh-cn_topic_0051408626_note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0051408626_p4727398915441"><a name="zh-cn_topic_0051408626_p4727398915441"></a><a name="zh-cn_topic_0051408626_p4727398915441"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row657177691168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408626_p215391011168"><a name="zh-cn_topic_0051408626_p215391011168"></a><a name="zh-cn_topic_0051408626_p215391011168"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408626_p669456211168"><a name="zh-cn_topic_0051408626_p669456211168"></a><a name="zh-cn_topic_0051408626_p669456211168"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408626_p538862341168"><a name="zh-cn_topic_0051408626_p538862341168"></a><a name="zh-cn_topic_0051408626_p538862341168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408626_p27088191168"><a name="zh-cn_topic_0051408626_p27088191168"></a><a name="zh-cn_topic_0051408626_p27088191168"></a>返回结果个数限制，值为大于0的整数。默认值为1000。</p>
    <p id="zh-cn_topic_0051408626_p14657115572511"><a name="zh-cn_topic_0051408626_p14657115572511"></a><a name="zh-cn_topic_0051408626_p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="zh-cn_topic_0051408626_p1233994321914"><a name="zh-cn_topic_0051408626_p1233994321914"></a><a name="zh-cn_topic_0051408626_p1233994321914"></a><strong id="zh-cn_topic_0051408626_b15619135183016"><a name="zh-cn_topic_0051408626_b15619135183016"></a><a name="zh-cn_topic_0051408626_b15619135183016"></a>GET /v2/<em id="zh-cn_topic_0051408626_i86219512306"><a name="zh-cn_topic_0051408626_i86219512306"></a><a name="zh-cn_topic_0051408626_i86219512306"></a>xxx</em>/snapshots?limit=50</strong>，表示查询第1~50个快照。<strong id="zh-cn_topic_0051408626_b18611337305"><a name="zh-cn_topic_0051408626_b18611337305"></a><a name="zh-cn_topic_0051408626_b18611337305"></a>GET /v2/<em id="zh-cn_topic_0051408626_i149081817173015"><a name="zh-cn_topic_0051408626_i149081817173015"></a><a name="zh-cn_topic_0051408626_i149081817173015"></a>xxx</em>/snapshots?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row243793751168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408626_p285723381168"><a name="zh-cn_topic_0051408626_p285723381168"></a><a name="zh-cn_topic_0051408626_p285723381168"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408626_p326580131168"><a name="zh-cn_topic_0051408626_p326580131168"></a><a name="zh-cn_topic_0051408626_p326580131168"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408626_p280534011168"><a name="zh-cn_topic_0051408626_p280534011168"></a><a name="zh-cn_topic_0051408626_p280534011168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408626_p577330051168"><a name="zh-cn_topic_0051408626_p577330051168"></a><a name="zh-cn_topic_0051408626_p577330051168"></a>云硬盘快照名称，不支持模糊匹配。<span id="zh-cn_topic_0051408626_text36369718152549"><a name="zh-cn_topic_0051408626_text36369718152549"></a><a name="zh-cn_topic_0051408626_text36369718152549"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row288521214459"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p463319195457"><a name="p463319195457"></a><a name="p463319195457"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p1163321984520"><a name="p1163321984520"></a><a name="p1163321984520"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p663321934517"><a name="p663321934517"></a><a name="p663321934517"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p063361915456"><a name="p063361915456"></a><a name="p063361915456"></a>降序或升序，默认为“desc”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row498350041168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408626_p101035441168"><a name="zh-cn_topic_0051408626_p101035441168"></a><a name="zh-cn_topic_0051408626_p101035441168"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408626_p130807691168"><a name="zh-cn_topic_0051408626_p130807691168"></a><a name="zh-cn_topic_0051408626_p130807691168"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408626_p529093741168"><a name="zh-cn_topic_0051408626_p529093741168"></a><a name="zh-cn_topic_0051408626_p529093741168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408626_p578009201168"><a name="zh-cn_topic_0051408626_p578009201168"></a><a name="zh-cn_topic_0051408626_p578009201168"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row504462351168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408626_p596132261168"><a name="zh-cn_topic_0051408626_p596132261168"></a><a name="zh-cn_topic_0051408626_p596132261168"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408626_p639420261168"><a name="zh-cn_topic_0051408626_p639420261168"></a><a name="zh-cn_topic_0051408626_p639420261168"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408626_p119216351168"><a name="zh-cn_topic_0051408626_p119216351168"></a><a name="zh-cn_topic_0051408626_p119216351168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408626_p261283481168"><a name="zh-cn_topic_0051408626_p261283481168"></a><a name="zh-cn_topic_0051408626_p261283481168"></a>云硬盘快照对应的卷ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    无


## 响应<a name="section539031881175"></a>

-   响应参数

    <a name="zh-cn_topic_0051408626_table622128841175"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408626_row535860991175"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408626_p455067371175"><a name="zh-cn_topic_0051408626_p455067371175"></a><a name="zh-cn_topic_0051408626_p455067371175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408626_p621670471175"><a name="zh-cn_topic_0051408626_p621670471175"></a><a name="zh-cn_topic_0051408626_p621670471175"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408626_p574320291175"><a name="zh-cn_topic_0051408626_p574320291175"></a><a name="zh-cn_topic_0051408626_p574320291175"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408626_row6562497210425"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p4264686310429"><a name="zh-cn_topic_0051408626_p4264686310429"></a><a name="zh-cn_topic_0051408626_p4264686310429"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p3184386910429"><a name="zh-cn_topic_0051408626_p3184386910429"></a><a name="zh-cn_topic_0051408626_p3184386910429"></a>list&lt;map&lt;string,string&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p1773437510429"><a name="zh-cn_topic_0051408626_p1773437510429"></a><a name="zh-cn_topic_0051408626_p1773437510429"></a>云硬盘快照列表查询位置标记，与响应body中的snapshots同级，当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row214827971175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p623850141175"><a name="zh-cn_topic_0051408626_p623850141175"></a><a name="zh-cn_topic_0051408626_p623850141175"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p200213431175"><a name="zh-cn_topic_0051408626_p200213431175"></a><a name="zh-cn_topic_0051408626_p200213431175"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p279846901175"><a name="zh-cn_topic_0051408626_p279846901175"></a><a name="zh-cn_topic_0051408626_p279846901175"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row505356201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p668534581175"><a name="zh-cn_topic_0051408626_p668534581175"></a><a name="zh-cn_topic_0051408626_p668534581175"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p464210281175"><a name="zh-cn_topic_0051408626_p464210281175"></a><a name="zh-cn_topic_0051408626_p464210281175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p283450141175"><a name="zh-cn_topic_0051408626_p283450141175"></a><a name="zh-cn_topic_0051408626_p283450141175"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row537785391175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p610943921175"><a name="zh-cn_topic_0051408626_p610943921175"></a><a name="zh-cn_topic_0051408626_p610943921175"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p496987011175"><a name="zh-cn_topic_0051408626_p496987011175"></a><a name="zh-cn_topic_0051408626_p496987011175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p583203691175"><a name="zh-cn_topic_0051408626_p583203691175"></a><a name="zh-cn_topic_0051408626_p583203691175"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row551212811175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p356388081175"><a name="zh-cn_topic_0051408626_p356388081175"></a><a name="zh-cn_topic_0051408626_p356388081175"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p10622981175"><a name="zh-cn_topic_0051408626_p10622981175"></a><a name="zh-cn_topic_0051408626_p10622981175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p575287091175"><a name="zh-cn_topic_0051408626_p575287091175"></a><a name="zh-cn_topic_0051408626_p575287091175"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row479963371175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p624980901175"><a name="zh-cn_topic_0051408626_p624980901175"></a><a name="zh-cn_topic_0051408626_p624980901175"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p291805641175"><a name="zh-cn_topic_0051408626_p291805641175"></a><a name="zh-cn_topic_0051408626_p291805641175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p592057221175"><a name="zh-cn_topic_0051408626_p592057221175"></a><a name="zh-cn_topic_0051408626_p592057221175"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row630894511175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p99718891175"><a name="zh-cn_topic_0051408626_p99718891175"></a><a name="zh-cn_topic_0051408626_p99718891175"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p24167171175"><a name="zh-cn_topic_0051408626_p24167171175"></a><a name="zh-cn_topic_0051408626_p24167171175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p183889601175"><a name="zh-cn_topic_0051408626_p183889601175"></a><a name="zh-cn_topic_0051408626_p183889601175"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row312829201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p508885661175"><a name="zh-cn_topic_0051408626_p508885661175"></a><a name="zh-cn_topic_0051408626_p508885661175"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p283331481175"><a name="zh-cn_topic_0051408626_p283331481175"></a><a name="zh-cn_topic_0051408626_p283331481175"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p22339381175"><a name="zh-cn_topic_0051408626_p22339381175"></a><a name="zh-cn_topic_0051408626_p22339381175"></a>云硬盘快照的元数据信息。</p>
    <p id="p1678772717473"><a name="p1678772717473"></a><a name="p1678772717473"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row201054491175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p179286481175"><a name="zh-cn_topic_0051408626_p179286481175"></a><a name="zh-cn_topic_0051408626_p179286481175"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p429343721175"><a name="zh-cn_topic_0051408626_p429343721175"></a><a name="zh-cn_topic_0051408626_p429343721175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p365124961175"><a name="zh-cn_topic_0051408626_p365124961175"></a><a name="zh-cn_topic_0051408626_p365124961175"></a>快照所属的云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row601770151175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p425000331175"><a name="zh-cn_topic_0051408626_p425000331175"></a><a name="zh-cn_topic_0051408626_p425000331175"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p199506681175"><a name="zh-cn_topic_0051408626_p199506681175"></a><a name="zh-cn_topic_0051408626_p199506681175"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p340521631175"><a name="zh-cn_topic_0051408626_p340521631175"></a><a name="zh-cn_topic_0051408626_p340521631175"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408626_row380340191175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408626_p608567071175"><a name="zh-cn_topic_0051408626_p608567071175"></a><a name="zh-cn_topic_0051408626_p608567071175"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408626_p304462151175"><a name="zh-cn_topic_0051408626_p304462151175"></a><a name="zh-cn_topic_0051408626_p304462151175"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408626_p416400291175"><a name="zh-cn_topic_0051408626_p416400291175"></a><a name="zh-cn_topic_0051408626_p416400291175"></a>快照更新时间。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
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


## 返回值<a name="section4644965111956"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

