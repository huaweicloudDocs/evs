# 查询云硬盘快照列表<a name="evs_04_2096"></a>

## 功能介绍<a name="section5262172611544"></a>

查询云硬盘快照列表。

## URI<a name="section1511931811555"></a>

-   URI格式

    GET /v2/\{project\_id\}/snapshots

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

    <a name="table633033061168"></a>
    <table><thead align="left"><tr id="row57109071168"><th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.1.5.1.1"><p id="p599303181168"><a name="p599303181168"></a><a name="p599303181168"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.623762376237625%" id="mcps1.1.5.1.2"><p id="p225175981168"><a name="p225175981168"></a><a name="p225175981168"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.029702970297027%" id="mcps1.1.5.1.3"><p id="p119861301168"><a name="p119861301168"></a><a name="p119861301168"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="p313524671168"><a name="p313524671168"></a><a name="p313524671168"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12128142617596"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762430_p49168107152914"><a name="zh-cn_topic_0058762430_p49168107152914"></a><a name="zh-cn_topic_0058762430_p49168107152914"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762430_p23193765152914"><a name="zh-cn_topic_0058762430_p23193765152914"></a><a name="zh-cn_topic_0058762430_p23193765152914"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762430_p66755704152914"><a name="zh-cn_topic_0058762430_p66755704152914"></a><a name="zh-cn_topic_0058762430_p66755704152914"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762430_p38502923152914"><a name="zh-cn_topic_0058762430_p38502923152914"></a><a name="zh-cn_topic_0058762430_p38502923152914"></a><span id="text127381323152311"><a name="text127381323152311"></a><a name="text127381323152311"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="row137367471168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p389347291168"><a name="p389347291168"></a><a name="p389347291168"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="p667053841168"><a name="p667053841168"></a><a name="p667053841168"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="p344270561168"><a name="p344270561168"></a><a name="p344270561168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p371281361168"><a name="p371281361168"></a><a name="p371281361168"></a>偏移量。</p>
    <div class="note" id="note6490498915441"><a name="note6490498915441"></a><a name="note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p4727398915441"><a name="p4727398915441"></a><a name="p4727398915441"></a>分页查询快照时使用，与limit配合使用。假如共有30个快照，设置offset为11，limit为10，即为从第12个快照开始查询，一次最多可读取10个快照。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row657177691168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p215391011168"><a name="p215391011168"></a><a name="p215391011168"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="p669456211168"><a name="p669456211168"></a><a name="p669456211168"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="p538862341168"><a name="p538862341168"></a><a name="p538862341168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p27088191168"><a name="p27088191168"></a><a name="p27088191168"></a>返回结果个数限制。</p>
    <p id="p116811542151"><a name="p116811542151"></a><a name="p116811542151"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="p14657115572511"><a name="p14657115572511"></a><a name="p14657115572511"></a>当租户所有的快照数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="p1233994321914"><a name="p1233994321914"></a><a name="p1233994321914"></a><strong id="b15619135183016"><a name="b15619135183016"></a><a name="b15619135183016"></a>GET /v2/<em id="i86219512306"><a name="i86219512306"></a><a name="i86219512306"></a>xxx</em>/snapshots?limit=50</strong>，表示查询第1~50个快照。<strong id="b18611337305"><a name="b18611337305"></a><a name="b18611337305"></a>GET /v2/<em id="i149081817173015"><a name="i149081817173015"></a><a name="i149081817173015"></a>xxx</em>/snapshots?offset=50&amp;limit=50</strong>，表示查询第51~100个快照。</p>
    </td>
    </tr>
    <tr id="row243793751168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p285723381168"><a name="p285723381168"></a><a name="p285723381168"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="p326580131168"><a name="p326580131168"></a><a name="p326580131168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="p280534011168"><a name="p280534011168"></a><a name="p280534011168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p577330051168"><a name="p577330051168"></a><a name="p577330051168"></a>云硬盘快照名称，不支持模糊匹配。<span id="text36369718152549"><a name="text36369718152549"></a><a name="text36369718152549"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row498350041168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p101035441168"><a name="p101035441168"></a><a name="p101035441168"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="p130807691168"><a name="p130807691168"></a><a name="p130807691168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="p529093741168"><a name="p529093741168"></a><a name="p529093741168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p578009201168"><a name="p578009201168"></a><a name="p578009201168"></a>云硬盘快照状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row504462351168"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.1.5.1.1 "><p id="p596132261168"><a name="p596132261168"></a><a name="p596132261168"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.623762376237625%" headers="mcps1.1.5.1.2 "><p id="p639420261168"><a name="p639420261168"></a><a name="p639420261168"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.029702970297027%" headers="mcps1.1.5.1.3 "><p id="p119216351168"><a name="p119216351168"></a><a name="p119216351168"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p261283481168"><a name="p261283481168"></a><a name="p261283481168"></a>云硬盘快照对应的卷ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询状态为available的云硬盘快照为例。

