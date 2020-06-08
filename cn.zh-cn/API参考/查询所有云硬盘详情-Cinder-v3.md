# 查询所有云硬盘详情<a name="evs_04_3033"></a>

## 功能介绍<a name="section60214390"></a>

查询所有云硬盘详情。

## URI<a name="section5058598"></a>

-   URI格式

    GET /v3/\{project\_id\}/volumes/detail

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
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="zh-cn_topic_0058762431_table4291376694520"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762431_row75210794520"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058762431_p6092069194520"><a name="zh-cn_topic_0058762431_p6092069194520"></a><a name="zh-cn_topic_0058762431_p6092069194520"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058762431_p3562891594520"><a name="zh-cn_topic_0058762431_p3562891594520"></a><a name="zh-cn_topic_0058762431_p3562891594520"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058762431_p26101294520"><a name="zh-cn_topic_0058762431_p26101294520"></a><a name="zh-cn_topic_0058762431_p26101294520"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058762431_p2114201394520"><a name="zh-cn_topic_0058762431_p2114201394520"></a><a name="zh-cn_topic_0058762431_p2114201394520"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762431_row3478152794520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p60095082153718"><a name="zh-cn_topic_0058762431_p60095082153718"></a><a name="zh-cn_topic_0058762431_p60095082153718"></a>marker</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p35863456153718"><a name="zh-cn_topic_0058762431_p35863456153718"></a><a name="zh-cn_topic_0058762431_p35863456153718"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p19258860153718"><a name="zh-cn_topic_0058762431_p19258860153718"></a><a name="zh-cn_topic_0058762431_p19258860153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p16463795153718"><a name="zh-cn_topic_0058762431_p16463795153718"></a><a name="zh-cn_topic_0058762431_p16463795153718"></a><span id="text97115183392"><a name="text97115183392"></a><a name="text97115183392"></a>分页查询的起始资源id，取值为上一页最后一条查询记录的资源id。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row2183600894520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p56729311153718"><a name="zh-cn_topic_0058762431_p56729311153718"></a><a name="zh-cn_topic_0058762431_p56729311153718"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p38113769154021"><a name="zh-cn_topic_0058762431_p38113769154021"></a><a name="zh-cn_topic_0058762431_p38113769154021"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p15250867153718"><a name="zh-cn_topic_0058762431_p15250867153718"></a><a name="zh-cn_topic_0058762431_p15250867153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p27360714153718"><a name="zh-cn_topic_0058762431_p27360714153718"></a><a name="zh-cn_topic_0058762431_p27360714153718"></a>云硬盘名称。<span id="zh-cn_topic_0058762431_text2734781215241"><a name="zh-cn_topic_0058762431_text2734781215241"></a><a name="zh-cn_topic_0058762431_text2734781215241"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row4640654394520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p14628184153718"><a name="zh-cn_topic_0058762431_p14628184153718"></a><a name="zh-cn_topic_0058762431_p14628184153718"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p44032231153718"><a name="zh-cn_topic_0058762431_p44032231153718"></a><a name="zh-cn_topic_0058762431_p44032231153718"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p9840947153718"><a name="zh-cn_topic_0058762431_p9840947153718"></a><a name="zh-cn_topic_0058762431_p9840947153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p58919203153718"><a name="zh-cn_topic_0058762431_p58919203153718"></a><a name="zh-cn_topic_0058762431_p58919203153718"></a>返回结果个数限制。</p>
    <p id="p13400175415125"><a name="p13400175415125"></a><a name="p13400175415125"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    <p id="zh-cn_topic_0058762431_p14657115572511"><a name="zh-cn_topic_0058762431_p14657115572511"></a><a name="zh-cn_topic_0058762431_p14657115572511"></a>当租户所有的云硬盘数量大于50个时，为了提升您的查询效率，建议查询的时候使用limit参数，并且参数值最大设置为50。查询示例：</p>
    <p id="zh-cn_topic_0058762431_p1233994321914"><a name="zh-cn_topic_0058762431_p1233994321914"></a><a name="zh-cn_topic_0058762431_p1233994321914"></a><strong id="zh-cn_topic_0058762431_b15619135183016"><a name="zh-cn_topic_0058762431_b15619135183016"></a><a name="zh-cn_topic_0058762431_b15619135183016"></a>GET /v3/<em id="zh-cn_topic_0058762431_i86219512306"><a name="zh-cn_topic_0058762431_i86219512306"></a><a name="zh-cn_topic_0058762431_i86219512306"></a>xxx</em>/volumes/detail?limit=50</strong>，表示查询第1~50个云硬盘。<strong id="zh-cn_topic_0058762431_b18611337305"><a name="zh-cn_topic_0058762431_b18611337305"></a><a name="zh-cn_topic_0058762431_b18611337305"></a>GET /v3/<em id="zh-cn_topic_0058762431_i149081817173015"><a name="zh-cn_topic_0058762431_i149081817173015"></a><a name="zh-cn_topic_0058762431_i149081817173015"></a>xxx</em>/volumes/detail?offset=50&amp;limit=50</strong>，表示查询第51~100个云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row6054321594520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p2426142153718"><a name="zh-cn_topic_0058762431_p2426142153718"></a><a name="zh-cn_topic_0058762431_p2426142153718"></a>sort_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p43526083154024"><a name="zh-cn_topic_0058762431_p43526083154024"></a><a name="zh-cn_topic_0058762431_p43526083154024"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p13119059153718"><a name="zh-cn_topic_0058762431_p13119059153718"></a><a name="zh-cn_topic_0058762431_p13119059153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p43249593152914"><a name="p43249593152914"></a><a name="p43249593152914"></a>返回结果按该关键字排序，支持id，status，size，created_at等关键字，默认为“created_at”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row5521380794520"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p29735682153718"><a name="zh-cn_topic_0058762431_p29735682153718"></a><a name="zh-cn_topic_0058762431_p29735682153718"></a>sort_dir</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p16700889154026"><a name="zh-cn_topic_0058762431_p16700889154026"></a><a name="zh-cn_topic_0058762431_p16700889154026"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p10345862153718"><a name="zh-cn_topic_0058762431_p10345862153718"></a><a name="zh-cn_topic_0058762431_p10345862153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><div class="p" id="p2025341125211"><a name="p2025341125211"></a><a name="p2025341125211"></a>返回结果按照降序或升序排列，默认为“desc”。<a name="ul107075455529"></a><a name="ul107075455529"></a><ul id="ul107075455529"><li>降序：desc</li><li>升序：asc</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row49871977153626"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p20840349153718"><a name="zh-cn_topic_0058762431_p20840349153718"></a><a name="zh-cn_topic_0058762431_p20840349153718"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p10346748153718"><a name="zh-cn_topic_0058762431_p10346748153718"></a><a name="zh-cn_topic_0058762431_p10346748153718"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p32780292153718"><a name="zh-cn_topic_0058762431_p32780292153718"></a><a name="zh-cn_topic_0058762431_p32780292153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p02247913491"><a name="p02247913491"></a><a name="p02247913491"></a>偏移量</p>
    <p id="zh-cn_topic_0058762430_p27592310152914"><a name="zh-cn_topic_0058762430_p27592310152914"></a><a name="zh-cn_topic_0058762430_p27592310152914"></a>偏移量为一个大于0小于磁盘总个数的整数，表示查询该偏移量后面的所有的云硬盘。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row2837320153624"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p22515601153718"><a name="zh-cn_topic_0058762431_p22515601153718"></a><a name="zh-cn_topic_0058762431_p22515601153718"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p53812252154029"><a name="zh-cn_topic_0058762431_p53812252154029"></a><a name="zh-cn_topic_0058762431_p53812252154029"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p18251790153718"><a name="zh-cn_topic_0058762431_p18251790153718"></a><a name="zh-cn_topic_0058762431_p18251790153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p2000007153718"><a name="zh-cn_topic_0058762431_p2000007153718"></a><a name="zh-cn_topic_0058762431_p2000007153718"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row34125704153621"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p48719302153718"><a name="zh-cn_topic_0058762431_p48719302153718"></a><a name="zh-cn_topic_0058762431_p48719302153718"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p31082833154032"><a name="zh-cn_topic_0058762431_p31082833154032"></a><a name="zh-cn_topic_0058762431_p31082833154032"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p7822125153718"><a name="zh-cn_topic_0058762431_p7822125153718"></a><a name="zh-cn_topic_0058762431_p7822125153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p29612385153718"><a name="zh-cn_topic_0058762431_p29612385153718"></a><a name="zh-cn_topic_0058762431_p29612385153718"></a>云硬盘元数据。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row61070326153619"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762431_p45483948153718"><a name="zh-cn_topic_0058762431_p45483948153718"></a><a name="zh-cn_topic_0058762431_p45483948153718"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762431_p23816783154035"><a name="zh-cn_topic_0058762431_p23816783154035"></a><a name="zh-cn_topic_0058762431_p23816783154035"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762431_p54179442153718"><a name="zh-cn_topic_0058762431_p54179442153718"></a><a name="zh-cn_topic_0058762431_p54179442153718"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762431_p26458700153718"><a name="zh-cn_topic_0058762431_p26458700153718"></a><a name="zh-cn_topic_0058762431_p26458700153718"></a>AZ信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section3266414134213"></a>

