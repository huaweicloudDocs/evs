# 查询单个云硬盘详情<a name="evs_04_2007"></a>

## 功能介绍<a name="section60214390"></a>

查询单个云硬盘的详细信息。支持企业项目授权功能。

## URI<a name="section5058598"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudvolumes/\{volume\_id\}

-   参数说明

    <a name="evs_04_2011_table58294385"></a>
    <table><thead align="left"><tr id="evs_04_2011_row24683273"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="evs_04_2011_p53188122"><a name="evs_04_2011_p53188122"></a><a name="evs_04_2011_p53188122"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="evs_04_2011_p13270664"><a name="evs_04_2011_p13270664"></a><a name="evs_04_2011_p13270664"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="evs_04_2011_p1182010"><a name="evs_04_2011_p1182010"></a><a name="evs_04_2011_p1182010"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_row28634009"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p37653388"><a name="evs_04_2011_p37653388"></a><a name="evs_04_2011_p37653388"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p30025596"><a name="evs_04_2011_p30025596"></a><a name="evs_04_2011_p30025596"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p16154192"><a name="evs_04_2011_p16154192"></a><a name="evs_04_2011_p16154192"></a>项目ID。</p>
    <p id="evs_04_2011_p55811451337"><a name="evs_04_2011_p55811451337"></a><a name="evs_04_2011_p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row11170003"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p32355065"><a name="evs_04_2011_p32355065"></a><a name="evs_04_2011_p32355065"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p3514615"><a name="evs_04_2011_p3514615"></a><a name="evs_04_2011_p3514615"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p16248438"><a name="evs_04_2011_p16248438"></a><a name="evs_04_2011_p16248438"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

-   请求样例

    ```
    GET https://{endpoint}/v2/{project_id}/cloudvolumes/b104b8db-170d-441b-897a-3c8ba9c5a214
    ```


## 响应消息<a name="section7093323"></a>

