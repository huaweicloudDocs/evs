# 查询租户的详细配额<a name="evs_04_2073"></a>

## 功能介绍<a name="section9502070"></a>

查询租户的详细配额。

## 调试<a name="section765963762516"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EVS&api=CinderListQuotas)中直接运行调试该接口。

## URI<a name="section18409771"></a>

-   URI格式

    GET /v2/\{project\_id\}/os-quota-sets/\{target\_project\_id\}?usage=True

-   参数说明

    <a name="table117163"></a>
    <table><thead align="left"><tr id="row55762700"><th class="cellrowborder" valign="top" width="33.33%" id="mcps1.1.4.1.1"><p id="p20484818"><a name="p20484818"></a><a name="p20484818"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.3%" id="mcps1.1.4.1.2"><p id="p48657561"><a name="p48657561"></a><a name="p48657561"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.370000000000005%" id="mcps1.1.4.1.3"><p id="p48948360"><a name="p48948360"></a><a name="p48948360"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5394248"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p34280961"><a name="p34280961"></a><a name="p34280961"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.3%" headers="mcps1.1.4.1.2 "><p id="p25294426"><a name="p25294426"></a><a name="p25294426"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.370000000000005%" headers="mcps1.1.4.1.3 "><p id="p35582587"><a name="p35582587"></a><a name="p35582587"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row1630212817190"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p730312861919"><a name="p730312861919"></a><a name="p730312861919"></a>target_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.3%" headers="mcps1.1.4.1.2 "><p id="p20303188151911"><a name="p20303188151911"></a><a name="p20303188151911"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.370000000000005%" headers="mcps1.1.4.1.3 "><p id="p33032891913"><a name="p33032891913"></a><a name="p33032891913"></a>目标的项目ID。与project_id保持一致即可。</p>
    </td>
    </tr>
    <tr id="row12711612181914"><td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.1 "><p id="p10271101212194"><a name="p10271101212194"></a><a name="p10271101212194"></a>usage</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.3%" headers="mcps1.1.4.1.2 "><p id="p727112128195"><a name="p727112128195"></a><a name="p727112128195"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.370000000000005%" headers="mcps1.1.4.1.3 "><p id="p112714121195"><a name="p112714121195"></a><a name="p112714121195"></a>是否查询配额详细信息。当前只支持传true。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section31470215"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v2/{project_id}/os-quota-sets/{project_id}?usage=True
    ```


## 响应消息<a name="section14796483"></a>

-   响应参数

    <a name="table13993131410556"></a>
    <table><thead align="left"><tr id="row799321420553"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="p099351495511"><a name="p099351495511"></a><a name="p099351495511"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="p5993141425516"><a name="p5993141425516"></a><a name="p5993141425516"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p17993414135514"><a name="p17993414135514"></a><a name="p17993414135514"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row209931814185513"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p119941014125514"><a name="p119941014125514"></a><a name="p119941014125514"></a>quota_set</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p14994514165520"><a name="p14994514165520"></a><a name="p14994514165520"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1099416145558"><a name="p1099416145558"></a><a name="p1099416145558"></a>查询请求返回的配额信息，请参见<a href="#li4741865201620">•quota_set参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row3451722569"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li4741865201620"></a>quota\_set参数说明

    <a name="table42676787201620"></a>
    <table><thead align="left"><tr id="row15715964201620"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="p65033611201620"><a name="p65033611201620"></a><a name="p65033611201620"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="p5090379315311"><a name="p5090379315311"></a><a name="p5090379315311"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p1989612244512"><a name="p1989612244512"></a><a name="p1989612244512"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row60124619201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p38255980201620"><a name="p38255980201620"></a><a name="p38255980201620"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p2956653915311"><a name="p2956653915311"></a><a name="p2956653915311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p10336815201620"><a name="p10336815201620"></a><a name="p10336815201620"></a>云硬盘数量，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row25922478201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p19345972201620"><a name="p19345972201620"></a><a name="p19345972201620"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p4607944115311"><a name="p4607944115311"></a><a name="p4607944115311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p26061300201620"><a name="p26061300201620"></a><a name="p26061300201620"></a>快照数量，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row33225116201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p6879872201620"><a name="p6879872201620"></a><a name="p6879872201620"></a>gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p4144727715311"><a name="p4144727715311"></a><a name="p4144727715311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p41689235201620"><a name="p41689235201620"></a><a name="p41689235201620"></a>总大小（快照+云硬盘），单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row39658796201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p58245913201620"><a name="p58245913201620"></a><a name="p58245913201620"></a>volumes_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p178624415311"><a name="p178624415311"></a><a name="p178624415311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p33568305201620"><a name="p33568305201620"></a><a name="p33568305201620"></a>SSD类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row4389102316598"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p899932855916"><a name="p899932855916"></a><a name="p899932855916"></a>volumes_GPSSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p2999182815912"><a name="p2999182815912"></a><a name="p2999182815912"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p5999132845914"><a name="p5999132845914"></a><a name="p5999132845914"></a>GPSSD类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row158911913505"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p1849815075218"><a name="p1849815075218"></a><a name="p1849815075218"></a>volumes_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p249817065214"><a name="p249817065214"></a><a name="p249817065214"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p849819015526"><a name="p849819015526"></a><a name="p849819015526"></a>SAS类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row33679293201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p6988929729"><a name="p6988929729"></a><a name="p6988929729"></a>snapshots_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p1046809615311"><a name="p1046809615311"></a><a name="p1046809615311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p19567167201620"><a name="p19567167201620"></a><a name="p19567167201620"></a>SSD类型云硬盘预留快照个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row12629195618592"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p19405201109"><a name="p19405201109"></a><a name="p19405201109"></a>snapshots_GPSSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p154058119018"><a name="p154058119018"></a><a name="p154058119018"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p34055115019"><a name="p34055115019"></a><a name="p34055115019"></a>GPSSD类型云硬盘预留快照个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row775510173509"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p1820015264531"><a name="p1820015264531"></a><a name="p1820015264531"></a>snapshots_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p10200132615539"><a name="p10200132615539"></a><a name="p10200132615539"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p22001126175315"><a name="p22001126175315"></a><a name="p22001126175315"></a>SAS类型云硬盘预留快照个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row41886775201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p932213524218"><a name="p932213524218"></a><a name="p932213524218"></a>gigabytes_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p4260948115311"><a name="p4260948115311"></a><a name="p4260948115311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p3943730201620"><a name="p3943730201620"></a><a name="p3943730201620"></a>SSD类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row1050517334011"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p179611135601"><a name="p179611135601"></a><a name="p179611135601"></a>gigabytes_GPSSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p896113515020"><a name="p896113515020"></a><a name="p896113515020"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1996114351606"><a name="p1996114351606"></a><a name="p1996114351606"></a>GPSSD类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row1086118284505"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p344652745413"><a name="p344652745413"></a><a name="p344652745413"></a>gigabytes_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p544602713542"><a name="p544602713542"></a><a name="p544602713542"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1544632717540"><a name="p1544632717540"></a><a name="p1544632717540"></a>SAS类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row35493575201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p56407339201620"><a name="p56407339201620"></a><a name="p56407339201620"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p2881594215311"><a name="p2881594215311"></a><a name="p2881594215311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p50275403201620"><a name="p50275403201620"></a><a name="p50275403201620"></a>租户ID。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="row49825446201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p9329306201620"><a name="p9329306201620"></a><a name="p9329306201620"></a>backups</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p5238998415311"><a name="p5238998415311"></a><a name="p5238998415311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p6295376201620"><a name="p6295376201620"></a><a name="p6295376201620"></a>备份个数，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row56658385201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p25926512201620"><a name="p25926512201620"></a><a name="p25926512201620"></a>backup_gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p1573030215311"><a name="p1573030215311"></a><a name="p1573030215311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p49989712201620"><a name="p49989712201620"></a><a name="p49989712201620"></a>备份大小，单位为GB，键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="row1569318421316"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p4969152818"><a name="p4969152818"></a><a name="p4969152818"></a>per_volume_gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="p19697521415"><a name="p19697521415"></a><a name="p19697521415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p11969135217118"><a name="p11969135217118"></a><a name="p11969135217118"></a>每个云硬盘的容量配额限制。键值对，包含：reserved（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：** 
    >如果返回值中limit为-1，表示没有限制配额。

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
        "quota_set": {
            "gigabytes_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 21
            }, 
            "volumes_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 8
            }, 
            "gigabytes": {
                "reserved": 0, 
                "limit": 42790, 
                "in_use": 2792
            }, 
            "backup_gigabytes": {
                "reserved": 0, 
                "limit": 5120, 
                "in_use": 51
            }, 
            "snapshots_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 28
            }, 
            "snapshots": {
                "reserved": 0, 
                "limit": 10, 
                "in_use": 6
            }, 
            "id": "cd631140887d4b6e9c786b67a6dd4c02", 
            "volumes_SAS": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 2
            }, 
            "snapshots_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 108
            }, 
            "gigabytes_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 168
            }, 
            "backups": {
                "reserved": 0, 
                "limit": 100, 
                "in_use": 10
            }, 
            "gigabytes_SSD": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 1085
            }, 
            "snapshots_SATA": {
                "reserved": 0, 
                "limit": -1, 
                "in_use": 0
            }
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


## 状态码<a name="section66059488"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

