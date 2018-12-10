# 查询所有云硬盘详情<a name="ZH-CN_TOPIC_0058762431"></a>

## 功能介绍<a name="section60214390"></a>

查询所有云硬盘详情。

## URI<a name="section5058598"></a>

-   URI格式

    GET /v2/\{project\_id\}/volumes/detail

-   参数说明

    <a name="table58294385"></a>
    <table><thead align="left"><tr id="row24683273"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p53188122"><a name="p53188122"></a><a name="p53188122"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p13270664"><a name="p13270664"></a><a name="p13270664"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p1182010"><a name="p1182010"></a><a name="p1182010"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row28634009"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p37653388"><a name="p37653388"></a><a name="p37653388"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p30025596"><a name="p30025596"></a><a name="p30025596"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p16154192"><a name="p16154192"></a><a name="p16154192"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="table4291376694520"></a>
    <table><thead align="left"><tr id="row75210794520"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="p6092069194520"><a name="p6092069194520"></a><a name="p6092069194520"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="p3562891594520"><a name="p3562891594520"></a><a name="p3562891594520"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="p26101294520"><a name="p26101294520"></a><a name="p26101294520"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="p2114201394520"><a name="p2114201394520"></a><a name="p2114201394520"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3478152794520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p60095082153718"><a name="p60095082153718"></a><a name="p60095082153718"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p35863456153718"><a name="p35863456153718"></a><a name="p35863456153718"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p19258860153718"><a name="p19258860153718"></a><a name="p19258860153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p16463795153718"><a name="p16463795153718"></a><a name="p16463795153718"></a>取值为上一页数据的最后一条记录的id，返回值为该项后面的项。</p>
    </td>
    </tr>
    <tr id="row2183600894520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p56729311153718"><a name="p56729311153718"></a><a name="p56729311153718"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p38113769154021"><a name="p38113769154021"></a><a name="p38113769154021"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p15250867153718"><a name="p15250867153718"></a><a name="p15250867153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p27360714153718"><a name="p27360714153718"></a><a name="p27360714153718"></a>云硬盘名称。<span id="text2734781215241"><a name="text2734781215241"></a><a name="text2734781215241"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row4640654394520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p14628184153718"><a name="p14628184153718"></a><a name="p14628184153718"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p44032231153718"><a name="p44032231153718"></a><a name="p44032231153718"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p9840947153718"><a name="p9840947153718"></a><a name="p9840947153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p58919203153718"><a name="p58919203153718"></a><a name="p58919203153718"></a>返回结果个数限制，取值为大于0的整数。</p>
    <p id="p14657115572511"><a name="p14657115572511"></a><a name="p14657115572511"></a>当租户所有的云硬盘数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="p1233994321914"><a name="p1233994321914"></a><a name="p1233994321914"></a><strong id="b15619135183016"><a name="b15619135183016"></a><a name="b15619135183016"></a>GET /v2/<em id="i86219512306"><a name="i86219512306"></a><a name="i86219512306"></a>xxx</em>/volumes/detail?limit=50</strong>，表示查询第1~50个云硬盘。<strong id="b18611337305"><a name="b18611337305"></a><a name="b18611337305"></a>GET /v2/<em id="i149081817173015"><a name="i149081817173015"></a><a name="i149081817173015"></a>xxx</em>/volumes/detail?offset=50&amp;limit=50</strong>，表示查询第51~100个云硬盘。</p>
    </td>
    </tr>
    <tr id="row6054321594520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p2426142153718"><a name="p2426142153718"></a><a name="p2426142153718"></a>sort_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p43526083154024"><a name="p43526083154024"></a><a name="p43526083154024"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p13119059153718"><a name="p13119059153718"></a><a name="p13119059153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p56010871153718"><a name="p56010871153718"></a><a name="p56010871153718"></a>返回结果按该关键字排序（支持id，status，size，created_at等关键字，默认为“created_at”）。</p>
    </td>
    </tr>
    <tr id="row5521380794520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p29735682153718"><a name="p29735682153718"></a><a name="p29735682153718"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p16700889154026"><a name="p16700889154026"></a><a name="p16700889154026"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p10345862153718"><a name="p10345862153718"></a><a name="p10345862153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p32708487153718"><a name="p32708487153718"></a><a name="p32708487153718"></a>降序或升序(默认为“desc”)。</p>
    </td>
    </tr>
    <tr id="row49871977153626"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p20840349153718"><a name="p20840349153718"></a><a name="p20840349153718"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p10346748153718"><a name="p10346748153718"></a><a name="p10346748153718"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p32780292153718"><a name="p32780292153718"></a><a name="p32780292153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p37957980153718"><a name="p37957980153718"></a><a name="p37957980153718"></a>偏移量（偏移量为一个大于0小于磁盘总个数的整数，表示查询该偏移量后面的所有的卷）。</p>
    </td>
    </tr>
    <tr id="row2837320153624"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p22515601153718"><a name="p22515601153718"></a><a name="p22515601153718"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p53812252154029"><a name="p53812252154029"></a><a name="p53812252154029"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p18251790153718"><a name="p18251790153718"></a><a name="p18251790153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p2000007153718"><a name="p2000007153718"></a><a name="p2000007153718"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row34125704153621"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p48719302153718"><a name="p48719302153718"></a><a name="p48719302153718"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p31082833154032"><a name="p31082833154032"></a><a name="p31082833154032"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p7822125153718"><a name="p7822125153718"></a><a name="p7822125153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p29612385153718"><a name="p29612385153718"></a><a name="p29612385153718"></a>云硬盘元数据。</p>
    </td>
    </tr>
    <tr id="row61070326153619"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p45483948153718"><a name="p45483948153718"></a><a name="p45483948153718"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p23816783154035"><a name="p23816783154035"></a><a name="p23816783154035"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p54179442153718"><a name="p54179442153718"></a><a name="p54179442153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p26458700153718"><a name="p26458700153718"></a><a name="p26458700153718"></a>AZ信息。</p>
    </td>
    </tr>
    <tr id="row2432768294520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p28148606153718"><a name="p28148606153718"></a><a name="p28148606153718"></a>changes-since</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p14402331154037"><a name="p14402331154037"></a><a name="p14402331154037"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p66524343153718"><a name="p66524343153718"></a><a name="p66524343153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p19762672153718"><a name="p19762672153718"></a><a name="p19762672153718"></a>云硬盘更新时间，时间格式示例：2016-01-08T09:41:18。该参数仅在管理员操作中有效。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section45527389"></a>

