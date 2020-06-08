# 添加云硬盘的元数据<a name="evs_04_2074"></a>

## 功能介绍<a name="section60214390"></a>

添加或更新云硬盘的元数据。

## URI<a name="section5058598"></a>

-   URI格式

    POST /v2/\{project\_id\}/volumes/\{volume\_id\}/metadata

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
    <tr id="row11170003"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p32355065"><a name="p32355065"></a><a name="p32355065"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p3514615"><a name="p3514615"></a><a name="p3514615"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p16248438"><a name="p16248438"></a><a name="p16248438"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

-   请求参数

    <a name="table31588048"></a>
    <table><thead align="left"><tr id="row57330849"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="p13287175"><a name="p13287175"></a><a name="p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="p2519427"><a name="p2519427"></a><a name="p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="p2747002"><a name="p2747002"></a><a name="p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="p21180630"><a name="p21180630"></a><a name="p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row53167494153413"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="p11599783153413"><a name="p11599783153413"></a><a name="p11599783153413"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p58405153413"><a name="p58405153413"></a><a name="p58405153413"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="p4730855153413"><a name="p4730855153413"></a><a name="p4730855153413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p203071547124818"><a name="p203071547124818"></a><a name="p203071547124818"></a>需要更新的元数据信息，请参见<a href="#li54973602211845">•metadata参数说明</a>。</p>
    <p id="p47654998153413"><a name="p47654998153413"></a><a name="p47654998153413"></a><span id="text17527183012510"><a name="text17527183012510"></a><a name="text17527183012510"></a>metadata中的key和value长度不大于255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li54973602211845"></a>metadata参数说明

    <a name="table32717123212358"></a>
    <table><thead align="left"><tr id="row2280240212358"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="p50481723212358"><a name="p50481723212358"></a><a name="p50481723212358"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.2"><p id="p62487767212358"><a name="p62487767212358"></a><a name="p62487767212358"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p28344363212358"><a name="p28344363212358"></a><a name="p28344363212358"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.524752475247524%" id="mcps1.1.5.1.4"><p id="p14192096212358"><a name="p14192096212358"></a><a name="p14192096212358"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row8709150212358"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p34352524212358"><a name="p34352524212358"></a><a name="p34352524212358"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p31091026212358"><a name="p31091026212358"></a><a name="p31091026212358"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p35345177212358"><a name="p35345177212358"></a><a name="p35345177212358"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.1.5.1.4 "><p id="p44387080212358"><a name="p44387080212358"></a><a name="p44387080212358"></a>一个或多个键值对形式的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "metadata": {
            "key1": "value1", 
            "key2": "value2"
        }
    }
    ```


## 响应消息<a name="section7093323"></a>

-   响应参数

    <a name="table11977025201856"></a>
    <table><thead align="left"><tr id="row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p11709178184818"><a name="p11709178184818"></a><a name="p11709178184818"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p67131989483"><a name="p67131989483"></a><a name="p67131989483"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p87153824811"><a name="p87153824811"></a><a name="p87153824811"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p16378828201856"><a name="p16378828201856"></a><a name="p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p6490369115541"><a name="p6490369115541"></a><a name="p6490369115541"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p20205612201856"><a name="p20205612201856"></a><a name="p20205612201856"></a>键值对，云硬盘的元数据信息。</p>
    </td>
    </tr>
    <tr id="row11511747165814"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
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
        "metadata": {
            "key1": "value1", 
            "key2": "value2"
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