-   请求样例

    ```
    GET https://{endpoint}/v2/{project_id}/snapshots?status=available
    ```


## 响应消息<a name="section539031881175"></a>

-   响应参数

    <a name="table139122611716"></a>
    <table><thead align="left"><tr id="row139212261178"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p592132601710"><a name="p592132601710"></a><a name="p592132601710"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p492026161714"><a name="p492026161714"></a><a name="p492026161714"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p9928266175"><a name="p9928266175"></a><a name="p9928266175"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2925156111719"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p623850141175"><a name="p623850141175"></a><a name="p623850141175"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p200213431175"><a name="p200213431175"></a><a name="p200213431175"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p279846901175"><a name="p279846901175"></a><a name="p279846901175"></a>快照信息，请参见<a href="#li367387041175">•snapshots参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row892172614170"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p59292621716"><a name="p59292621716"></a><a name="p59292621716"></a>snapshots_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p9921026101717"><a name="p9921026101717"></a><a name="p9921026101717"></a>list&lt;map&lt;String,String&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p693112661716"><a name="p693112661716"></a><a name="p693112661716"></a>云硬盘快照列表查询位置标记。当查询时指定limit时会返回该字段，返回该字段表示本次查询只查出了部分云硬盘快照信息。</p>
    </td>
    </tr>
    <tr id="row7894718155410"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li367387041175"></a>snapshots参数说明

    <a name="table622128841175"></a>
    <table><thead align="left"><tr id="row535860991175"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p455067371175"><a name="p455067371175"></a><a name="p455067371175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p621670471175"><a name="p621670471175"></a><a name="p621670471175"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p574320291175"><a name="p574320291175"></a><a name="p574320291175"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row505356201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p668534581175"><a name="p668534581175"></a><a name="p668534581175"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p464210281175"><a name="p464210281175"></a><a name="p464210281175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p283450141175"><a name="p283450141175"></a><a name="p283450141175"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row537785391175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p610943921175"><a name="p610943921175"></a><a name="p610943921175"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p496987011175"><a name="p496987011175"></a><a name="p496987011175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p583203691175"><a name="p583203691175"></a><a name="p583203691175"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row551212811175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p356388081175"><a name="p356388081175"></a><a name="p356388081175"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p10622981175"><a name="p10622981175"></a><a name="p10622981175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p575287091175"><a name="p575287091175"></a><a name="p575287091175"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row479963371175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p624980901175"><a name="p624980901175"></a><a name="p624980901175"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p291805641175"><a name="p291805641175"></a><a name="p291805641175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p592057221175"><a name="p592057221175"></a><a name="p592057221175"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row630894511175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p99718891175"><a name="p99718891175"></a><a name="p99718891175"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p24167171175"><a name="p24167171175"></a><a name="p24167171175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p183889601175"><a name="p183889601175"></a><a name="p183889601175"></a>云硬盘快照创建时间。</p>
    <p id="p16450449115618"><a name="p16450449115618"></a><a name="p16450449115618"></a><span id="text8188185355614"><a name="text8188185355614"></a><a name="text8188185355614"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row312829201175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p508885661175"><a name="p508885661175"></a><a name="p508885661175"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p283331481175"><a name="p283331481175"></a><a name="p283331481175"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p22339381175"><a name="p22339381175"></a><a name="p22339381175"></a>云硬盘快照的元数据信息。</p>
    <p id="p1678772717473"><a name="p1678772717473"></a><a name="p1678772717473"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="row201054491175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p179286481175"><a name="p179286481175"></a><a name="p179286481175"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p429343721175"><a name="p429343721175"></a><a name="p429343721175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p365124961175"><a name="p365124961175"></a><a name="p365124961175"></a>快照所属的云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row601770151175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p425000331175"><a name="p425000331175"></a><a name="p425000331175"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p199506681175"><a name="p199506681175"></a><a name="p199506681175"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p340521631175"><a name="p340521631175"></a><a name="p340521631175"></a>云硬盘快照大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="row380340191175"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p608567071175"><a name="p608567071175"></a><a name="p608567071175"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p304462151175"><a name="p304462151175"></a><a name="p304462151175"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p416400291175"><a name="p416400291175"></a><a name="p416400291175"></a>快照更新时间。</p>
    <p id="p835995905612"><a name="p835995905612"></a><a name="p835995905612"></a><span id="text7360459195618"><a name="text7360459195618"></a><a name="text7360459195618"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
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

请参考[错误码说明](错误码说明.md)。