无

## 响应<a name="section7093323"></a>

-   响应参数

    <a name="table34701445142557"></a>
    <table><thead align="left"><tr id="row12524911142557"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p7884856142557"><a name="p7884856142557"></a><a name="p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p34693598142557"><a name="p34693598142557"></a><a name="p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p58539486142557"><a name="p58539486142557"></a><a name="p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1454458922727"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p4339080622729"><a name="p4339080622729"></a><a name="p4339080622729"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p2499435922729"><a name="p2499435922729"></a><a name="p2499435922729"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p4103742722729"><a name="p4103742722729"></a><a name="p4103742722729"></a>查询请求返回的云硬盘列表。</p>
    </td>
    </tr>
    <tr id="row444782011610"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p54175786153922"><a name="p54175786153922"></a><a name="p54175786153922"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p26162565153922"><a name="p26162565153922"></a><a name="p26162565153922"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p55227932153922"><a name="p55227932153922"></a><a name="p55227932153922"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row44077962142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p62953588153922"><a name="p62953588153922"></a><a name="p62953588153922"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p494261191750"><a name="p494261191750"></a><a name="p494261191750"></a>list&lt;map&lt;string,string&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p379966153922"><a name="p379966153922"></a><a name="p379966153922"></a>云硬盘URI自描述信息。</p>
    </td>
    </tr>
    <tr id="row16186817142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p8559918153922"><a name="p8559918153922"></a><a name="p8559918153922"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p38279089154138"><a name="p38279089154138"></a><a name="p38279089154138"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p50401086153922"><a name="p50401086153922"></a><a name="p50401086153922"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="row45785905142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p33843531153922"><a name="p33843531153922"></a><a name="p33843531153922"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p15510513154140"><a name="p15510513154140"></a><a name="p15510513154140"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p60776191153922"><a name="p60776191153922"></a><a name="p60776191153922"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row35247553142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p13993091153922"><a name="p13993091153922"></a><a name="p13993091153922"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p59698591153922"><a name="p59698591153922"></a><a name="p59698591153922"></a>array</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p35128232153922"><a name="p35128232153922"></a><a name="p35128232153922"></a>挂载信息。</p>
    </td>
    </tr>
    <tr id="row27126244142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p40004503153922"><a name="p40004503153922"></a><a name="p40004503153922"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p51760296154143"><a name="p51760296154143"></a><a name="p51760296154143"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p12372460153922"><a name="p12372460153922"></a><a name="p12372460153922"></a>云硬盘所属的AZ信息。</p>
    </td>
    </tr>
    <tr id="row7009490142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p26935952153922"><a name="p26935952153922"></a><a name="p26935952153922"></a>os-vol-host-attr:host</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p61285780154145"><a name="p61285780154145"></a><a name="p61285780154145"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p12079427153922"><a name="p12079427153922"></a><a name="p12079427153922"></a>云硬盘所在的主机。</p>
    </td>
    </tr>
    <tr id="row49237196142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p14641407153922"><a name="p14641407153922"></a><a name="p14641407153922"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p15993974154147"><a name="p15993974154147"></a><a name="p15993974154147"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p40148014153922"><a name="p40148014153922"></a><a name="p40148014153922"></a>源云硬盘ID，如果是从源云硬盘创建，则有值。</p>
    </td>
    </tr>
    <tr id="row39017307142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p8437822153922"><a name="p8437822153922"></a><a name="p8437822153922"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p43970411154151"><a name="p43970411154151"></a><a name="p43970411154151"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p57569910153922"><a name="p57569910153922"></a><a name="p57569910153922"></a>快照ID，如果是从快照创建，则有值。</p>
    </td>
    </tr>
    <tr id="row20107664142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p25424812153922"><a name="p25424812153922"></a><a name="p25424812153922"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p16247974154153"><a name="p16247974154153"></a><a name="p16247974154153"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p22193516153922"><a name="p22193516153922"></a><a name="p22193516153922"></a>描述。</p>
    </td>
    </tr>
    <tr id="row12897861142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p5837556153922"><a name="p5837556153922"></a><a name="p5837556153922"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p30798966154156"><a name="p30798966154156"></a><a name="p30798966154156"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p8308266153922"><a name="p8308266153922"></a><a name="p8308266153922"></a>云硬盘创建时间。</p>
    </td>
    </tr>
    <tr id="row45680217142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p16928326153922"><a name="p16928326153922"></a><a name="p16928326153922"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p35495495154158"><a name="p35495495154158"></a><a name="p35495495154158"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p60775887153922"><a name="p60775887153922"></a><a name="p60775887153922"></a>云硬盘类型。</p>
    </td>
    </tr>
    <tr id="row47480567142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p13771931153922"><a name="p13771931153922"></a><a name="p13771931153922"></a>os-vol-tenant-attr:tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p4873995415420"><a name="p4873995415420"></a><a name="p4873995415420"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p9058246153922"><a name="p9058246153922"></a><a name="p9058246153922"></a>云硬盘所属的租户ID。</p>
    </td>
    </tr>
    <tr id="row31517135142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p26792948153922"><a name="p26792948153922"></a><a name="p26792948153922"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p22745155153922"><a name="p22745155153922"></a><a name="p22745155153922"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p47959551153922"><a name="p47959551153922"></a><a name="p47959551153922"></a>云硬盘大小。</p>
    </td>
    </tr>
    <tr id="row15610713142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p65903514153922"><a name="p65903514153922"></a><a name="p65903514153922"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p36584404153922"><a name="p36584404153922"></a><a name="p36584404153922"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p63055822144653"><a name="p63055822144653"></a><a name="p63055822144653"></a>云硬盘的元数据。</p>
    <p id="p1210013914474"><a name="p1210013914474"></a><a name="p1210013914474"></a>如果元数据中不包含hw:passthrough字段，云硬盘默认为VBD类型。</p>
    <p id="p3812802015506"><a name="p3812802015506"></a><a name="p3812802015506"></a>如果元数据中不包含__system__encrypted字段，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="row5657368142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p5824606153922"><a name="p5824606153922"></a><a name="p5824606153922"></a>os-vol-mig-status-attr:migstat</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p28057958154213"><a name="p28057958154213"></a><a name="p28057958154213"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p38401827153922"><a name="p38401827153922"></a><a name="p38401827153922"></a>云硬盘迁移状态。</p>
    </td>
    </tr>
    <tr id="row42462677142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p10535641153922"><a name="p10535641153922"></a><a name="p10535641153922"></a>os-vol-mig-status-attr:name_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p41814751154216"><a name="p41814751154216"></a><a name="p41814751154216"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p45371608153922"><a name="p45371608153922"></a><a name="p45371608153922"></a>云硬盘迁移名称ID。</p>
    </td>
    </tr>
    <tr id="row35655683142957"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p42283458153922"><a name="p42283458153922"></a><a name="p42283458153922"></a>os-volume-replication:extended_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p9813320154224"><a name="p9813320154224"></a><a name="p9813320154224"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p28603805153922"><a name="p28603805153922"></a><a name="p28603805153922"></a>云硬盘复制扩展状态。</p>
    </td>
    </tr>
    <tr id="row319029143856"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p48426632153922"><a name="p48426632153922"></a><a name="p48426632153922"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p30243153153922"><a name="p30243153153922"></a><a name="p30243153153922"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p51528552153922"><a name="p51528552153922"></a><a name="p51528552153922"></a>是否为加密云硬盘。</p>
    </td>
    </tr>
    <tr id="row6226231314391"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p50459706153922"><a name="p50459706153922"></a><a name="p50459706153922"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p43392623154228"><a name="p43392623154228"></a><a name="p43392623154228"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p57639660153922"><a name="p57639660153922"></a><a name="p57639660153922"></a>云硬盘备份状态。</p>
    </td>
    </tr>
    <tr id="row1430942214399"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p9163288153922"><a name="p9163288153922"></a><a name="p9163288153922"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p28184221154230"><a name="p28184221154230"></a><a name="p28184221154230"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p59763545153922"><a name="p59763545153922"></a><a name="p59763545153922"></a>使用云硬盘的用户ID。</p>
    </td>
    </tr>
    <tr id="row1801485814395"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p13972139153922"><a name="p13972139153922"></a><a name="p13972139153922"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p60028304154232"><a name="p60028304154232"></a><a name="p60028304154232"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p40663722153922"><a name="p40663722153922"></a><a name="p40663722153922"></a>云硬盘所属一致性组ID。</p>
    </td>
    </tr>
    <tr id="row53974058144326"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p48844805153922"><a name="p48844805153922"></a><a name="p48844805153922"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p26156143154240"><a name="p26156143154240"></a><a name="p26156143154240"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p20882911153922"><a name="p20882911153922"></a><a name="p20882911153922"></a>是否为可启动云硬盘。</p>
    </td>
    </tr>
    <tr id="row46340323144336"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p57039357153922"><a name="p57039357153922"></a><a name="p57039357153922"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p51292786154244"><a name="p51292786154244"></a><a name="p51292786154244"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p46488385153922"><a name="p46488385153922"></a><a name="p46488385153922"></a>云硬盘更新时间。</p>
    </td>
    </tr>
    <tr id="row36758187144417"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p56950153922"><a name="p56950153922"></a><a name="p56950153922"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p4612960153922"><a name="p4612960153922"></a><a name="p4612960153922"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p66643618153922"><a name="p66643618153922"></a><a name="p66643618153922"></a>是否为可共享云硬盘。</p>
    <div class="note" id="note3800959821323"><a name="note3800959821323"></a><a name="note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p45212589213213"><a name="p45212589213213"></a><a name="p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row4658776614505"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p63488919153922"><a name="p63488919153922"></a><a name="p63488919153922"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p42328837153922"><a name="p42328837153922"></a><a name="p42328837153922"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p23021465153922"><a name="p23021465153922"></a><a name="p23021465153922"></a>是否为可共享云硬盘。</p>
    </td>
    </tr>
    <tr id="row29234512142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p5432339153922"><a name="p5432339153922"></a><a name="p5432339153922"></a>volume_image_metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p37366318153922"><a name="p37366318153922"></a><a name="p37366318153922"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p11733449153922"><a name="p11733449153922"></a><a name="p11733449153922"></a>如果云硬盘是从镜像创建的则会有该字段，否则该字段为空。</p>
    <div class="note" id="note13108526174911"><a name="note13108526174911"></a><a name="note13108526174911"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0020235147_p1888154732118"><a name="zh-cn_topic_0020235147_p1888154732118"></a><a name="zh-cn_topic_0020235147_p1888154732118"></a>关于“volume_image_metadata”字段的详细说明，具体请参见“镜像服务API参考”中的“查询镜像详情（OpenStack原生）”章节。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row7814730142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p30858594153922"><a name="p30858594153922"></a><a name="p30858594153922"></a>volumes_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p16518180153922"><a name="p16518180153922"></a><a name="p16518180153922"></a>array</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p62074649153922"><a name="p62074649153922"></a><a name="p62074649153922"></a>云硬盘列表查询位置标记，与响应body中的volumes同级。如果本次查询只返回部分列表信息时，会返回查询到的当前磁盘mark标记的url，可以继续使用这个url查询剩余列表信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   links参数说明

    <a name="zh-cn_topic_0058762429_table24355024185927"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762429_row16225418185927"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762429_p39190461185927"><a name="zh-cn_topic_0058762429_p39190461185927"></a><a name="zh-cn_topic_0058762429_p39190461185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762429_p20310744185927"><a name="zh-cn_topic_0058762429_p20310744185927"></a><a name="zh-cn_topic_0058762429_p20310744185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762429_p47699944185927"><a name="zh-cn_topic_0058762429_p47699944185927"></a><a name="zh-cn_topic_0058762429_p47699944185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762429_row38490285185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p30705403185927"><a name="zh-cn_topic_0058762429_p30705403185927"></a><a name="zh-cn_topic_0058762429_p30705403185927"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p4109689185927"><a name="zh-cn_topic_0058762429_p4109689185927"></a><a name="zh-cn_topic_0058762429_p4109689185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p53015590185927"><a name="zh-cn_topic_0058762429_p53015590185927"></a><a name="zh-cn_topic_0058762429_p53015590185927"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row7378265185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p60768596185927"><a name="zh-cn_topic_0058762429_p60768596185927"></a><a name="zh-cn_topic_0058762429_p60768596185927"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p23309219185927"><a name="zh-cn_topic_0058762429_p23309219185927"></a><a name="zh-cn_topic_0058762429_p23309219185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p57795935185927"><a name="zh-cn_topic_0058762429_p57795935185927"></a><a name="zh-cn_topic_0058762429_p57795935185927"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   attachments参数说明

    <a name="zh-cn_topic_0058762429_table6503386185927"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762429_row1296819185927"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762429_p37933504185927"><a name="zh-cn_topic_0058762429_p37933504185927"></a><a name="zh-cn_topic_0058762429_p37933504185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762429_p52714965185927"><a name="zh-cn_topic_0058762429_p52714965185927"></a><a name="zh-cn_topic_0058762429_p52714965185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762429_p50913593185927"><a name="zh-cn_topic_0058762429_p50913593185927"></a><a name="zh-cn_topic_0058762429_p50913593185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762429_row30360408185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p43274016185927"><a name="zh-cn_topic_0058762429_p43274016185927"></a><a name="zh-cn_topic_0058762429_p43274016185927"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p15534392185927"><a name="zh-cn_topic_0058762429_p15534392185927"></a><a name="zh-cn_topic_0058762429_p15534392185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p49891705185927"><a name="zh-cn_topic_0058762429_p49891705185927"></a><a name="zh-cn_topic_0058762429_p49891705185927"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row49550172185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p54141023185927"><a name="zh-cn_topic_0058762429_p54141023185927"></a><a name="zh-cn_topic_0058762429_p54141023185927"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p23346722185927"><a name="zh-cn_topic_0058762429_p23346722185927"></a><a name="zh-cn_topic_0058762429_p23346722185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p35416329185927"><a name="zh-cn_topic_0058762429_p35416329185927"></a><a name="zh-cn_topic_0058762429_p35416329185927"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row35650386185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p2000176185927"><a name="zh-cn_topic_0058762429_p2000176185927"></a><a name="zh-cn_topic_0058762429_p2000176185927"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p27796542185927"><a name="zh-cn_topic_0058762429_p27796542185927"></a><a name="zh-cn_topic_0058762429_p27796542185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p38329099185927"><a name="zh-cn_topic_0058762429_p38329099185927"></a><a name="zh-cn_topic_0058762429_p38329099185927"></a>挂载的时间信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row9417574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p24626033185927"><a name="zh-cn_topic_0058762429_p24626033185927"></a><a name="zh-cn_topic_0058762429_p24626033185927"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p48551632185927"><a name="zh-cn_topic_0058762429_p48551632185927"></a><a name="zh-cn_topic_0058762429_p48551632185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p48591276185927"><a name="zh-cn_topic_0058762429_p48591276185927"></a><a name="zh-cn_topic_0058762429_p48591276185927"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row34668301185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p56668991185927"><a name="zh-cn_topic_0058762429_p56668991185927"></a><a name="zh-cn_topic_0058762429_p56668991185927"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p26785545185927"><a name="zh-cn_topic_0058762429_p26785545185927"></a><a name="zh-cn_topic_0058762429_p26785545185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p48959624185927"><a name="zh-cn_topic_0058762429_p48959624185927"></a><a name="zh-cn_topic_0058762429_p48959624185927"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row41070280185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p38358373185927"><a name="zh-cn_topic_0058762429_p38358373185927"></a><a name="zh-cn_topic_0058762429_p38358373185927"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p20020490185927"><a name="zh-cn_topic_0058762429_p20020490185927"></a><a name="zh-cn_topic_0058762429_p20020490185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p22392462185927"><a name="zh-cn_topic_0058762429_p22392462185927"></a><a name="zh-cn_topic_0058762429_p22392462185927"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row205574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p16651565185927"><a name="zh-cn_topic_0058762429_p16651565185927"></a><a name="zh-cn_topic_0058762429_p16651565185927"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p6599487185927"><a name="zh-cn_topic_0058762429_p6599487185927"></a><a name="zh-cn_topic_0058762429_p6599487185927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p14021450185927"><a name="zh-cn_topic_0058762429_p14021450185927"></a><a name="zh-cn_topic_0058762429_p14021450185927"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   metadata参数说明

    <a name="zh-cn_topic_0102756196_table3430728295554"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0102756196_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0102756196_p8809200174410"><a name="zh-cn_topic_0102756196_p8809200174410"></a><a name="zh-cn_topic_0102756196_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0102756196_p168135017449"><a name="zh-cn_topic_0102756196_p168135017449"></a><a name="zh-cn_topic_0102756196_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0102756196_p1282213034412"><a name="zh-cn_topic_0102756196_p1282213034412"></a><a name="zh-cn_topic_0102756196_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0102756196_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p1562408795622"><a name="zh-cn_topic_0102756196_p1562408795622"></a><a name="zh-cn_topic_0102756196_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p5759155095622"><a name="zh-cn_topic_0102756196_p5759155095622"></a><a name="zh-cn_topic_0102756196_p5759155095622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p177192813501"><a name="zh-cn_topic_0102756196_p177192813501"></a><a name="zh-cn_topic_0102756196_p177192813501"></a>metadata中的表示加密功能的字段。<a name="zh-cn_topic_0102756196_ul141951225145011"></a><a name="zh-cn_topic_0102756196_ul141951225145011"></a><ul id="zh-cn_topic_0102756196_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p241272995622"><a name="zh-cn_topic_0102756196_p241272995622"></a><a name="zh-cn_topic_0102756196_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p6121338895622"><a name="zh-cn_topic_0102756196_p6121338895622"></a><a name="zh-cn_topic_0102756196_p6121338895622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0102756196_p4159804295622"><a name="zh-cn_topic_0102756196_p4159804295622"></a><a name="zh-cn_topic_0102756196_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p1478896104915"><a name="zh-cn_topic_0102756196_p1478896104915"></a><a name="zh-cn_topic_0102756196_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p52681767104915"><a name="zh-cn_topic_0102756196_p52681767104915"></a><a name="zh-cn_topic_0102756196_p52681767104915"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p17177177145116"><a name="zh-cn_topic_0102756196_p17177177145116"></a><a name="zh-cn_topic_0102756196_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="zh-cn_topic_0102756196_ul14462208141855"></a><a name="zh-cn_topic_0102756196_ul14462208141855"></a><ul id="zh-cn_topic_0102756196_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p3500156018292"><a name="zh-cn_topic_0102756196_p3500156018292"></a><a name="zh-cn_topic_0102756196_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p1655411118292"><a name="zh-cn_topic_0102756196_p1655411118292"></a><a name="zh-cn_topic_0102756196_p1655411118292"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0102756196_p47931946183150"><a name="zh-cn_topic_0102756196_p47931946183150"></a><a name="zh-cn_topic_0102756196_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row16478023164611"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p15479323204615"><a name="zh-cn_topic_0102756196_p15479323204615"></a><a name="zh-cn_topic_0102756196_p15479323204615"></a>readonly</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p134792232467"><a name="zh-cn_topic_0102756196_p134792232467"></a><a name="zh-cn_topic_0102756196_p134792232467"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p3479112318462"><a name="zh-cn_topic_0102756196_p3479112318462"></a><a name="zh-cn_topic_0102756196_p3479112318462"></a>是否为只读模式云硬盘。<a name="zh-cn_topic_0102756196_ul11587123175320"></a><a name="zh-cn_topic_0102756196_ul11587123175320"></a><ul id="zh-cn_topic_0102756196_ul11587123175320"><li>True表示云硬盘仅支持可读模式。</li><li>False表示云硬盘支持读写模式。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row347911235465"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p18479142364612"><a name="zh-cn_topic_0102756196_p18479142364612"></a><a name="zh-cn_topic_0102756196_p18479142364612"></a>attached_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p1547917231465"><a name="zh-cn_topic_0102756196_p1547917231465"></a><a name="zh-cn_topic_0102756196_p1547917231465"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p11479102334617"><a name="zh-cn_topic_0102756196_p11479102334617"></a><a name="zh-cn_topic_0102756196_p11479102334617"></a>只有当云硬盘已挂载至云服务器时，才有该字段，表示云硬盘的使用模式。<a name="zh-cn_topic_0102756196_ul17760125635418"></a><a name="zh-cn_topic_0102756196_ul17760125635418"></a><ul id="zh-cn_topic_0102756196_ul17760125635418"><li>ro表示只读模式。</li><li>rw表示读写模式。</li></ul>
    </div>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "volumes": [
            {
                "attachments": [ ], 
                "availability_zone": "xxx", 
                "bootable": "false", 
                "consistencygroup_id": null, 
                "created_at": "2016-05-25T02:42:10.856332", 
                "description": null, 
                "encrypted": false, 
                "id": "b104b8db-170d-441b-897a-3c8ba9c5a214", 
                "links": [
                    {
                        "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://volume.localdomain.com:8776/dd14c6ac581f40059e27f5320b60bf2f/volumes/b104b8db-170d-441b-897a-3c8ba9c5a214", 
                        "rel": "bookmark"
                    }
                ], 
                "metadata": {
                    "__openstack_region_name": "pod01.xxx", 
                    "a": "b", 
                    "quantityGB": "1", 
                    "volInfoUrl": "fusionstorage://172.30.64.10/0/FEFEEB07D3924CDEA93C612D4E16882D"
                }, 
                "name": "zjb_u25_test", 
                "os-vol-host-attr:host": "pod01.xxx#SATA", 
                "volume_image_metadata": { }, 
                "os-vol-mig-status-attr:migstat": null, 
                "os-vol-mig-status-attr:name_id": null, 
                "os-vol-tenant-attr:tenant_id": "dd14c6ac581f40059e27f5320b60bf2f",  
                "os-volume-replication:extended_status": null, 
                "replication_status": "disabled", 
                "multiattach": false, 
                "size": 1, 
                "snapshot_id": null, 
                "source_volid": null, 
                "status": "available", 
                "updated_at": "2016-05-25T02:42:22.341984", 
                "user_id": "b0524e8342084ef5b74f158f78fc3049", 
                "volume_type": "SATA"
            }
        ], 
        "volumes_links": [
            {
                "href": "https://volume.localdomain.com:8776/v2/dd14c6ac581f40059e27f5320b60bf2f/volumes/detail?limit=1&marker=b104b8db-170d-441b-897a-3c8ba9c5a214", 
                "rel": "next"
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

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错为：

    ```
    {
        "itemNotFound": {
            "message": "XXXX", 
            "code": "XXX"
        }
    } 
    ```


## 返回值<a name="section63839913"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

