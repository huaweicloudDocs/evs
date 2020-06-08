# 查询租户的详细配额<a name="evs_04_3037"></a>

## 功能介绍<a name="section9502070"></a>

查询租户的详细配额。

## URI<a name="section18409771"></a>

-   URI格式

    GET /v3/\{project\_id\}/os-quota-sets/\{project\_id\}?usage=True

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
    </tbody>
    </table>


## 请求消息<a name="section31470215"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v3/{project_id}/os-quota-sets/{project_id}?usage=True
    ```


## 响应消息<a name="section14796483"></a>

-   响应参数

    <a name="evs_04_2073_table13993131410556"></a>
    <table><thead align="left"><tr id="evs_04_2073_row799321420553"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2073_p099351495511"><a name="evs_04_2073_p099351495511"></a><a name="evs_04_2073_p099351495511"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_2073_p5993141425516"><a name="evs_04_2073_p5993141425516"></a><a name="evs_04_2073_p5993141425516"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2073_p17993414135514"><a name="evs_04_2073_p17993414135514"></a><a name="evs_04_2073_p17993414135514"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2073_row209931814185513"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p119941014125514"><a name="evs_04_2073_p119941014125514"></a><a name="evs_04_2073_p119941014125514"></a>quota_set</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p14994514165520"><a name="evs_04_2073_p14994514165520"></a><a name="evs_04_2073_p14994514165520"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p1099416145558"><a name="evs_04_2073_p1099416145558"></a><a name="evs_04_2073_p1099416145558"></a>查询请求返回的配额信息，请参见<a href="#evs_04_2073_li4741865201620">•quota_set参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row3451722569"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p129522216412"><a name="evs_04_2073_p129522216412"></a><a name="evs_04_2073_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p1595262111415"><a name="evs_04_2073_p1595262111415"></a><a name="evs_04_2073_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p109527215417"><a name="evs_04_2073_p109527215417"></a><a name="evs_04_2073_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2073_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2073_li4741865201620"></a>quota\_set参数说明

    <a name="evs_04_2073_table42676787201620"></a>
    <table><thead align="left"><tr id="evs_04_2073_row15715964201620"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="evs_04_2073_p65033611201620"><a name="evs_04_2073_p65033611201620"></a><a name="evs_04_2073_p65033611201620"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="evs_04_2073_p5090379315311"><a name="evs_04_2073_p5090379315311"></a><a name="evs_04_2073_p5090379315311"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2073_p1989612244512"><a name="evs_04_2073_p1989612244512"></a><a name="evs_04_2073_p1989612244512"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2073_row60124619201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p38255980201620"><a name="evs_04_2073_p38255980201620"></a><a name="evs_04_2073_p38255980201620"></a>volumes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p2956653915311"><a name="evs_04_2073_p2956653915311"></a><a name="evs_04_2073_p2956653915311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p10336815201620"><a name="evs_04_2073_p10336815201620"></a><a name="evs_04_2073_p10336815201620"></a>云硬盘数量，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row25922478201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p19345972201620"><a name="evs_04_2073_p19345972201620"></a><a name="evs_04_2073_p19345972201620"></a>snapshots</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p4607944115311"><a name="evs_04_2073_p4607944115311"></a><a name="evs_04_2073_p4607944115311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p26061300201620"><a name="evs_04_2073_p26061300201620"></a><a name="evs_04_2073_p26061300201620"></a>快照数量，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row33225116201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p6879872201620"><a name="evs_04_2073_p6879872201620"></a><a name="evs_04_2073_p6879872201620"></a>gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p4144727715311"><a name="evs_04_2073_p4144727715311"></a><a name="evs_04_2073_p4144727715311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p41689235201620"><a name="evs_04_2073_p41689235201620"></a><a name="evs_04_2073_p41689235201620"></a>总大小（快照+云硬盘），单位为GB，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row39658796201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p58245913201620"><a name="evs_04_2073_p58245913201620"></a><a name="evs_04_2073_p58245913201620"></a>volume_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p178624415311"><a name="evs_04_2073_p178624415311"></a><a name="evs_04_2073_p178624415311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p33568305201620"><a name="evs_04_2073_p33568305201620"></a><a name="evs_04_2073_p33568305201620"></a>SSD类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row158911913505"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p1849815075218"><a name="evs_04_2073_p1849815075218"></a><a name="evs_04_2073_p1849815075218"></a>volume_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p249817065214"><a name="evs_04_2073_p249817065214"></a><a name="evs_04_2073_p249817065214"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p849819015526"><a name="evs_04_2073_p849819015526"></a><a name="evs_04_2073_p849819015526"></a>SAS类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row13803613155014"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p7801730165210"><a name="evs_04_2073_p7801730165210"></a><a name="evs_04_2073_p7801730165210"></a>volume_SATA</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p168012306521"><a name="evs_04_2073_p168012306521"></a><a name="evs_04_2073_p168012306521"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p1280119305522"><a name="evs_04_2073_p1280119305522"></a><a name="evs_04_2073_p1280119305522"></a>SATA类型云硬盘预留的云硬盘个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row33679293201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p6988929729"><a name="evs_04_2073_p6988929729"></a><a name="evs_04_2073_p6988929729"></a>snapshots_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p1046809615311"><a name="evs_04_2073_p1046809615311"></a><a name="evs_04_2073_p1046809615311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p19567167201620"><a name="evs_04_2073_p19567167201620"></a><a name="evs_04_2073_p19567167201620"></a>SSD类型云硬盘预留快照个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row775510173509"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p1820015264531"><a name="evs_04_2073_p1820015264531"></a><a name="evs_04_2073_p1820015264531"></a>snapshots_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p10200132615539"><a name="evs_04_2073_p10200132615539"></a><a name="evs_04_2073_p10200132615539"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p22001126175315"><a name="evs_04_2073_p22001126175315"></a><a name="evs_04_2073_p22001126175315"></a>SAS类型云硬盘预留快照个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row12575621105012"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p109062273533"><a name="evs_04_2073_p109062273533"></a><a name="evs_04_2073_p109062273533"></a>snapshots_SATA</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p199061427105317"><a name="evs_04_2073_p199061427105317"></a><a name="evs_04_2073_p199061427105317"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p129066272538"><a name="evs_04_2073_p129066272538"></a><a name="evs_04_2073_p129066272538"></a>SATA类型云硬盘预留快照个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row41886775201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p932213524218"><a name="evs_04_2073_p932213524218"></a><a name="evs_04_2073_p932213524218"></a>gigabytes_SSD</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p4260948115311"><a name="evs_04_2073_p4260948115311"></a><a name="evs_04_2073_p4260948115311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p3943730201620"><a name="evs_04_2073_p3943730201620"></a><a name="evs_04_2073_p3943730201620"></a>SSD类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row1086118284505"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p344652745413"><a name="evs_04_2073_p344652745413"></a><a name="evs_04_2073_p344652745413"></a>gigabytes_SAS</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p544602713542"><a name="evs_04_2073_p544602713542"></a><a name="evs_04_2073_p544602713542"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p1544632717540"><a name="evs_04_2073_p1544632717540"></a><a name="evs_04_2073_p1544632717540"></a>SAS类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row1314725125019"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p047629135419"><a name="evs_04_2073_p047629135419"></a><a name="evs_04_2073_p047629135419"></a>gigabytes_SATA</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p1447102917543"><a name="evs_04_2073_p1447102917543"></a><a name="evs_04_2073_p1447102917543"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p94710297546"><a name="evs_04_2073_p94710297546"></a><a name="evs_04_2073_p94710297546"></a>SATA类型云硬盘预留的size大小，单位为GB，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row35493575201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p56407339201620"><a name="evs_04_2073_p56407339201620"></a><a name="evs_04_2073_p56407339201620"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p2881594215311"><a name="evs_04_2073_p2881594215311"></a><a name="evs_04_2073_p2881594215311"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p50275403201620"><a name="evs_04_2073_p50275403201620"></a><a name="evs_04_2073_p50275403201620"></a>租户ID。<span id="evs_04_2073_text19941457165313"><a name="evs_04_2073_text19941457165313"></a><a name="evs_04_2073_text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2073_row49825446201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p9329306201620"><a name="evs_04_2073_p9329306201620"></a><a name="evs_04_2073_p9329306201620"></a>backups</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p5238998415311"><a name="evs_04_2073_p5238998415311"></a><a name="evs_04_2073_p5238998415311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p6295376201620"><a name="evs_04_2073_p6295376201620"></a><a name="evs_04_2073_p6295376201620"></a>备份个数，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_row56658385201620"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_p25926512201620"><a name="evs_04_2073_p25926512201620"></a><a name="evs_04_2073_p25926512201620"></a>backup_gigabytes</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_p1573030215311"><a name="evs_04_2073_p1573030215311"></a><a name="evs_04_2073_p1573030215311"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_p49989712201620"><a name="evs_04_2073_p49989712201620"></a><a name="evs_04_2073_p49989712201620"></a>备份大小，单位为GB，键值对，包含：reserved（预留）、allocated（预留）、limit（最大）和in_use（已使用）。</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](public_sys-resources/icon-note.gif) **说明：**   
    >如果返回值中limit为-1，表示没有限制配额。  

-   <a name="evs_04_2073_li0419202382514"></a>error参数说明

    <a name="evs_04_2073_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2073_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2073_evs_04_2013_p19541716103019"><a name="evs_04_2073_evs_04_2013_p19541716103019"></a><a name="evs_04_2073_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2073_evs_04_2013_p39375186103019"><a name="evs_04_2073_evs_04_2013_p39375186103019"></a><a name="evs_04_2073_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2073_evs_04_2013_p38578950103019"><a name="evs_04_2073_evs_04_2013_p38578950103019"></a><a name="evs_04_2073_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2073_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_evs_04_2013_p46815658103019"><a name="evs_04_2073_evs_04_2013_p46815658103019"></a><a name="evs_04_2073_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_evs_04_2013_p33971979103019"><a name="evs_04_2073_evs_04_2013_p33971979103019"></a><a name="evs_04_2073_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_evs_04_2013_p21623243103019"><a name="evs_04_2073_evs_04_2013_p21623243103019"></a><a name="evs_04_2073_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2073_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2073_evs_04_2013_p59870541103019"><a name="evs_04_2073_evs_04_2013_p59870541103019"></a><a name="evs_04_2073_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2073_evs_04_2013_p17675690103019"><a name="evs_04_2073_evs_04_2013_p17675690103019"></a><a name="evs_04_2073_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2073_evs_04_2013_p6087468103019"><a name="evs_04_2073_evs_04_2013_p6087468103019"></a><a name="evs_04_2073_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2073_evs_04_2013_p54787218103019"><a name="evs_04_2073_evs_04_2013_p54787218103019"></a><a name="evs_04_2073_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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
                "allocated":0,
                "limit": -1, 
                "in_use": 21
            }, 
            "volumes_SATA": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 8
            }, 
            "gigabytes": {
                "reserved": 0, 
                "allocated":0,
                "limit": 42790, 
                "in_use": 2792
            }, 
            "backup_gigabytes": {
                "reserved": 0,
                "allocated":0, 
                "limit": 5120, 
                "in_use": 51
            }, 
            "snapshots_SAS": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes_SSD": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 28
            }, 
            "snapshots": {
                "reserved": 0, 
                "allocated":0,
                "limit": 10, 
                "in_use": 6
            }, 
            "id": "cd631140887d4b6e9c786b67a6dd4c02", 
            "volumes_SAS": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 2
            }, 
            "snapshots_SSD": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 0
            }, 
            "volumes": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 108
            }, 
            "gigabytes_SATA": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 168
            }, 
            "backups": {
                "reserved": 0, 
                "allocated":0,
                "limit": 100, 
                "in_use": 10
            }, 
            "gigabytes_SSD": {
                "reserved": 0, 
                "allocated":0,
                "limit": -1, 
                "in_use": 1085
            }, 
            "snapshots_SATA": {
                "reserved": 0, 
                "allocated":0,
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

请参考[错误码说明](错误码说明.md)。

