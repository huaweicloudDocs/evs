# 更新云硬盘<a name="ZH-CN_TOPIC_0102644048"></a>

## 功能介绍<a name="section60214390"></a>

更新云硬盘。

## URI<a name="section5058598"></a>

-   URI格式

    PUT /v3/\{project\_id\}/volumes/\{volume\_id\}

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
    <tr id="row11170003"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p32355065"><a name="p32355065"></a><a name="p32355065"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p3514615"><a name="p3514615"></a><a name="p3514615"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p16248438"><a name="p16248438"></a><a name="p16248438"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section45527389"></a>

-   请求参数

    <a name="zh-cn_topic_0058762429_table2126321"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762429_row49924131"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058762429_p37408856172245"><a name="zh-cn_topic_0058762429_p37408856172245"></a><a name="zh-cn_topic_0058762429_p37408856172245"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058762429_p11847581"><a name="zh-cn_topic_0058762429_p11847581"></a><a name="zh-cn_topic_0058762429_p11847581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058762429_p20130041"><a name="zh-cn_topic_0058762429_p20130041"></a><a name="zh-cn_topic_0058762429_p20130041"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="49%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058762429_p19920592"><a name="zh-cn_topic_0058762429_p19920592"></a><a name="zh-cn_topic_0058762429_p19920592"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762429_row55501748173249"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p46048346173251"><a name="zh-cn_topic_0058762429_p46048346173251"></a><a name="zh-cn_topic_0058762429_p46048346173251"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p38928506173251"><a name="zh-cn_topic_0058762429_p38928506173251"></a><a name="zh-cn_topic_0058762429_p38928506173251"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p66201254173251"><a name="zh-cn_topic_0058762429_p66201254173251"></a><a name="zh-cn_topic_0058762429_p66201254173251"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p60701383173251"><a name="zh-cn_topic_0058762429_p60701383173251"></a><a name="zh-cn_topic_0058762429_p60701383173251"></a>待更新的云硬盘信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row64095011151910"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p17428326151912"><a name="zh-cn_topic_0058762429_p17428326151912"></a><a name="zh-cn_topic_0058762429_p17428326151912"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p2408306151912"><a name="zh-cn_topic_0058762429_p2408306151912"></a><a name="zh-cn_topic_0058762429_p2408306151912"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p60855094151912"><a name="zh-cn_topic_0058762429_p60855094151912"></a><a name="zh-cn_topic_0058762429_p60855094151912"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p30315611151912"><a name="zh-cn_topic_0058762429_p30315611151912"></a><a name="zh-cn_topic_0058762429_p30315611151912"></a>云硬盘名称。<span id="zh-cn_topic_0058762429_text18392687151915"><a name="zh-cn_topic_0058762429_text18392687151915"></a><a name="zh-cn_topic_0058762429_text18392687151915"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row22579971154332"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p38689692151834"><a name="zh-cn_topic_0058762429_p38689692151834"></a><a name="zh-cn_topic_0058762429_p38689692151834"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p46857371151834"><a name="zh-cn_topic_0058762429_p46857371151834"></a><a name="zh-cn_topic_0058762429_p46857371151834"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p37350702151834"><a name="zh-cn_topic_0058762429_p37350702151834"></a><a name="zh-cn_topic_0058762429_p37350702151834"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p5508030151834"><a name="zh-cn_topic_0058762429_p5508030151834"></a><a name="zh-cn_topic_0058762429_p5508030151834"></a>云硬盘描述。<span id="zh-cn_topic_0058762429_text37546214151923"><a name="zh-cn_topic_0058762429_text37546214151923"></a><a name="zh-cn_topic_0058762429_text37546214151923"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row8766885152152"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p24732045152159"><a name="zh-cn_topic_0058762429_p24732045152159"></a><a name="zh-cn_topic_0058762429_p24732045152159"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p57138635152159"><a name="zh-cn_topic_0058762429_p57138635152159"></a><a name="zh-cn_topic_0058762429_p57138635152159"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p64826762152159"><a name="zh-cn_topic_0058762429_p64826762152159"></a><a name="zh-cn_topic_0058762429_p64826762152159"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p63795990152036"><a name="zh-cn_topic_0058762429_p63795990152036"></a><a name="zh-cn_topic_0058762429_p63795990152036"></a>云硬盘的元数据。</p>
    <p id="zh-cn_topic_0058762429_p16476402152159"><a name="zh-cn_topic_0058762429_p16476402152159"></a><a name="zh-cn_topic_0058762429_p16476402152159"></a><span id="zh-cn_topic_0058762429_text39777218152047"><a name="zh-cn_topic_0058762429_text39777218152047"></a><a name="zh-cn_topic_0058762429_text39777218152047"></a>元数据中的key和value长度不大于255字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row62503562"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p8330898151834"><a name="zh-cn_topic_0058762429_p8330898151834"></a><a name="zh-cn_topic_0058762429_p8330898151834"></a>display_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p3714153151834"><a name="zh-cn_topic_0058762429_p3714153151834"></a><a name="zh-cn_topic_0058762429_p3714153151834"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p32411005151834"><a name="zh-cn_topic_0058762429_p32411005151834"></a><a name="zh-cn_topic_0058762429_p32411005151834"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p8045749151834"><a name="zh-cn_topic_0058762429_p8045749151834"></a><a name="zh-cn_topic_0058762429_p8045749151834"></a>同name，name和display_name任意指定一个即可（若两个都指定，则以name为主）。<span id="zh-cn_topic_0058762429_text39910621151950"><a name="zh-cn_topic_0058762429_text39910621151950"></a><a name="zh-cn_topic_0058762429_text39910621151950"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row20483630151827"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058762429_p26880332151834"><a name="zh-cn_topic_0058762429_p26880332151834"></a><a name="zh-cn_topic_0058762429_p26880332151834"></a>display_description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058762429_p29823311151834"><a name="zh-cn_topic_0058762429_p29823311151834"></a><a name="zh-cn_topic_0058762429_p29823311151834"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058762429_p66877970151834"><a name="zh-cn_topic_0058762429_p66877970151834"></a><a name="zh-cn_topic_0058762429_p66877970151834"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="49%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058762429_p48406461151834"><a name="zh-cn_topic_0058762429_p48406461151834"></a><a name="zh-cn_topic_0058762429_p48406461151834"></a>同description，description和display_description任意指定一个即可（若两个都指定，则以description为主）。<span id="zh-cn_topic_0058762429_text3105939815201"><a name="zh-cn_topic_0058762429_text3105939815201"></a><a name="zh-cn_topic_0058762429_text3105939815201"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "volume": {
            "name": "test_volume", 
            "description": "test"
        }
    }
    ```


## 响应<a name="section7093323"></a>

-   响应参数

    <a name="zh-cn_topic_0058762429_table34701445142557"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762429_row12524911142557"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762429_p7884856142557"><a name="zh-cn_topic_0058762429_p7884856142557"></a><a name="zh-cn_topic_0058762429_p7884856142557"></a>名称</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762429_p34693598142557"><a name="zh-cn_topic_0058762429_p34693598142557"></a><a name="zh-cn_topic_0058762429_p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762429_p58539486142557"><a name="zh-cn_topic_0058762429_p58539486142557"></a><a name="zh-cn_topic_0058762429_p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762429_row1675773795822"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p2207530595824"><a name="zh-cn_topic_0058762429_p2207530595824"></a><a name="zh-cn_topic_0058762429_p2207530595824"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p4326928995824"><a name="zh-cn_topic_0058762429_p4326928995824"></a><a name="zh-cn_topic_0058762429_p4326928995824"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p1931206295824"><a name="zh-cn_topic_0058762429_p1931206295824"></a><a name="zh-cn_topic_0058762429_p1931206295824"></a>更新后的云硬盘信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row444782011610"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p18308336144438"><a name="zh-cn_topic_0058762429_p18308336144438"></a><a name="zh-cn_topic_0058762429_p18308336144438"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p6580236144438"><a name="zh-cn_topic_0058762429_p6580236144438"></a><a name="zh-cn_topic_0058762429_p6580236144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p21928856144438"><a name="zh-cn_topic_0058762429_p21928856144438"></a><a name="zh-cn_topic_0058762429_p21928856144438"></a>云硬盘ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row44077962142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p14226985144438"><a name="zh-cn_topic_0058762429_p14226985144438"></a><a name="zh-cn_topic_0058762429_p14226985144438"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p50073503191822"><a name="zh-cn_topic_0058762429_p50073503191822"></a><a name="zh-cn_topic_0058762429_p50073503191822"></a>list&lt;map&lt;string,string&gt;&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p50473003144438"><a name="zh-cn_topic_0058762429_p50473003144438"></a><a name="zh-cn_topic_0058762429_p50473003144438"></a>云硬盘URI自描述信息</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row16186817142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p19162411144438"><a name="zh-cn_topic_0058762429_p19162411144438"></a><a name="zh-cn_topic_0058762429_p19162411144438"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p8651439144438"><a name="zh-cn_topic_0058762429_p8651439144438"></a><a name="zh-cn_topic_0058762429_p8651439144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p55103877144438"><a name="zh-cn_topic_0058762429_p55103877144438"></a><a name="zh-cn_topic_0058762429_p55103877144438"></a>云硬盘名称</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row2987651144410"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p39625821144438"><a name="zh-cn_topic_0058762429_p39625821144438"></a><a name="zh-cn_topic_0058762429_p39625821144438"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p55574965144438"><a name="zh-cn_topic_0058762429_p55574965144438"></a><a name="zh-cn_topic_0058762429_p55574965144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p24889213144438"><a name="zh-cn_topic_0058762429_p24889213144438"></a><a name="zh-cn_topic_0058762429_p24889213144438"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a></p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row45785905142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p24843442144438"><a name="zh-cn_topic_0058762429_p24843442144438"></a><a name="zh-cn_topic_0058762429_p24843442144438"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p66161799144438"><a name="zh-cn_topic_0058762429_p66161799144438"></a><a name="zh-cn_topic_0058762429_p66161799144438"></a>array</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p27432950144438"><a name="zh-cn_topic_0058762429_p27432950144438"></a><a name="zh-cn_topic_0058762429_p27432950144438"></a>挂载信息</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row35247553142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p179170144438"><a name="zh-cn_topic_0058762429_p179170144438"></a><a name="zh-cn_topic_0058762429_p179170144438"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p14512814144438"><a name="zh-cn_topic_0058762429_p14512814144438"></a><a name="zh-cn_topic_0058762429_p14512814144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p58206487144438"><a name="zh-cn_topic_0058762429_p58206487144438"></a><a name="zh-cn_topic_0058762429_p58206487144438"></a>云硬盘所属AZ</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row27126244142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p19727534144438"><a name="zh-cn_topic_0058762429_p19727534144438"></a><a name="zh-cn_topic_0058762429_p19727534144438"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p54426427144438"><a name="zh-cn_topic_0058762429_p54426427144438"></a><a name="zh-cn_topic_0058762429_p54426427144438"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p5526931144438"><a name="zh-cn_topic_0058762429_p5526931144438"></a><a name="zh-cn_topic_0058762429_p5526931144438"></a>是否为可启动云硬盘</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row7009490142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p2601247144438"><a name="zh-cn_topic_0058762429_p2601247144438"></a><a name="zh-cn_topic_0058762429_p2601247144438"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p9374472144438"><a name="zh-cn_topic_0058762429_p9374472144438"></a><a name="zh-cn_topic_0058762429_p9374472144438"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p34192098144438"><a name="zh-cn_topic_0058762429_p34192098144438"></a><a name="zh-cn_topic_0058762429_p34192098144438"></a>是否为加密云硬盘</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row49237196142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p28651206144438"><a name="zh-cn_topic_0058762429_p28651206144438"></a><a name="zh-cn_topic_0058762429_p28651206144438"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p1296456144535"><a name="zh-cn_topic_0058762429_p1296456144535"></a><a name="zh-cn_topic_0058762429_p1296456144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p28821893144438"><a name="zh-cn_topic_0058762429_p28821893144438"></a><a name="zh-cn_topic_0058762429_p28821893144438"></a>创建云硬盘的时间</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row39017307142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p6085885144438"><a name="zh-cn_topic_0058762429_p6085885144438"></a><a name="zh-cn_topic_0058762429_p6085885144438"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p18611115144535"><a name="zh-cn_topic_0058762429_p18611115144535"></a><a name="zh-cn_topic_0058762429_p18611115144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p44410693144438"><a name="zh-cn_topic_0058762429_p44410693144438"></a><a name="zh-cn_topic_0058762429_p44410693144438"></a>云硬盘描述</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row20107664142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p28923171144438"><a name="zh-cn_topic_0058762429_p28923171144438"></a><a name="zh-cn_topic_0058762429_p28923171144438"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p22198851144535"><a name="zh-cn_topic_0058762429_p22198851144535"></a><a name="zh-cn_topic_0058762429_p22198851144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p9630579144438"><a name="zh-cn_topic_0058762429_p9630579144438"></a><a name="zh-cn_topic_0058762429_p9630579144438"></a>云硬盘类型</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row12897861142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p41370851144438"><a name="zh-cn_topic_0058762429_p41370851144438"></a><a name="zh-cn_topic_0058762429_p41370851144438"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p7354807144535"><a name="zh-cn_topic_0058762429_p7354807144535"></a><a name="zh-cn_topic_0058762429_p7354807144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p27786537144438"><a name="zh-cn_topic_0058762429_p27786537144438"></a><a name="zh-cn_topic_0058762429_p27786537144438"></a>云硬盘复制状态</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row45680217142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p56617581144438"><a name="zh-cn_topic_0058762429_p56617581144438"></a><a name="zh-cn_topic_0058762429_p56617581144438"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p25180208144535"><a name="zh-cn_topic_0058762429_p25180208144535"></a><a name="zh-cn_topic_0058762429_p25180208144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p40860550144438"><a name="zh-cn_topic_0058762429_p40860550144438"></a><a name="zh-cn_topic_0058762429_p40860550144438"></a>所属一致性组ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row47480567142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p58114746144438"><a name="zh-cn_topic_0058762429_p58114746144438"></a><a name="zh-cn_topic_0058762429_p58114746144438"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p47440982144535"><a name="zh-cn_topic_0058762429_p47440982144535"></a><a name="zh-cn_topic_0058762429_p47440982144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p52975605144438"><a name="zh-cn_topic_0058762429_p52975605144438"></a><a name="zh-cn_topic_0058762429_p52975605144438"></a>源云硬盘ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row31517135142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p31619531144438"><a name="zh-cn_topic_0058762429_p31619531144438"></a><a name="zh-cn_topic_0058762429_p31619531144438"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p66078031144535"><a name="zh-cn_topic_0058762429_p66078031144535"></a><a name="zh-cn_topic_0058762429_p66078031144535"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p57055846144438"><a name="zh-cn_topic_0058762429_p57055846144438"></a><a name="zh-cn_topic_0058762429_p57055846144438"></a>快照ID</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row15610713142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p53325033144438"><a name="zh-cn_topic_0058762429_p53325033144438"></a><a name="zh-cn_topic_0058762429_p53325033144438"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p24360403144438"><a name="zh-cn_topic_0058762429_p24360403144438"></a><a name="zh-cn_topic_0058762429_p24360403144438"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p42403730144438"><a name="zh-cn_topic_0058762429_p42403730144438"></a><a name="zh-cn_topic_0058762429_p42403730144438"></a>元数据</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row5657368142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p42241765144438"><a name="zh-cn_topic_0058762429_p42241765144438"></a><a name="zh-cn_topic_0058762429_p42241765144438"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p66139813144438"><a name="zh-cn_topic_0058762429_p66139813144438"></a><a name="zh-cn_topic_0058762429_p66139813144438"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p17400122144438"><a name="zh-cn_topic_0058762429_p17400122144438"></a><a name="zh-cn_topic_0058762429_p17400122144438"></a>云硬盘大小</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row39412545144428"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p1113688144438"><a name="zh-cn_topic_0058762429_p1113688144438"></a><a name="zh-cn_topic_0058762429_p1113688144438"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p51894643144540"><a name="zh-cn_topic_0058762429_p51894643144540"></a><a name="zh-cn_topic_0058762429_p51894643144540"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p109947201368"><a name="zh-cn_topic_0058762429_p109947201368"></a><a name="zh-cn_topic_0058762429_p109947201368"></a>预留属性</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row25381049144431"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p26680804144438"><a name="zh-cn_topic_0058762429_p26680804144438"></a><a name="zh-cn_topic_0058762429_p26680804144438"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p39072645144540"><a name="zh-cn_topic_0058762429_p39072645144540"></a><a name="zh-cn_topic_0058762429_p39072645144540"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p42877354144438"><a name="zh-cn_topic_0058762429_p42877354144438"></a><a name="zh-cn_topic_0058762429_p42877354144438"></a>云硬盘更新时间</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row48384415144425"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p51969649144438"><a name="zh-cn_topic_0058762429_p51969649144438"></a><a name="zh-cn_topic_0058762429_p51969649144438"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p48792012144438"><a name="zh-cn_topic_0058762429_p48792012144438"></a><a name="zh-cn_topic_0058762429_p48792012144438"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p15113052144438"><a name="zh-cn_topic_0058762429_p15113052144438"></a><a name="zh-cn_topic_0058762429_p15113052144438"></a>是否为可共享云硬盘</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_row42462677142557"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_p11561839144438"><a name="zh-cn_topic_0058762429_p11561839144438"></a><a name="zh-cn_topic_0058762429_p11561839144438"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_p64093800144438"><a name="zh-cn_topic_0058762429_p64093800144438"></a><a name="zh-cn_topic_0058762429_p64093800144438"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_p15283679144438"><a name="zh-cn_topic_0058762429_p15283679144438"></a><a name="zh-cn_topic_0058762429_p15283679144438"></a>是否为可共享云硬盘</p>
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

    <a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_table3430728295554"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p8809200174410"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p8809200174410"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p168135017449"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p168135017449"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1282213034412"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1282213034412"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1562408795622"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1562408795622"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p5759155095622"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p5759155095622"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p5759155095622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p177192813501"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p177192813501"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p177192813501"></a>metadata中的表示加密功能的字段。<a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul141951225145011"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul141951225145011"></a><ul id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p241272995622"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p241272995622"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p6121338895622"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p6121338895622"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p6121338895622"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p4159804295622"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p4159804295622"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1478896104915"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1478896104915"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p52681767104915"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p52681767104915"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p52681767104915"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p17177177145116"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p17177177145116"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul14462208141855"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul14462208141855"></a><ul id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3500156018292"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3500156018292"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1655411118292"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1655411118292"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1655411118292"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p47931946183150"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p47931946183150"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row16478023164611"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p15479323204615"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p15479323204615"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p15479323204615"></a>readonly</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p134792232467"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p134792232467"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p134792232467"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3479112318462"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3479112318462"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p3479112318462"></a>是否为只读模式云硬盘。<a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul11587123175320"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul11587123175320"></a><ul id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul11587123175320"><li>True表示云硬盘仅支持可读模式。</li><li>False表示云硬盘支持读写模式。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_row347911235465"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p18479142364612"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p18479142364612"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p18479142364612"></a>attached_mode</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1547917231465"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1547917231465"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p1547917231465"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p11479102334617"><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p11479102334617"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_p11479102334617"></a>只有当云硬盘已挂载至云服务器时，才有该字段，表示云硬盘的使用模式。<a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul17760125635418"></a><a name="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul17760125635418"></a><ul id="zh-cn_topic_0058762429_zh-cn_topic_0102756196_ul17760125635418"><li>ro表示只读模式。</li><li>rw表示读写模式。</li></ul>
    </div>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "volume": {
            "attachments": [ ], 
            "availability_zone": "xxx", 
            "bootable": "false", 
            "consistencygroup_id": null, 
            "created_at": "2016-05-25T02:38:40.392463", 
            "description": "create for api test", 
            "encrypted": false, 
            "id": "8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
            "links": [
                {
                    "href": "https://volume.localdomain.com:8776/v2/5dd0b0056f3d47b6ab4121667d35621a/volumes/8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
                    "rel": "self"
                }, 
                {
                    "href": "https://volume.localdomain.com:8776/5dd0b0056f3d47b6ab4121667d35621a/volumes/8dd7c486-8e9f-49fe-bceb-26aa7e312b66", 
                    "rel": "bookmark"
                }
            ], 
            "metadata": {
                "volume_owner": "openapi"
            }, 
            "name": "openapi_vol01", 
            "replication_status": "disabled", 
            "multiattach": false, 
            "size": 40, 
            "snapshot_id": null, 
            "source_volid": null, 
            "status": "creating", 
            "updated_at": null, 
            "user_id": "39f6696ae23740708d0f358a253c2637", 
            "volume_type": "SATA"
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错为：

    ```
    {
        "badRequest": {
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