以查询状态为available的云硬盘详情为例。

-   请求样例

    ```
    GET https://{endpoint}/v3/{project_id}/volumes/detail?status=available
    ```


## 响应消息<a name="section7093323"></a>

-   响应参数

    <a name="table3231819124520"></a>
    <table><thead align="left"><tr id="row182320192456"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p62321919144515"><a name="p62321919144515"></a><a name="p62321919144515"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.14788521147885%" id="mcps1.1.4.1.2"><p id="p2232219174510"><a name="p2232219174510"></a><a name="p2232219174510"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.67423257674233%" id="mcps1.1.4.1.3"><p id="p132325192454"><a name="p132325192454"></a><a name="p132325192454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row42321819154515"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p823213196454"><a name="p823213196454"></a><a name="p823213196454"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="p13232181974513"><a name="p13232181974513"></a><a name="p13232181974513"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="p5232131916457"><a name="p5232131916457"></a><a name="p5232131916457"></a>查询请求返回的云硬盘列表，请参见<a href="#zh-cn_topic_0058762431_li3451542201439">•volumes参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row1024031914455"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p7240111944517"><a name="p7240111944517"></a><a name="p7240111944517"></a>volumes_links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="p1924013198451"><a name="p1924013198451"></a><a name="p1924013198451"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="p9240101964519"><a name="p9240101964519"></a><a name="p9240101964519"></a>云硬盘列表查询位置标记。如果本次查询只返回部分列表信息时，会返回查询到的当前磁盘mark标记的url，可以继续使用这个url查询剩余列表信息，请参见<a href="#zh-cn_topic_0058762431_li851885019247">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row1825458164715"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058762431_li3451542201439"></a>volumes参数说明

    <a name="zh-cn_topic_0058762431_table34701445142557"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762431_row12524911142557"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762431_p7884856142557"><a name="zh-cn_topic_0058762431_p7884856142557"></a><a name="zh-cn_topic_0058762431_p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.14788521147885%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762431_p34693598142557"><a name="zh-cn_topic_0058762431_p34693598142557"></a><a name="zh-cn_topic_0058762431_p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.67423257674233%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762431_p58539486142557"><a name="zh-cn_topic_0058762431_p58539486142557"></a><a name="zh-cn_topic_0058762431_p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762431_row444782011610"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p54175786153922"><a name="zh-cn_topic_0058762431_p54175786153922"></a><a name="zh-cn_topic_0058762431_p54175786153922"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p26162565153922"><a name="zh-cn_topic_0058762431_p26162565153922"></a><a name="zh-cn_topic_0058762431_p26162565153922"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p55227932153922"><a name="zh-cn_topic_0058762431_p55227932153922"></a><a name="zh-cn_topic_0058762431_p55227932153922"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row44077962142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p62953588153922"><a name="zh-cn_topic_0058762431_p62953588153922"></a><a name="zh-cn_topic_0058762431_p62953588153922"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p494261191750"><a name="zh-cn_topic_0058762431_p494261191750"></a><a name="zh-cn_topic_0058762431_p494261191750"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p379966153922"><a name="zh-cn_topic_0058762431_p379966153922"></a><a name="zh-cn_topic_0058762431_p379966153922"></a>云硬盘URI自描述信息，请参见<a href="#zh-cn_topic_0058762431_li851885019247">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row16186817142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p8559918153922"><a name="zh-cn_topic_0058762431_p8559918153922"></a><a name="zh-cn_topic_0058762431_p8559918153922"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p38279089154138"><a name="zh-cn_topic_0058762431_p38279089154138"></a><a name="zh-cn_topic_0058762431_p38279089154138"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p50401086153922"><a name="zh-cn_topic_0058762431_p50401086153922"></a><a name="zh-cn_topic_0058762431_p50401086153922"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row45785905142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p33843531153922"><a name="zh-cn_topic_0058762431_p33843531153922"></a><a name="zh-cn_topic_0058762431_p33843531153922"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p15510513154140"><a name="zh-cn_topic_0058762431_p15510513154140"></a><a name="zh-cn_topic_0058762431_p15510513154140"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p60776191153922"><a name="zh-cn_topic_0058762431_p60776191153922"></a><a name="zh-cn_topic_0058762431_p60776191153922"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row35247553142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p13993091153922"><a name="zh-cn_topic_0058762431_p13993091153922"></a><a name="zh-cn_topic_0058762431_p13993091153922"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p59698591153922"><a name="zh-cn_topic_0058762431_p59698591153922"></a><a name="zh-cn_topic_0058762431_p59698591153922"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p35128232153922"><a name="zh-cn_topic_0058762431_p35128232153922"></a><a name="zh-cn_topic_0058762431_p35128232153922"></a>挂载信息，请参见<a href="#zh-cn_topic_0058762431_li5001921919316">•attachments参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row27126244142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p40004503153922"><a name="zh-cn_topic_0058762431_p40004503153922"></a><a name="zh-cn_topic_0058762431_p40004503153922"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p51760296154143"><a name="zh-cn_topic_0058762431_p51760296154143"></a><a name="zh-cn_topic_0058762431_p51760296154143"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p12372460153922"><a name="zh-cn_topic_0058762431_p12372460153922"></a><a name="zh-cn_topic_0058762431_p12372460153922"></a>云硬盘所属的AZ信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row7009490142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p26935952153922"><a name="zh-cn_topic_0058762431_p26935952153922"></a><a name="zh-cn_topic_0058762431_p26935952153922"></a>os-vol-host-attr:host</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p61285780154145"><a name="zh-cn_topic_0058762431_p61285780154145"></a><a name="zh-cn_topic_0058762431_p61285780154145"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p12079427153922"><a name="zh-cn_topic_0058762431_p12079427153922"></a><a name="zh-cn_topic_0058762431_p12079427153922"></a><span id="text1720893911585"><a name="text1720893911585"></a><a name="text1720893911585"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row49237196142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p14641407153922"><a name="zh-cn_topic_0058762431_p14641407153922"></a><a name="zh-cn_topic_0058762431_p14641407153922"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p15993974154147"><a name="zh-cn_topic_0058762431_p15993974154147"></a><a name="zh-cn_topic_0058762431_p15993974154147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p40148014153922"><a name="zh-cn_topic_0058762431_p40148014153922"></a><a name="zh-cn_topic_0058762431_p40148014153922"></a>源云硬盘ID，如果是从源云硬盘创建，则有值。</p>
    <p id="p4357134552610"><a name="p4357134552610"></a><a name="p4357134552610"></a><span id="text18357144552617"><a name="text18357144552617"></a><a name="text18357144552617"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row39017307142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p8437822153922"><a name="zh-cn_topic_0058762431_p8437822153922"></a><a name="zh-cn_topic_0058762431_p8437822153922"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p43970411154151"><a name="zh-cn_topic_0058762431_p43970411154151"></a><a name="zh-cn_topic_0058762431_p43970411154151"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p57569910153922"><a name="zh-cn_topic_0058762431_p57569910153922"></a><a name="zh-cn_topic_0058762431_p57569910153922"></a>快照ID，如果是从快照创建，则有值。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row20107664142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p25424812153922"><a name="zh-cn_topic_0058762431_p25424812153922"></a><a name="zh-cn_topic_0058762431_p25424812153922"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p16247974154153"><a name="zh-cn_topic_0058762431_p16247974154153"></a><a name="zh-cn_topic_0058762431_p16247974154153"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p22193516153922"><a name="zh-cn_topic_0058762431_p22193516153922"></a><a name="zh-cn_topic_0058762431_p22193516153922"></a>描述。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row12897861142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p5837556153922"><a name="zh-cn_topic_0058762431_p5837556153922"></a><a name="zh-cn_topic_0058762431_p5837556153922"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p30798966154156"><a name="zh-cn_topic_0058762431_p30798966154156"></a><a name="zh-cn_topic_0058762431_p30798966154156"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p8308266153922"><a name="zh-cn_topic_0058762431_p8308266153922"></a><a name="zh-cn_topic_0058762431_p8308266153922"></a>云硬盘创建时间。</p>
    <p id="p23708433313"><a name="p23708433313"></a><a name="p23708433313"></a><span id="text127118487312"><a name="text127118487312"></a><a name="text127118487312"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row45680217142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p16928326153922"><a name="zh-cn_topic_0058762431_p16928326153922"></a><a name="zh-cn_topic_0058762431_p16928326153922"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p35495495154158"><a name="zh-cn_topic_0058762431_p35495495154158"></a><a name="zh-cn_topic_0058762431_p35495495154158"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p60775887153922"><a name="zh-cn_topic_0058762431_p60775887153922"></a><a name="zh-cn_topic_0058762431_p60775887153922"></a>云硬盘类型。</p>
    <div class="p" id="zh-cn_topic_0044524833_p112762317377"><a name="zh-cn_topic_0044524833_p112762317377"></a><a name="zh-cn_topic_0044524833_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row47480567142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p13771931153922"><a name="zh-cn_topic_0058762431_p13771931153922"></a><a name="zh-cn_topic_0058762431_p13771931153922"></a>os-vol-tenant-attr:tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p4873995415420"><a name="zh-cn_topic_0058762431_p4873995415420"></a><a name="zh-cn_topic_0058762431_p4873995415420"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p9058246153922"><a name="zh-cn_topic_0058762431_p9058246153922"></a><a name="zh-cn_topic_0058762431_p9058246153922"></a>云硬盘所属的租户ID。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row31517135142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p26792948153922"><a name="zh-cn_topic_0058762431_p26792948153922"></a><a name="zh-cn_topic_0058762431_p26792948153922"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p22745155153922"><a name="zh-cn_topic_0058762431_p22745155153922"></a><a name="zh-cn_topic_0058762431_p22745155153922"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p47959551153922"><a name="zh-cn_topic_0058762431_p47959551153922"></a><a name="zh-cn_topic_0058762431_p47959551153922"></a>云硬盘大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row15610713142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p65903514153922"><a name="zh-cn_topic_0058762431_p65903514153922"></a><a name="zh-cn_topic_0058762431_p65903514153922"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p36584404153922"><a name="zh-cn_topic_0058762431_p36584404153922"></a><a name="zh-cn_topic_0058762431_p36584404153922"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p63055822144653"><a name="zh-cn_topic_0058762431_p63055822144653"></a><a name="zh-cn_topic_0058762431_p63055822144653"></a>云硬盘的元数据，请参见<a href="#li29114110314">•metadata参数说明</a>。</p>
    <p id="zh-cn_topic_0058762431_p1210013914474"><a name="zh-cn_topic_0058762431_p1210013914474"></a><a name="zh-cn_topic_0058762431_p1210013914474"></a>如果元数据中不包含hw:passthrough字段，云硬盘默认为VBD类型。</p>
    <p id="zh-cn_topic_0058762431_p3812802015506"><a name="zh-cn_topic_0058762431_p3812802015506"></a><a name="zh-cn_topic_0058762431_p3812802015506"></a>如果元数据中不包含__system__encrypted字段，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row5657368142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p5824606153922"><a name="zh-cn_topic_0058762431_p5824606153922"></a><a name="zh-cn_topic_0058762431_p5824606153922"></a>os-vol-mig-status-attr:migstat</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p28057958154213"><a name="zh-cn_topic_0058762431_p28057958154213"></a><a name="zh-cn_topic_0058762431_p28057958154213"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p38401827153922"><a name="zh-cn_topic_0058762431_p38401827153922"></a><a name="zh-cn_topic_0058762431_p38401827153922"></a><span id="text203605127103"><a name="text203605127103"></a><a name="text203605127103"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row42462677142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p10535641153922"><a name="zh-cn_topic_0058762431_p10535641153922"></a><a name="zh-cn_topic_0058762431_p10535641153922"></a>os-vol-mig-status-attr:name_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p41814751154216"><a name="zh-cn_topic_0058762431_p41814751154216"></a><a name="zh-cn_topic_0058762431_p41814751154216"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p45371608153922"><a name="zh-cn_topic_0058762431_p45371608153922"></a><a name="zh-cn_topic_0058762431_p45371608153922"></a><span id="text268125418222"><a name="text268125418222"></a><a name="text268125418222"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row35655683142957"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p42283458153922"><a name="zh-cn_topic_0058762431_p42283458153922"></a><a name="zh-cn_topic_0058762431_p42283458153922"></a>os-volume-replication:extended_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p9813320154224"><a name="zh-cn_topic_0058762431_p9813320154224"></a><a name="zh-cn_topic_0058762431_p9813320154224"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p28603805153922"><a name="zh-cn_topic_0058762431_p28603805153922"></a><a name="zh-cn_topic_0058762431_p28603805153922"></a><span id="text379518478151"><a name="text379518478151"></a><a name="text379518478151"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row57913155185111"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p47452553185118"><a name="zh-cn_topic_0058762431_p47452553185118"></a><a name="zh-cn_topic_0058762431_p47452553185118"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p18451581185118"><a name="zh-cn_topic_0058762431_p18451581185118"></a><a name="zh-cn_topic_0058762431_p18451581185118"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p27951625185124"><a name="zh-cn_topic_0058762431_p27951625185124"></a><a name="zh-cn_topic_0058762431_p27951625185124"></a><span id="text16290132561216"><a name="text16290132561216"></a><a name="text16290132561216"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row6226231314391"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p50459706153922"><a name="zh-cn_topic_0058762431_p50459706153922"></a><a name="zh-cn_topic_0058762431_p50459706153922"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p43392623154228"><a name="zh-cn_topic_0058762431_p43392623154228"></a><a name="zh-cn_topic_0058762431_p43392623154228"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p57639660153922"><a name="zh-cn_topic_0058762431_p57639660153922"></a><a name="zh-cn_topic_0058762431_p57639660153922"></a><span id="text6498181171119"><a name="text6498181171119"></a><a name="text6498181171119"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row1430942214399"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p9163288153922"><a name="zh-cn_topic_0058762431_p9163288153922"></a><a name="zh-cn_topic_0058762431_p9163288153922"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p28184221154230"><a name="zh-cn_topic_0058762431_p28184221154230"></a><a name="zh-cn_topic_0058762431_p28184221154230"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p59763545153922"><a name="zh-cn_topic_0058762431_p59763545153922"></a><a name="zh-cn_topic_0058762431_p59763545153922"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row1801485814395"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p13972139153922"><a name="zh-cn_topic_0058762431_p13972139153922"></a><a name="zh-cn_topic_0058762431_p13972139153922"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p60028304154232"><a name="zh-cn_topic_0058762431_p60028304154232"></a><a name="zh-cn_topic_0058762431_p60028304154232"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="p17844141412282"><a name="p17844141412282"></a><a name="p17844141412282"></a><span id="text13343838181111"><a name="text13343838181111"></a><a name="text13343838181111"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row53974058144326"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p48844805153922"><a name="zh-cn_topic_0058762431_p48844805153922"></a><a name="zh-cn_topic_0058762431_p48844805153922"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p26156143154240"><a name="zh-cn_topic_0058762431_p26156143154240"></a><a name="zh-cn_topic_0058762431_p26156143154240"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_p8780414125315"><a name="zh-cn_topic_0098680634_p8780414125315"></a><a name="zh-cn_topic_0098680634_p8780414125315"></a>是否为启动云硬盘。<a name="ul185931714111"></a><a name="ul185931714111"></a><ul id="ul185931714111"><li>true：表示为启动云硬盘。</li><li>false：表示为非启动云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row46340323144336"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p57039357153922"><a name="zh-cn_topic_0058762431_p57039357153922"></a><a name="zh-cn_topic_0058762431_p57039357153922"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p51292786154244"><a name="zh-cn_topic_0058762431_p51292786154244"></a><a name="zh-cn_topic_0058762431_p51292786154244"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p46488385153922"><a name="zh-cn_topic_0058762431_p46488385153922"></a><a name="zh-cn_topic_0058762431_p46488385153922"></a>云硬盘更新时间。</p>
    <p id="p121428117412"><a name="p121428117412"></a><a name="p121428117412"></a><span id="text91428118418"><a name="text91428118418"></a><a name="text91428118418"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row36758187144417"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p56950153922"><a name="zh-cn_topic_0058762431_p56950153922"></a><a name="zh-cn_topic_0058762431_p56950153922"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p4612960153922"><a name="zh-cn_topic_0058762431_p4612960153922"></a><a name="zh-cn_topic_0058762431_p4612960153922"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p66643618153922"><a name="zh-cn_topic_0058762431_p66643618153922"></a><a name="zh-cn_topic_0058762431_p66643618153922"></a>是否为可共享云硬盘。</p>
    <div class="note" id="zh-cn_topic_0058762431_note3800959821323"><a name="zh-cn_topic_0058762431_note3800959821323"></a><a name="zh-cn_topic_0058762431_note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0058762431_p45212589213213"><a name="zh-cn_topic_0058762431_p45212589213213"></a><a name="zh-cn_topic_0058762431_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row4658776614505"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p63488919153922"><a name="zh-cn_topic_0058762431_p63488919153922"></a><a name="zh-cn_topic_0058762431_p63488919153922"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p42328837153922"><a name="zh-cn_topic_0058762431_p42328837153922"></a><a name="zh-cn_topic_0058762431_p42328837153922"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_p4781191416535"><a name="zh-cn_topic_0098680634_p4781191416535"></a><a name="zh-cn_topic_0098680634_p4781191416535"></a>是否为共享云硬盘。<a name="ul161621719119"></a><a name="ul161621719119"></a><ul id="ul161621719119"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762431_row29234512142557"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762431_p5432339153922"><a name="zh-cn_topic_0058762431_p5432339153922"></a><a name="zh-cn_topic_0058762431_p5432339153922"></a>volume_image_metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.14788521147885%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762431_p37366318153922"><a name="zh-cn_topic_0058762431_p37366318153922"></a><a name="zh-cn_topic_0058762431_p37366318153922"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.67423257674233%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762431_p11733449153922"><a name="zh-cn_topic_0058762431_p11733449153922"></a><a name="zh-cn_topic_0058762431_p11733449153922"></a>如果云硬盘是从镜像创建的则会有该字段，否则该字段为空。</p>
    <div class="note" id="note14735916164810"><a name="note14735916164810"></a><a name="note14735916164810"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2009_p16054517146"><a name="evs_04_2009_p16054517146"></a><a name="evs_04_2009_p16054517146"></a>关于“volume_image_metadata”字段的详细说明，具体请参见<a href="https://support.huaweicloud.com/api-ims/ims_03_0703.html" target="_blank" rel="noopener noreferrer">查询镜像详情（OpenStack原生）</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058762431_li851885019247"></a>links参数说明

    <a name="evs_04_2069_evs_04_2067_table24355024185927"></a>
    <table><thead align="left"><tr id="evs_04_2069_evs_04_2067_row16225418185927"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2069_evs_04_2067_p39190461185927"><a name="evs_04_2069_evs_04_2067_p39190461185927"></a><a name="evs_04_2069_evs_04_2067_p39190461185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2069_evs_04_2067_p20310744185927"><a name="evs_04_2069_evs_04_2067_p20310744185927"></a><a name="evs_04_2069_evs_04_2067_p20310744185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="evs_04_2069_evs_04_2067_p47699944185927"><a name="evs_04_2069_evs_04_2067_p47699944185927"></a><a name="evs_04_2069_evs_04_2067_p47699944185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2069_evs_04_2067_row38490285185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p30705403185927"><a name="evs_04_2069_evs_04_2067_p30705403185927"></a><a name="evs_04_2069_evs_04_2067_p30705403185927"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p4109689185927"><a name="evs_04_2069_evs_04_2067_p4109689185927"></a><a name="evs_04_2069_evs_04_2067_p4109689185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p53015590185927"><a name="evs_04_2069_evs_04_2067_p53015590185927"></a><a name="evs_04_2069_evs_04_2067_p53015590185927"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row7378265185927"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p60768596185927"><a name="evs_04_2069_evs_04_2067_p60768596185927"></a><a name="evs_04_2069_evs_04_2067_p60768596185927"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p23309219185927"><a name="evs_04_2069_evs_04_2067_p23309219185927"></a><a name="evs_04_2069_evs_04_2067_p23309219185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p57795935185927"><a name="evs_04_2069_evs_04_2067_p57795935185927"></a><a name="evs_04_2069_evs_04_2067_p57795935185927"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0058762431_li5001921919316"></a>attachments参数说明

    <a name="evs_04_2069_evs_04_2067_table6503386185927"></a>
    <table><thead align="left"><tr id="evs_04_2069_evs_04_2067_row1296819185927"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="evs_04_2069_evs_04_2067_p37933504185927"><a name="evs_04_2069_evs_04_2067_p37933504185927"></a><a name="evs_04_2069_evs_04_2067_p37933504185927"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="evs_04_2069_evs_04_2067_p52714965185927"><a name="evs_04_2069_evs_04_2067_p52714965185927"></a><a name="evs_04_2069_evs_04_2067_p52714965185927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="evs_04_2069_evs_04_2067_p50913593185927"><a name="evs_04_2069_evs_04_2067_p50913593185927"></a><a name="evs_04_2069_evs_04_2067_p50913593185927"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2069_evs_04_2067_row30360408185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p43274016185927"><a name="evs_04_2069_evs_04_2067_p43274016185927"></a><a name="evs_04_2069_evs_04_2067_p43274016185927"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p15534392185927"><a name="evs_04_2069_evs_04_2067_p15534392185927"></a><a name="evs_04_2069_evs_04_2067_p15534392185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p49891705185927"><a name="evs_04_2069_evs_04_2067_p49891705185927"></a><a name="evs_04_2069_evs_04_2067_p49891705185927"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row49550172185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p54141023185927"><a name="evs_04_2069_evs_04_2067_p54141023185927"></a><a name="evs_04_2069_evs_04_2067_p54141023185927"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p23346722185927"><a name="evs_04_2069_evs_04_2067_p23346722185927"></a><a name="evs_04_2069_evs_04_2067_p23346722185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p35416329185927"><a name="evs_04_2069_evs_04_2067_p35416329185927"></a><a name="evs_04_2069_evs_04_2067_p35416329185927"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row35650386185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p2000176185927"><a name="evs_04_2069_evs_04_2067_p2000176185927"></a><a name="evs_04_2069_evs_04_2067_p2000176185927"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p27796542185927"><a name="evs_04_2069_evs_04_2067_p27796542185927"></a><a name="evs_04_2069_evs_04_2067_p27796542185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p38329099185927"><a name="evs_04_2069_evs_04_2067_p38329099185927"></a><a name="evs_04_2069_evs_04_2067_p38329099185927"></a>挂载的时间信息。</p>
    <p id="evs_04_2069_evs_04_2067_p3414132514312"><a name="evs_04_2069_evs_04_2067_p3414132514312"></a><a name="evs_04_2069_evs_04_2067_p3414132514312"></a><span id="evs_04_2069_evs_04_2067_text7299269449"><a name="evs_04_2069_evs_04_2067_text7299269449"></a><a name="evs_04_2069_evs_04_2067_text7299269449"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row9417574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p24626033185927"><a name="evs_04_2069_evs_04_2067_p24626033185927"></a><a name="evs_04_2069_evs_04_2067_p24626033185927"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p48551632185927"><a name="evs_04_2069_evs_04_2067_p48551632185927"></a><a name="evs_04_2069_evs_04_2067_p48551632185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p48591276185927"><a name="evs_04_2069_evs_04_2067_p48591276185927"></a><a name="evs_04_2069_evs_04_2067_p48591276185927"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row34668301185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p56668991185927"><a name="evs_04_2069_evs_04_2067_p56668991185927"></a><a name="evs_04_2069_evs_04_2067_p56668991185927"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p26785545185927"><a name="evs_04_2069_evs_04_2067_p26785545185927"></a><a name="evs_04_2069_evs_04_2067_p26785545185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p48959624185927"><a name="evs_04_2069_evs_04_2067_p48959624185927"></a><a name="evs_04_2069_evs_04_2067_p48959624185927"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row41070280185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p38358373185927"><a name="evs_04_2069_evs_04_2067_p38358373185927"></a><a name="evs_04_2069_evs_04_2067_p38358373185927"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p20020490185927"><a name="evs_04_2069_evs_04_2067_p20020490185927"></a><a name="evs_04_2069_evs_04_2067_p20020490185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p22392462185927"><a name="evs_04_2069_evs_04_2067_p22392462185927"></a><a name="evs_04_2069_evs_04_2067_p22392462185927"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="evs_04_2069_evs_04_2067_row205574185927"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2069_evs_04_2067_p16651565185927"><a name="evs_04_2069_evs_04_2067_p16651565185927"></a><a name="evs_04_2069_evs_04_2067_p16651565185927"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2069_evs_04_2067_p6599487185927"><a name="evs_04_2069_evs_04_2067_p6599487185927"></a><a name="evs_04_2069_evs_04_2067_p6599487185927"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2069_evs_04_2067_p14021450185927"><a name="evs_04_2069_evs_04_2067_p14021450185927"></a><a name="evs_04_2069_evs_04_2067_p14021450185927"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li29114110314"></a>metadata参数说明

    <a name="evs_04_3004_table3430728295554"></a>
    <table><thead align="left"><tr id="evs_04_3004_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_3004_p8809200174410"><a name="evs_04_3004_p8809200174410"></a><a name="evs_04_3004_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_3004_p168135017449"><a name="evs_04_3004_p168135017449"></a><a name="evs_04_3004_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_3004_p1282213034412"><a name="evs_04_3004_p1282213034412"></a><a name="evs_04_3004_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_3004_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p1562408795622"><a name="evs_04_3004_p1562408795622"></a><a name="evs_04_3004_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p5759155095622"><a name="evs_04_3004_p5759155095622"></a><a name="evs_04_3004_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_3004_p177192813501"><a name="evs_04_3004_p177192813501"></a><a name="evs_04_3004_p177192813501"></a>metadata中的表示加密功能的字段。<a name="evs_04_3004_ul141951225145011"></a><a name="evs_04_3004_ul141951225145011"></a><ul id="evs_04_3004_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_3004_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p241272995622"><a name="evs_04_3004_p241272995622"></a><a name="evs_04_3004_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p6121338895622"><a name="evs_04_3004_p6121338895622"></a><a name="evs_04_3004_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_3004_p4159804295622"><a name="evs_04_3004_p4159804295622"></a><a name="evs_04_3004_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="evs_04_3004_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p1478896104915"><a name="evs_04_3004_p1478896104915"></a><a name="evs_04_3004_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p52681767104915"><a name="evs_04_3004_p52681767104915"></a><a name="evs_04_3004_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_3004_p17177177145116"><a name="evs_04_3004_p17177177145116"></a><a name="evs_04_3004_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="evs_04_3004_ul14462208141855"></a><a name="evs_04_3004_ul14462208141855"></a><ul id="evs_04_3004_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_3004_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_3004_p3500156018292"><a name="evs_04_3004_p3500156018292"></a><a name="evs_04_3004_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_3004_p1655411118292"><a name="evs_04_3004_p1655411118292"></a><a name="evs_04_3004_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_3004_p47931946183150"><a name="evs_04_3004_p47931946183150"></a><a name="evs_04_3004_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
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


## 状态码<a name="section63839913"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