-   响应参数

    <a name="evs_04_2011_table10924124020519"></a>
    <table><thead align="left"><tr id="evs_04_2011_row11924194015519"><th class="cellrowborder" valign="top" width="18.82%" id="mcps1.1.4.1.1"><p id="evs_04_2011_p1925340155113"><a name="evs_04_2011_p1925340155113"></a><a name="evs_04_2011_p1925340155113"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.580000000000002%" id="mcps1.1.4.1.2"><p id="evs_04_2011_p13925440205111"><a name="evs_04_2011_p13925440205111"></a><a name="evs_04_2011_p13925440205111"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.599999999999994%" id="mcps1.1.4.1.3"><p id="evs_04_2011_p99250405513"><a name="evs_04_2011_p99250405513"></a><a name="evs_04_2011_p99250405513"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_row159251409514"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1292513408516"><a name="evs_04_2011_p1292513408516"></a><a name="evs_04_2011_p1292513408516"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p392564017518"><a name="evs_04_2011_p392564017518"></a><a name="evs_04_2011_p392564017518"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p16925134045115"><a name="evs_04_2011_p16925134045115"></a><a name="evs_04_2011_p16925134045115"></a>查询请求返回的云硬盘，请参见<a href="#evs_04_2011_li3451542201439">•volume参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row143812361506"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p129522216412"><a name="evs_04_2011_p129522216412"></a><a name="evs_04_2011_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1595262111415"><a name="evs_04_2011_p1595262111415"></a><a name="evs_04_2011_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p109527215417"><a name="evs_04_2011_p109527215417"></a><a name="evs_04_2011_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2011_li0419202382514"> error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2011_li3451542201439"></a>volume参数说明

    <a name="evs_04_2011_table34701445142557"></a>
    <table><thead align="left"><tr id="evs_04_2011_row12524911142557"><th class="cellrowborder" valign="top" width="18.82%" id="mcps1.1.4.1.1"><p id="evs_04_2011_p7884856142557"><a name="evs_04_2011_p7884856142557"></a><a name="evs_04_2011_p7884856142557"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.580000000000002%" id="mcps1.1.4.1.2"><p id="evs_04_2011_p34693598142557"><a name="evs_04_2011_p34693598142557"></a><a name="evs_04_2011_p34693598142557"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.599999999999994%" id="mcps1.1.4.1.3"><p id="evs_04_2011_p58539486142557"><a name="evs_04_2011_p58539486142557"></a><a name="evs_04_2011_p58539486142557"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_row44077962142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p13545137142557"><a name="evs_04_2011_p13545137142557"></a><a name="evs_04_2011_p13545137142557"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p23414333142557"><a name="evs_04_2011_p23414333142557"></a><a name="evs_04_2011_p23414333142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p9255075142557"><a name="evs_04_2011_p9255075142557"></a><a name="evs_04_2011_p9255075142557"></a><span id="evs_04_2011_text193761052172315"><a name="evs_04_2011_text193761052172315"></a><a name="evs_04_2011_text193761052172315"></a>云硬盘的ID。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row16186817142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p36063800142557"><a name="evs_04_2011_p36063800142557"></a><a name="evs_04_2011_p36063800142557"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p35486679142557"><a name="evs_04_2011_p35486679142557"></a><a name="evs_04_2011_p35486679142557"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p27456944142557"><a name="evs_04_2011_p27456944142557"></a><a name="evs_04_2011_p27456944142557"></a>云硬盘URI自描述信息，请参见<a href="#evs_04_2011_li4929184617138">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row45785905142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p17670785142557"><a name="evs_04_2011_p17670785142557"></a><a name="evs_04_2011_p17670785142557"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p22047453142557"><a name="evs_04_2011_p22047453142557"></a><a name="evs_04_2011_p22047453142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p33742556142557"><a name="evs_04_2011_p33742556142557"></a><a name="evs_04_2011_p33742556142557"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row35247553142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p36479557142557"><a name="evs_04_2011_p36479557142557"></a><a name="evs_04_2011_p36479557142557"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p2054104142557"><a name="evs_04_2011_p2054104142557"></a><a name="evs_04_2011_p2054104142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p55209810142557"><a name="evs_04_2011_p55209810142557"></a><a name="evs_04_2011_p55209810142557"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row27126244142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p49742149142557"><a name="evs_04_2011_p49742149142557"></a><a name="evs_04_2011_p49742149142557"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p2582234142557"><a name="evs_04_2011_p2582234142557"></a><a name="evs_04_2011_p2582234142557"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p30604994142557"><a name="evs_04_2011_p30604994142557"></a><a name="evs_04_2011_p30604994142557"></a>云硬盘的挂载信息，请参见<a href="#evs_04_2011_li4186567617138">•attachments参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row7009490142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p30897802142557"><a name="evs_04_2011_p30897802142557"></a><a name="evs_04_2011_p30897802142557"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p19694010142557"><a name="evs_04_2011_p19694010142557"></a><a name="evs_04_2011_p19694010142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p27840420142557"><a name="evs_04_2011_p27840420142557"></a><a name="evs_04_2011_p27840420142557"></a>云硬盘所属的AZ信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row49237196142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p28789925142557"><a name="evs_04_2011_p28789925142557"></a><a name="evs_04_2011_p28789925142557"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p50282587142557"><a name="evs_04_2011_p50282587142557"></a><a name="evs_04_2011_p50282587142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p63987579142557"><a name="evs_04_2011_p63987579142557"></a><a name="evs_04_2011_p63987579142557"></a>源云硬盘ID，如果是从源云硬盘创建，则有值。</p>
    <p id="evs_04_2011_p102771156662"><a name="evs_04_2011_p102771156662"></a><a name="evs_04_2011_p102771156662"></a><span id="evs_04_2011_text88578719717"><a name="evs_04_2011_text88578719717"></a><a name="evs_04_2011_text88578719717"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row39017307142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p6285295142557"><a name="evs_04_2011_p6285295142557"></a><a name="evs_04_2011_p6285295142557"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p39346916142557"><a name="evs_04_2011_p39346916142557"></a><a name="evs_04_2011_p39346916142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p54429968142557"><a name="evs_04_2011_p54429968142557"></a><a name="evs_04_2011_p54429968142557"></a>快照ID，如果是从快照创建，则有值。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row20107664142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p18108106142557"><a name="evs_04_2011_p18108106142557"></a><a name="evs_04_2011_p18108106142557"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p57470472142557"><a name="evs_04_2011_p57470472142557"></a><a name="evs_04_2011_p57470472142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p46172338142557"><a name="evs_04_2011_p46172338142557"></a><a name="evs_04_2011_p46172338142557"></a>云硬盘描述。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row12897861142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p38093790142557"><a name="evs_04_2011_p38093790142557"></a><a name="evs_04_2011_p38093790142557"></a>os-vol-tenant-attr:tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p65698111142557"><a name="evs_04_2011_p65698111142557"></a><a name="evs_04_2011_p65698111142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p5075579142557"><a name="evs_04_2011_p5075579142557"></a><a name="evs_04_2011_p5075579142557"></a>云硬盘所属的租户ID。<span id="evs_04_2011_text19941457165313"><a name="evs_04_2011_text19941457165313"></a><a name="evs_04_2011_text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row45680217142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p9110107142557"><a name="evs_04_2011_p9110107142557"></a><a name="evs_04_2011_p9110107142557"></a>volume_image_metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p66830090142557"><a name="evs_04_2011_p66830090142557"></a><a name="evs_04_2011_p66830090142557"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p50014861142557"><a name="evs_04_2011_p50014861142557"></a><a name="evs_04_2011_p50014861142557"></a>云硬盘镜像的元数据。</p>
    <div class="note" id="evs_04_2011_note410975220289"><a name="evs_04_2011_note410975220289"></a><a name="evs_04_2011_note410975220289"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2011_evs_04_2009_p16054517146"><a name="evs_04_2011_evs_04_2009_p16054517146"></a><a name="evs_04_2011_evs_04_2009_p16054517146"></a>关于“volume_image_metadata”字段的详细说明，具体请参见<a href="https://support.huaweicloud.com/api-ims/ims_03_0703.html" target="_blank" rel="noopener noreferrer">查询镜像详情（OpenStack原生）</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2011_row47480567142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p20720700142557"><a name="evs_04_2011_p20720700142557"></a><a name="evs_04_2011_p20720700142557"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p655154142557"><a name="evs_04_2011_p655154142557"></a><a name="evs_04_2011_p655154142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p3501903142557"><a name="evs_04_2011_p3501903142557"></a><a name="evs_04_2011_p3501903142557"></a>云硬盘创建时间。</p>
    <p id="evs_04_2011_p1834613217531"><a name="evs_04_2011_p1834613217531"></a><a name="evs_04_2011_p1834613217531"></a><span id="evs_04_2011_text153631054195313"><a name="evs_04_2011_text153631054195313"></a><a name="evs_04_2011_text153631054195313"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row31517135142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p2751105142557"><a name="evs_04_2011_p2751105142557"></a><a name="evs_04_2011_p2751105142557"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p21512968142557"><a name="evs_04_2011_p21512968142557"></a><a name="evs_04_2011_p21512968142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p16647604142557"><a name="evs_04_2011_p16647604142557"></a><a name="evs_04_2011_p16647604142557"></a>云硬盘类型。</p>
    <div class="p" id="evs_04_2011_zh-cn_topic_0044524833_p112762317377"><a name="evs_04_2011_zh-cn_topic_0044524833_p112762317377"></a><a name="evs_04_2011_zh-cn_topic_0044524833_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="evs_04_2011_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="evs_04_2011_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="evs_04_2011_zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2011_row15610713142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p56508275142557"><a name="evs_04_2011_p56508275142557"></a><a name="evs_04_2011_p56508275142557"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p13767590142557"><a name="evs_04_2011_p13767590142557"></a><a name="evs_04_2011_p13767590142557"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p628596142557"><a name="evs_04_2011_p628596142557"></a><a name="evs_04_2011_p628596142557"></a>云硬盘大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row5657368142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p55593700142557"><a name="evs_04_2011_p55593700142557"></a><a name="evs_04_2011_p55593700142557"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p6795819142557"><a name="evs_04_2011_p6795819142557"></a><a name="evs_04_2011_p6795819142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2011_zh-cn_topic_0098680634_p8780414125315"><a name="evs_04_2011_zh-cn_topic_0098680634_p8780414125315"></a><a name="evs_04_2011_zh-cn_topic_0098680634_p8780414125315"></a>是否为启动云硬盘。<a name="evs_04_2011_ul185931714111"></a><a name="evs_04_2011_ul185931714111"></a><ul id="evs_04_2011_ul185931714111"><li>true：表示为启动云硬盘。</li><li>false：表示为非启动云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2011_row42462677142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p16924779142557"><a name="evs_04_2011_p16924779142557"></a><a name="evs_04_2011_p16924779142557"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p28729858142557"><a name="evs_04_2011_p28729858142557"></a><a name="evs_04_2011_p28729858142557"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p2976878614485"><a name="evs_04_2011_p2976878614485"></a><a name="evs_04_2011_p2976878614485"></a>云硬盘的元数据，请参见<a href="#evs_04_2011_li29114110314">•metadata参数说明</a>。</p>
    <p id="evs_04_2011_p6664089144810"><a name="evs_04_2011_p6664089144810"></a><a name="evs_04_2011_p6664089144810"></a>如果元数据中不包含hw:passthrough字段，云硬盘默认为VBD类型。</p>
    <p id="evs_04_2011_p27113282155030"><a name="evs_04_2011_p27113282155030"></a><a name="evs_04_2011_p27113282155030"></a>如果元数据中不包含__system__encrypted字段，云硬盘默认为不加密。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row24435167142557"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p33091499142557"><a name="evs_04_2011_p33091499142557"></a><a name="evs_04_2011_p33091499142557"></a>os-vol-host-attr:host</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p63165723142557"><a name="evs_04_2011_p63165723142557"></a><a name="evs_04_2011_p63165723142557"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p33074440142557"><a name="evs_04_2011_p33074440142557"></a><a name="evs_04_2011_p33074440142557"></a><span id="evs_04_2011_text203605127103"><a name="evs_04_2011_text203605127103"></a><a name="evs_04_2011_text203605127103"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row16261731102710"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p47452553185118"><a name="evs_04_2011_p47452553185118"></a><a name="evs_04_2011_p47452553185118"></a>encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p18451581185118"><a name="evs_04_2011_p18451581185118"></a><a name="evs_04_2011_p18451581185118"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p27951625185124"><a name="evs_04_2011_p27951625185124"></a><a name="evs_04_2011_p27951625185124"></a><span id="evs_04_2011_text1610112322316"><a name="evs_04_2011_text1610112322316"></a><a name="evs_04_2011_text1610112322316"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row319029143856"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p25841403143856"><a name="evs_04_2011_p25841403143856"></a><a name="evs_04_2011_p25841403143856"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p12778905143856"><a name="evs_04_2011_p12778905143856"></a><a name="evs_04_2011_p12778905143856"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p23431040143856"><a name="evs_04_2011_p23431040143856"></a><a name="evs_04_2011_p23431040143856"></a>云硬盘更新时间。</p>
    <p id="evs_04_2011_p088761318554"><a name="evs_04_2011_p088761318554"></a><a name="evs_04_2011_p088761318554"></a><span id="evs_04_2011_text935132417554"><a name="evs_04_2011_text935132417554"></a><a name="evs_04_2011_text935132417554"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row6226231314391"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1008260514391"><a name="evs_04_2011_p1008260514391"></a><a name="evs_04_2011_p1008260514391"></a>os-volume-replication:extended_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1138464014391"><a name="evs_04_2011_p1138464014391"></a><a name="evs_04_2011_p1138464014391"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p246367414391"><a name="evs_04_2011_p246367414391"></a><a name="evs_04_2011_p246367414391"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row1430942214399"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1821254814399"><a name="evs_04_2011_p1821254814399"></a><a name="evs_04_2011_p1821254814399"></a>replication_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p6593029014399"><a name="evs_04_2011_p6593029014399"></a><a name="evs_04_2011_p6593029014399"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p5201068114399"><a name="evs_04_2011_p5201068114399"></a><a name="evs_04_2011_p5201068114399"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row1801485814395"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p4991739214395"><a name="evs_04_2011_p4991739214395"></a><a name="evs_04_2011_p4991739214395"></a>os-vol-mig-status-attr:migstat</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p55570357144311"><a name="evs_04_2011_p55570357144311"></a><a name="evs_04_2011_p55570357144311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p61763041144311"><a name="evs_04_2011_p61763041144311"></a><a name="evs_04_2011_p61763041144311"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row46340323144336"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p62578689144336"><a name="evs_04_2011_p62578689144336"></a><a name="evs_04_2011_p62578689144336"></a>consistencygroup_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p20253849144646"><a name="evs_04_2011_p20253849144646"></a><a name="evs_04_2011_p20253849144646"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p9956989144646"><a name="evs_04_2011_p9956989144646"></a><a name="evs_04_2011_p9956989144646"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row36758187144417"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p24623167144417"><a name="evs_04_2011_p24623167144417"></a><a name="evs_04_2011_p24623167144417"></a>os-vol-mig-status-attr:name_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p34730547144648"><a name="evs_04_2011_p34730547144648"></a><a name="evs_04_2011_p34730547144648"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p32527650144648"><a name="evs_04_2011_p32527650144648"></a><a name="evs_04_2011_p32527650144648"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row30115821144625"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p23462435144625"><a name="evs_04_2011_p23462435144625"></a><a name="evs_04_2011_p23462435144625"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p48108796144650"><a name="evs_04_2011_p48108796144650"></a><a name="evs_04_2011_p48108796144650"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p28827892144650"><a name="evs_04_2011_p28827892144650"></a><a name="evs_04_2011_p28827892144650"></a>是否为共享云硬盘。</p>
    <div class="note" id="evs_04_2011_note3800959821323"><a name="evs_04_2011_note3800959821323"></a><a name="evs_04_2011_note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2011_p45212589213213"><a name="evs_04_2011_p45212589213213"></a><a name="evs_04_2011_p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2011_row4658776614505"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1551273614505"><a name="evs_04_2011_p1551273614505"></a><a name="evs_04_2011_p1551273614505"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p4857213114505"><a name="evs_04_2011_p4857213114505"></a><a name="evs_04_2011_p4857213114505"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p4886676914505"><a name="evs_04_2011_p4886676914505"></a><a name="evs_04_2011_p4886676914505"></a>预留属性。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row16426724115040"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p59918584115045"><a name="evs_04_2011_p59918584115045"></a><a name="evs_04_2011_p59918584115045"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p21567161115045"><a name="evs_04_2011_p21567161115045"></a><a name="evs_04_2011_p21567161115045"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2011_zh-cn_topic_0098680634_p4781191416535"><a name="evs_04_2011_zh-cn_topic_0098680634_p4781191416535"></a><a name="evs_04_2011_zh-cn_topic_0098680634_p4781191416535"></a>是否为共享云硬盘。<a name="evs_04_2011_ul161621719119"></a><a name="evs_04_2011_ul161621719119"></a><ul id="evs_04_2011_ul161621719119"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2011_row115471547175713"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p47811214165316"><a name="evs_04_2011_p47811214165316"></a><a name="evs_04_2011_p47811214165316"></a>service_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p107811114125311"><a name="evs_04_2011_p107811114125311"></a><a name="evs_04_2011_p107811114125311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p17781151418539"><a name="evs_04_2011_p17781151418539"></a><a name="evs_04_2011_p17781151418539"></a>服务类型，结果为EVS、DSS、DESS。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row620045015579"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p12781121410537"><a name="evs_04_2011_p12781121410537"></a><a name="evs_04_2011_p12781121410537"></a>dedicated_storage_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1278151417534"><a name="evs_04_2011_p1278151417534"></a><a name="evs_04_2011_p1278151417534"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p12781111465310"><a name="evs_04_2011_p12781111465310"></a><a name="evs_04_2011_p12781111465310"></a>云硬盘所属的专属存储池ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row03921454195718"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1178131435314"><a name="evs_04_2011_p1178131435314"></a><a name="evs_04_2011_p1178131435314"></a>dedicated_storage_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1478161475312"><a name="evs_04_2011_p1478161475312"></a><a name="evs_04_2011_p1478161475312"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p1781171475316"><a name="evs_04_2011_p1781171475316"></a><a name="evs_04_2011_p1781171475316"></a>云硬盘所属的专属存储池的名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row1393175475712"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p69881644104318"><a name="evs_04_2011_p69881644104318"></a><a name="evs_04_2011_p69881644104318"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1198854414439"><a name="evs_04_2011_p1198854414439"></a><a name="evs_04_2011_p1198854414439"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p18988144418437"><a name="evs_04_2011_p18988144418437"></a><a name="evs_04_2011_p18988144418437"></a>云硬盘的标签。</p>
    <p id="evs_04_2011_p898894418432"><a name="evs_04_2011_p898894418432"></a><a name="evs_04_2011_p898894418432"></a>如果云硬盘有标签，则会有该字段，否则该字段为空。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row189091958125710"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p149881344124319"><a name="evs_04_2011_p149881344124319"></a><a name="evs_04_2011_p149881344124319"></a>wwn</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p3988174494319"><a name="evs_04_2011_p3988174494319"></a><a name="evs_04_2011_p3988174494319"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p6988244114313"><a name="evs_04_2011_p6988244114313"></a><a name="evs_04_2011_p6988244114313"></a>云硬盘挂载时的唯一标识。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row1971632951911"><td class="cellrowborder" valign="top" width="18.82%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p39941261495"><a name="evs_04_2011_p39941261495"></a><a name="evs_04_2011_p39941261495"></a>enterprise_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.580000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p1499413644915"><a name="evs_04_2011_p1499413644915"></a><a name="evs_04_2011_p1499413644915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.599999999999994%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p35013964916"><a name="evs_04_2011_p35013964916"></a><a name="evs_04_2011_p35013964916"></a>云硬盘上绑定的企业项目ID。</p>
    <div class="note" id="evs_04_2011_note6417183517"><a name="evs_04_2011_note6417183517"></a><a name="evs_04_2011_note6417183517"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2011_evs_04_2013_p18336524404"><a name="evs_04_2011_evs_04_2013_p18336524404"></a><a name="evs_04_2011_evs_04_2013_p18336524404"></a>关于企业项目ID的获取及企业项目特性的详细信息，请参见<a href="https://support.huaweicloud.com/usermanual-em/zh-cn_topic_0123692049.html" target="_blank" rel="noopener noreferrer">企业管理用户指南</a>。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2011_li4929184617138"></a>links参数说明

    <a name="evs_04_2011_table53116786111129"></a>
    <table><thead align="left"><tr id="evs_04_2011_row38921210111129"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="evs_04_2011_p65610305111129"><a name="evs_04_2011_p65610305111129"></a><a name="evs_04_2011_p65610305111129"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="evs_04_2011_p12834480111129"><a name="evs_04_2011_p12834480111129"></a><a name="evs_04_2011_p12834480111129"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2011_p52513065111129"><a name="evs_04_2011_p52513065111129"></a><a name="evs_04_2011_p52513065111129"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_row25699842111129"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p1312419111129"><a name="evs_04_2011_p1312419111129"></a><a name="evs_04_2011_p1312419111129"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p39197109111129"><a name="evs_04_2011_p39197109111129"></a><a name="evs_04_2011_p39197109111129"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p11067466111129"><a name="evs_04_2011_p11067466111129"></a><a name="evs_04_2011_p11067466111129"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row32498335111129"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p15119502111129"><a name="evs_04_2011_p15119502111129"></a><a name="evs_04_2011_p15119502111129"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p16720145111129"><a name="evs_04_2011_p16720145111129"></a><a name="evs_04_2011_p16720145111129"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p44991477111129"><a name="evs_04_2011_p44991477111129"></a><a name="evs_04_2011_p44991477111129"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2011_li4186567617138"></a>attachments参数说明

    <a name="evs_04_2011_table2886066111147"></a>
    <table><thead align="left"><tr id="evs_04_2011_row7036686111147"><th class="cellrowborder" valign="top" width="19.27807219278072%" id="mcps1.1.4.1.1"><p id="evs_04_2011_p33100723111147"><a name="evs_04_2011_p33100723111147"></a><a name="evs_04_2011_p33100723111147"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.0975902409759%" id="mcps1.1.4.1.2"><p id="evs_04_2011_p63912929111147"><a name="evs_04_2011_p63912929111147"></a><a name="evs_04_2011_p63912929111147"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.624337566243376%" id="mcps1.1.4.1.3"><p id="evs_04_2011_p36546037111147"><a name="evs_04_2011_p36546037111147"></a><a name="evs_04_2011_p36546037111147"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_row7439020111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p65689739111147"><a name="evs_04_2011_p65689739111147"></a><a name="evs_04_2011_p65689739111147"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p19268667111147"><a name="evs_04_2011_p19268667111147"></a><a name="evs_04_2011_p19268667111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p55737901111147"><a name="evs_04_2011_p55737901111147"></a><a name="evs_04_2011_p55737901111147"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row31879061111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p32067121111147"><a name="evs_04_2011_p32067121111147"></a><a name="evs_04_2011_p32067121111147"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p47300034111147"><a name="evs_04_2011_p47300034111147"></a><a name="evs_04_2011_p47300034111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p24142306111147"><a name="evs_04_2011_p24142306111147"></a><a name="evs_04_2011_p24142306111147"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row23348196112253"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p12155729112253"><a name="evs_04_2011_p12155729112253"></a><a name="evs_04_2011_p12155729112253"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p45090011112253"><a name="evs_04_2011_p45090011112253"></a><a name="evs_04_2011_p45090011112253"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p19692132112253"><a name="evs_04_2011_p19692132112253"></a><a name="evs_04_2011_p19692132112253"></a>挂载的时间信息。</p>
    <p id="evs_04_2011_p66401431193919"><a name="evs_04_2011_p66401431193919"></a><a name="evs_04_2011_p66401431193919"></a><span id="evs_04_2011_text1231921354419"><a name="evs_04_2011_text1231921354419"></a><a name="evs_04_2011_text1231921354419"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2011_row15954169111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p17219276111147"><a name="evs_04_2011_p17219276111147"></a><a name="evs_04_2011_p17219276111147"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p52584153111147"><a name="evs_04_2011_p52584153111147"></a><a name="evs_04_2011_p52584153111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p65069243111147"><a name="evs_04_2011_p65069243111147"></a><a name="evs_04_2011_p65069243111147"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row48752281111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p56620654111147"><a name="evs_04_2011_p56620654111147"></a><a name="evs_04_2011_p56620654111147"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p22870239111147"><a name="evs_04_2011_p22870239111147"></a><a name="evs_04_2011_p22870239111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p63332792111147"><a name="evs_04_2011_p63332792111147"></a><a name="evs_04_2011_p63332792111147"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row33124222111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p65816302111147"><a name="evs_04_2011_p65816302111147"></a><a name="evs_04_2011_p65816302111147"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p29520255111147"><a name="evs_04_2011_p29520255111147"></a><a name="evs_04_2011_p29520255111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p6214946111147"><a name="evs_04_2011_p6214946111147"></a><a name="evs_04_2011_p6214946111147"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_row55934521111147"><td class="cellrowborder" valign="top" width="19.27807219278072%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_p34402351111147"><a name="evs_04_2011_p34402351111147"></a><a name="evs_04_2011_p34402351111147"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.0975902409759%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_p35127017111147"><a name="evs_04_2011_p35127017111147"></a><a name="evs_04_2011_p35127017111147"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_p16521419111147"><a name="evs_04_2011_p16521419111147"></a><a name="evs_04_2011_p16521419111147"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2011_li29114110314"></a>metadata参数说明

    <a name="evs_04_2011_evs_04_3004_table3430728295554"></a>
    <table><thead align="left"><tr id="evs_04_2011_evs_04_3004_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2011_evs_04_3004_p8809200174410"><a name="evs_04_2011_evs_04_3004_p8809200174410"></a><a name="evs_04_2011_evs_04_3004_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_2011_evs_04_3004_p168135017449"><a name="evs_04_2011_evs_04_3004_p168135017449"></a><a name="evs_04_2011_evs_04_3004_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2011_evs_04_3004_p1282213034412"><a name="evs_04_2011_evs_04_3004_p1282213034412"></a><a name="evs_04_2011_evs_04_3004_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_evs_04_3004_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_3004_p1562408795622"><a name="evs_04_2011_evs_04_3004_p1562408795622"></a><a name="evs_04_2011_evs_04_3004_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_3004_p5759155095622"><a name="evs_04_2011_evs_04_3004_p5759155095622"></a><a name="evs_04_2011_evs_04_3004_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2011_evs_04_3004_p177192813501"><a name="evs_04_2011_evs_04_3004_p177192813501"></a><a name="evs_04_2011_evs_04_3004_p177192813501"></a>metadata中的表示加密功能的字段。<a name="evs_04_2011_evs_04_3004_ul141951225145011"></a><a name="evs_04_2011_evs_04_3004_ul141951225145011"></a><ul id="evs_04_2011_evs_04_3004_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2011_evs_04_3004_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_3004_p241272995622"><a name="evs_04_2011_evs_04_3004_p241272995622"></a><a name="evs_04_2011_evs_04_3004_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_3004_p6121338895622"><a name="evs_04_2011_evs_04_3004_p6121338895622"></a><a name="evs_04_2011_evs_04_3004_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_evs_04_3004_p4159804295622"><a name="evs_04_2011_evs_04_3004_p4159804295622"></a><a name="evs_04_2011_evs_04_3004_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_evs_04_3004_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_3004_p1478896104915"><a name="evs_04_2011_evs_04_3004_p1478896104915"></a><a name="evs_04_2011_evs_04_3004_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_3004_p52681767104915"><a name="evs_04_2011_evs_04_3004_p52681767104915"></a><a name="evs_04_2011_evs_04_3004_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2011_evs_04_3004_p17177177145116"><a name="evs_04_2011_evs_04_3004_p17177177145116"></a><a name="evs_04_2011_evs_04_3004_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="evs_04_2011_evs_04_3004_ul14462208141855"></a><a name="evs_04_2011_evs_04_3004_ul14462208141855"></a><ul id="evs_04_2011_evs_04_3004_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="evs_04_2011_evs_04_3004_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_3004_p3500156018292"><a name="evs_04_2011_evs_04_3004_p3500156018292"></a><a name="evs_04_2011_evs_04_3004_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_3004_p1655411118292"><a name="evs_04_2011_evs_04_3004_p1655411118292"></a><a name="evs_04_2011_evs_04_3004_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_evs_04_3004_p47931946183150"><a name="evs_04_2011_evs_04_3004_p47931946183150"></a><a name="evs_04_2011_evs_04_3004_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2011_li0419202382514"></a>error参数说明

    <a name="evs_04_2011_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2011_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2011_evs_04_2013_p19541716103019"><a name="evs_04_2011_evs_04_2013_p19541716103019"></a><a name="evs_04_2011_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2011_evs_04_2013_p39375186103019"><a name="evs_04_2011_evs_04_2013_p39375186103019"></a><a name="evs_04_2011_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2011_evs_04_2013_p38578950103019"><a name="evs_04_2011_evs_04_2013_p38578950103019"></a><a name="evs_04_2011_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2011_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_2013_p46815658103019"><a name="evs_04_2011_evs_04_2013_p46815658103019"></a><a name="evs_04_2011_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_2013_p33971979103019"><a name="evs_04_2011_evs_04_2013_p33971979103019"></a><a name="evs_04_2011_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_evs_04_2013_p21623243103019"><a name="evs_04_2011_evs_04_2013_p21623243103019"></a><a name="evs_04_2011_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2011_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2011_evs_04_2013_p59870541103019"><a name="evs_04_2011_evs_04_2013_p59870541103019"></a><a name="evs_04_2011_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2011_evs_04_2013_p17675690103019"><a name="evs_04_2011_evs_04_2013_p17675690103019"></a><a name="evs_04_2011_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2011_evs_04_2013_p6087468103019"><a name="evs_04_2011_evs_04_2013_p6087468103019"></a><a name="evs_04_2011_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2011_evs_04_2013_p54787218103019"><a name="evs_04_2011_evs_04_2013_p54787218103019"></a><a name="evs_04_2011_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "volume": {
            "attachments": [ ], 
            "links": [
                {
                    "href": "https://volume.az0.dc1.domainname.com/v2/40acc331ac784f34842ba4f08ff2be48/volumes/591ac654-26d8-41be-bb77-4f90699d2d41", 
                    "rel": "self"
                }, 
                {
                    "href": "https://volume.az0.dc1.domainname.com/40acc331ac784f34842ba4f08ff2be48/volumes/591ac654-26d8-41be-bb77-4f90699d2d41", 
                    "rel": "bookmark"
                }
            ], 
            "availability_zone": "az-dc-1", 
            "os-vol-host-attr:host": "az-dc-1#SSD", 
            "encrypted": false, 
            "multiattach": true, 
            "updated_at": "2016-02-03T02:19:29.895237", 
            "os-volume-replication:extended_status": null, 
            "replication_status": "disabled", 
            "snapshot_id": null, 
            "id": "591ac654-26d8-41be-bb77-4f90699d2d41", 
            "size": 40, 
            "user_id": "fd03ee73295e45478d88e15263d2ee4e", 
            "os-vol-tenant-attr:tenant_id": "40acc331ac784f34842ba4f08ff2be48", 
            "volume_image_metadata": null, 
            "os-vol-mig-status-attr:migstat": null, 
            "metadata": {}, 
            "tags": {
                "key1": "value1", 
                "key2": "value2"
            }, 
            "status": "available", 
            "description": "auto-created_from_restore_from_backup",  
            "source_volid": null, 
            "consistencygroup_id": null, 
            "os-vol-mig-status-attr:name_id": null, 
            "name": "restore_backup_0115efb3-678c-4a9e-bff6-d3cd278238b9", 
            "bootable": "false", 
            "created_at": "2016-02-03T02:19:11.723797", 
            "volume_type": null, 
            "service_type": "EVS", 
            "dedicated_storage_id": null, 
            "dedicated_storage_name": null, 
            "wwn": " 688860300000d136fa16f48f05992360"
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

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错为：

    ```
    {
        "badrequest": {
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

