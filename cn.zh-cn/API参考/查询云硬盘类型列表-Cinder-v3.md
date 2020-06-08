# 查询云硬盘类型列表<a name="evs_04_3035"></a>

## 功能介绍<a name="section18389930"></a>

查询支持的云硬盘类型。

## URI<a name="section31291646"></a>

-   URI格式

    GET /v3/\{project\_id\}/types

-   参数说明

    <a name="table57434139"></a>
    <table><thead align="left"><tr id="row461342"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p37368736"><a name="p37368736"></a><a name="p37368736"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p6968762"><a name="p6968762"></a><a name="p6968762"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p27598869"><a name="p27598869"></a><a name="p27598869"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20915929"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p16468652"><a name="p16468652"></a><a name="p16468652"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p58892473"><a name="p58892473"></a><a name="p58892473"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p5560998"><a name="p5560998"></a><a name="p5560998"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section13189358"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v3/{project_id}/types
    ```


## 响应消息<a name="section51595365"></a>

-   响应参数

    <a name="evs_04_2071_table157189144113"></a>
    <table><thead align="left"><tr id="evs_04_2071_row37118915416"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="evs_04_2071_p671295419"><a name="evs_04_2071_p671295419"></a><a name="evs_04_2071_p671295419"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2071_p47159114117"><a name="evs_04_2071_p47159114117"></a><a name="evs_04_2071_p47159114117"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2071_p1671199174116"><a name="evs_04_2071_p1671199174116"></a><a name="evs_04_2071_p1671199174116"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2071_row177120964114"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p14711298413"><a name="evs_04_2071_p14711298413"></a><a name="evs_04_2071_p14711298413"></a>volume_types</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p971892416"><a name="evs_04_2071_p971892416"></a><a name="evs_04_2071_p971892416"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p157117910419"><a name="evs_04_2071_p157117910419"></a><a name="evs_04_2071_p157117910419"></a>查询请求返回的云硬盘类型列表，请参见<a href="#evs_04_2071_li61994451201537">•volume_types参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row971797416"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p129522216412"><a name="evs_04_2071_p129522216412"></a><a name="evs_04_2071_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p1595262111415"><a name="evs_04_2071_p1595262111415"></a><a name="evs_04_2071_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p109527215417"><a name="evs_04_2071_p109527215417"></a><a name="evs_04_2071_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2071_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2071_li61994451201537"></a>volume\_types参数说明

    <a name="evs_04_2071_table5015685217931"></a>
    <table><thead align="left"><tr id="evs_04_2071_row3525603317931"><th class="cellrowborder" valign="top" width="21.45%" id="mcps1.1.4.1.1"><p id="evs_04_2071_p3716642517931"><a name="evs_04_2071_p3716642517931"></a><a name="evs_04_2071_p3716642517931"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.41%" id="mcps1.1.4.1.2"><p id="evs_04_2071_p459600531514"><a name="evs_04_2071_p459600531514"></a><a name="evs_04_2071_p459600531514"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2071_p4241583117931"><a name="evs_04_2071_p4241583117931"></a><a name="evs_04_2071_p4241583117931"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2071_row1313028517931"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p5692013517931"><a name="evs_04_2071_p5692013517931"></a><a name="evs_04_2071_p5692013517931"></a>extra_specs</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p317768361514"><a name="evs_04_2071_p317768361514"></a><a name="evs_04_2071_p317768361514"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p5928829717931"><a name="evs_04_2071_p5928829717931"></a><a name="evs_04_2071_p5928829717931"></a>云硬盘类型的规格，请参见<a href="#evs_04_2071_li963595619529">•extra_specs参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row6655870217931"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p2254579917931"><a name="evs_04_2071_p2254579917931"></a><a name="evs_04_2071_p2254579917931"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p378706671514"><a name="evs_04_2071_p378706671514"></a><a name="evs_04_2071_p378706671514"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p1505171317931"><a name="evs_04_2071_p1505171317931"></a><a name="evs_04_2071_p1505171317931"></a>云硬盘类型名称。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row124769217931"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p3395425317931"><a name="evs_04_2071_p3395425317931"></a><a name="evs_04_2071_p3395425317931"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p476251801514"><a name="evs_04_2071_p476251801514"></a><a name="evs_04_2071_p476251801514"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p3954068517931"><a name="evs_04_2071_p3954068517931"></a><a name="evs_04_2071_p3954068517931"></a>云硬盘类型的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row17240824161631"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p54329535161631"><a name="evs_04_2071_p54329535161631"></a><a name="evs_04_2071_p54329535161631"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p38616177161631"><a name="evs_04_2071_p38616177161631"></a><a name="evs_04_2071_p38616177161631"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p24780220161631"><a name="evs_04_2071_p24780220161631"></a><a name="evs_04_2071_p24780220161631"></a>云硬盘类型的描述信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row1027115162029"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p16087523162029"><a name="evs_04_2071_p16087523162029"></a><a name="evs_04_2071_p16087523162029"></a>qos_specs_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p28020971162029"><a name="evs_04_2071_p28020971162029"></a><a name="evs_04_2071_p28020971162029"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p34413580162029"><a name="evs_04_2071_p34413580162029"></a><a name="evs_04_2071_p34413580162029"></a><span id="evs_04_2071_text3111131184916"><a name="evs_04_2071_text3111131184916"></a><a name="evs_04_2071_text3111131184916"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row12948331162139"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p42181927162139"><a name="evs_04_2071_p42181927162139"></a><a name="evs_04_2071_p42181927162139"></a>is_public</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p61292894162139"><a name="evs_04_2071_p61292894162139"></a><a name="evs_04_2071_p61292894162139"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p26369379162139"><a name="evs_04_2071_p26369379162139"></a><a name="evs_04_2071_p26369379162139"></a><span id="evs_04_2071_text10706161911492"><a name="evs_04_2071_text10706161911492"></a><a name="evs_04_2071_text10706161911492"></a>预留属性。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2071_li963595619529"></a>extra\_specs参数说明

    <a name="evs_04_2071_table1763545695210"></a>
    <table><thead align="left"><tr id="evs_04_2071_row16361656165213"><th class="cellrowborder" valign="top" width="21.45%" id="mcps1.1.4.1.1"><p id="evs_04_2071_p1763619566527"><a name="evs_04_2071_p1763619566527"></a><a name="evs_04_2071_p1763619566527"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.41%" id="mcps1.1.4.1.2"><p id="evs_04_2071_p18636105619529"><a name="evs_04_2071_p18636105619529"></a><a name="evs_04_2071_p18636105619529"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2071_p186361556155214"><a name="evs_04_2071_p186361556155214"></a><a name="evs_04_2071_p186361556155214"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2071_row56365565526"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p063625610529"><a name="evs_04_2071_p063625610529"></a><a name="evs_04_2071_p063625610529"></a>volume_backend_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p3636165635219"><a name="evs_04_2071_p3636165635219"></a><a name="evs_04_2071_p3636165635219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p17636185614527"><a name="evs_04_2071_p17636185614527"></a><a name="evs_04_2071_p17636185614527"></a><span id="evs_04_2071_text205233101097"><a name="evs_04_2071_text205233101097"></a><a name="evs_04_2071_text205233101097"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row156362568523"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p863675695214"><a name="evs_04_2071_p863675695214"></a><a name="evs_04_2071_p863675695214"></a>availability-zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p8636175665214"><a name="evs_04_2071_p8636175665214"></a><a name="evs_04_2071_p8636175665214"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p18636356185213"><a name="evs_04_2071_p18636356185213"></a><a name="evs_04_2071_p18636356185213"></a><span id="evs_04_2071_text533914121390"><a name="evs_04_2071_text533914121390"></a><a name="evs_04_2071_text533914121390"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row17844276596"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p178418274593"><a name="evs_04_2071_p178418274593"></a><a name="evs_04_2071_p178418274593"></a>HW:availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p168416276599"><a name="evs_04_2071_p168416276599"></a><a name="evs_04_2071_p168416276599"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p1540410211408"><a name="evs_04_2071_p1540410211408"></a><a name="evs_04_2071_p1540410211408"></a><span id="evs_04_2071_evs_04_2071_text533914121390"><a name="evs_04_2071_evs_04_2071_text533914121390"></a><a name="evs_04_2071_evs_04_2071_text533914121390"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row3637135611527"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p163710561529"><a name="evs_04_2071_p163710561529"></a><a name="evs_04_2071_p163710561529"></a>RESKEY:availability_zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p166374562525"><a name="evs_04_2071_p166374562525"></a><a name="evs_04_2071_p166374562525"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p3637756205214"><a name="evs_04_2071_p3637756205214"></a><a name="evs_04_2071_p3637756205214"></a>支持当前云硬盘类型的AZ列表。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row16371656175219"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p1363716565526"><a name="evs_04_2071_p1363716565526"></a><a name="evs_04_2071_p1363716565526"></a>os-vendor-extended:sold_out_availability_zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p0637456155216"><a name="evs_04_2071_p0637456155216"></a><a name="evs_04_2071_p0637456155216"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p1063725695214"><a name="evs_04_2071_p1063725695214"></a><a name="evs_04_2071_p1063725695214"></a>当前云硬盘类型售罄的AZ列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2071_li0419202382514"></a>error参数说明

    <a name="evs_04_2071_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2071_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2071_evs_04_2013_p19541716103019"><a name="evs_04_2071_evs_04_2013_p19541716103019"></a><a name="evs_04_2071_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2071_evs_04_2013_p39375186103019"><a name="evs_04_2071_evs_04_2013_p39375186103019"></a><a name="evs_04_2071_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2071_evs_04_2013_p38578950103019"><a name="evs_04_2071_evs_04_2013_p38578950103019"></a><a name="evs_04_2071_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2071_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_evs_04_2013_p46815658103019"><a name="evs_04_2071_evs_04_2013_p46815658103019"></a><a name="evs_04_2071_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_evs_04_2013_p33971979103019"><a name="evs_04_2071_evs_04_2013_p33971979103019"></a><a name="evs_04_2071_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_evs_04_2013_p21623243103019"><a name="evs_04_2071_evs_04_2013_p21623243103019"></a><a name="evs_04_2071_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_evs_04_2013_p59870541103019"><a name="evs_04_2071_evs_04_2013_p59870541103019"></a><a name="evs_04_2071_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_evs_04_2013_p17675690103019"><a name="evs_04_2071_evs_04_2013_p17675690103019"></a><a name="evs_04_2071_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_evs_04_2013_p6087468103019"><a name="evs_04_2071_evs_04_2013_p6087468103019"></a><a name="evs_04_2071_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2071_evs_04_2013_p54787218103019"><a name="evs_04_2071_evs_04_2013_p54787218103019"></a><a name="evs_04_2071_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    { 
        "volume_types": [ 
            { 
                "extra_specs": { 
                    "volume_backend_name": "SAS",  
                    "availability-zone": "az-dc-1",  
                    "RESKEY:availability_zones": "az-dc-1,az-dc-2",  
                    "os-vendor-extended:sold_out_availability_zones": "az-dc-2" 
                },  
                "name": "SAS",  
                "qos_specs_id": null,  
                "id": "6c81c680-df58-4512-81e7-ecf66d160638",  
                "is_public": true,  
                "description": null 
            },  
            { 
                "extra_specs": { 
                    "volume_backend_name": "SATA",  
                    "availability-zone": "az-dc-1",  
                    "RESKEY:availability_zones": "az-dc-1,az-dc-2",  
                    "os-vendor-extended:sold_out_availability_zones": "az-dc-2"  
                },  
                "name": "SATA",  
                "qos_specs_id": "585f29d6-7147-42e7-bfb8-ca214f640f6f",  
                "is_public": true,  
                "id": "ea6e3c13-aac5-46e0-b280-745ed272e662",  
                "description": null 
            },  
            { 
                "extra_specs": { 
                    "volume_backend_name": "SSD",  
                    "availability-zone": "az-dc-1",  
                    "RESKEY:availability_zones": "az-dc-1,az-dc-2",  
                    "os-vendor-extended:sold_out_availability_zones": "az-dc-2"
                },  
                "name": "SSD",  
                "qos_specs_id": "39b0c29a-308b-4f86-b478-5d3d02a43837",  
                "is_public": true,  
                "id": "6f2dee9e-82f0-4be3-ad89-bae605a3d24f",  
                "description": null 
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
        "badrequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section61705107"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

