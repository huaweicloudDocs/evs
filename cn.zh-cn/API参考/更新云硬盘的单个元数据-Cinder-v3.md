# 更新云硬盘的单个元数据<a name="evs_04_3042"></a>

## 功能介绍<a name="section19390540"></a>

更新云硬盘的单个元数据。

## URI<a name="section40297137"></a>

-   URI格式

    PUT /v3/\{project\_id\}/volumes/\{volume\_id\}/metadata/\{key\}

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="28.92%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.07%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="28.92%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="28.92%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row3599748213115"><td class="cellrowborder" valign="top" width="28.92%" headers="mcps1.1.4.1.1 "><p id="p23144139213115"><a name="p23144139213115"></a><a name="p23144139213115"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.1.4.1.2 "><p id="p62735991213115"><a name="p62735991213115"></a><a name="p62735991213115"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p48450544213115"><a name="p48450544213115"></a><a name="p48450544213115"></a>需要更新的元数据的键。</p>
    <p id="p17337163611"><a name="p17337163611"></a><a name="p17337163611"></a>获取方法请参见<a href="查询云硬盘的元数据-Cinder-v3.md">查询云硬盘的元数据</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section27129916"></a>

-   请求参数

    <a name="evs_04_2078_table31588048"></a>
    <table><thead align="left"><tr id="evs_04_2078_row57330849"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="evs_04_2078_p13287175"><a name="evs_04_2078_p13287175"></a><a name="evs_04_2078_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="evs_04_2078_p2519427"><a name="evs_04_2078_p2519427"></a><a name="evs_04_2078_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="evs_04_2078_p2747002"><a name="evs_04_2078_p2747002"></a><a name="evs_04_2078_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="evs_04_2078_p21180630"><a name="evs_04_2078_p21180630"></a><a name="evs_04_2078_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2078_row53167494153413"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="evs_04_2078_p11599783153413"><a name="evs_04_2078_p11599783153413"></a><a name="evs_04_2078_p11599783153413"></a>meta</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="evs_04_2078_p58405153413"><a name="evs_04_2078_p58405153413"></a><a name="evs_04_2078_p58405153413"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="evs_04_2078_p4730855153413"><a name="evs_04_2078_p4730855153413"></a><a name="evs_04_2078_p4730855153413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="evs_04_2078_p47654998153413"><a name="evs_04_2078_p47654998153413"></a><a name="evs_04_2078_p47654998153413"></a>需要更新的元数据信息，请参见<a href="#evs_04_2078_li54973602211845">•meta参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2078_li54973602211845"></a>meta参数说明

    <a name="evs_04_2078_table32717123212358"></a>
    <table><thead align="left"><tr id="evs_04_2078_row2280240212358"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="evs_04_2078_p50481723212358"><a name="evs_04_2078_p50481723212358"></a><a name="evs_04_2078_p50481723212358"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="evs_04_2078_p62487767212358"><a name="evs_04_2078_p62487767212358"></a><a name="evs_04_2078_p62487767212358"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="evs_04_2078_p28344363212358"><a name="evs_04_2078_p28344363212358"></a><a name="evs_04_2078_p28344363212358"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="evs_04_2078_p14192096212358"><a name="evs_04_2078_p14192096212358"></a><a name="evs_04_2078_p14192096212358"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2078_row8709150212358"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="evs_04_2078_p34352524212358"><a name="evs_04_2078_p34352524212358"></a><a name="evs_04_2078_p34352524212358"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="evs_04_2078_p31091026212358"><a name="evs_04_2078_p31091026212358"></a><a name="evs_04_2078_p31091026212358"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2078_p35345177212358"><a name="evs_04_2078_p35345177212358"></a><a name="evs_04_2078_p35345177212358"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2078_p44387080212358"><a name="evs_04_2078_p44387080212358"></a><a name="evs_04_2078_p44387080212358"></a>一个键值对形式的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "meta": {
            "key1": "value1"
        }
    }
    ```


## 响应消息<a name="section42842654"></a>

-   响应参数

    <a name="evs_04_2078_table11977025201856"></a>
    <table><thead align="left"><tr id="evs_04_2078_row8102228201856"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="evs_04_2078_p52300707201856"><a name="evs_04_2078_p52300707201856"></a><a name="evs_04_2078_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="evs_04_2078_p3642697315541"><a name="evs_04_2078_p3642697315541"></a><a name="evs_04_2078_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="evs_04_2078_p17319263201856"><a name="evs_04_2078_p17319263201856"></a><a name="evs_04_2078_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2078_row60683035201856"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2078_p16378828201856"><a name="evs_04_2078_p16378828201856"></a><a name="evs_04_2078_p16378828201856"></a>meta</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2078_p6490369115541"><a name="evs_04_2078_p6490369115541"></a><a name="evs_04_2078_p6490369115541"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2078_p20205612201856"><a name="evs_04_2078_p20205612201856"></a><a name="evs_04_2078_p20205612201856"></a>键值对，云硬盘的单个元数据信息。</p>
    </td>
    </tr>
    <tr id="evs_04_2078_row9713816171"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2078_p129522216412"><a name="evs_04_2078_p129522216412"></a><a name="evs_04_2078_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2078_p1595262111415"><a name="evs_04_2078_p1595262111415"></a><a name="evs_04_2078_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2078_p109527215417"><a name="evs_04_2078_p109527215417"></a><a name="evs_04_2078_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2078_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2078_li0419202382514"></a>error参数说明

    <a name="evs_04_2078_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2078_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2078_evs_04_2013_p19541716103019"><a name="evs_04_2078_evs_04_2013_p19541716103019"></a><a name="evs_04_2078_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2078_evs_04_2013_p39375186103019"><a name="evs_04_2078_evs_04_2013_p39375186103019"></a><a name="evs_04_2078_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2078_evs_04_2013_p38578950103019"><a name="evs_04_2078_evs_04_2013_p38578950103019"></a><a name="evs_04_2078_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2078_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2078_evs_04_2013_p46815658103019"><a name="evs_04_2078_evs_04_2013_p46815658103019"></a><a name="evs_04_2078_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2078_evs_04_2013_p33971979103019"><a name="evs_04_2078_evs_04_2013_p33971979103019"></a><a name="evs_04_2078_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2078_evs_04_2013_p21623243103019"><a name="evs_04_2078_evs_04_2013_p21623243103019"></a><a name="evs_04_2078_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2078_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2078_evs_04_2013_p59870541103019"><a name="evs_04_2078_evs_04_2013_p59870541103019"></a><a name="evs_04_2078_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2078_evs_04_2013_p17675690103019"><a name="evs_04_2078_evs_04_2013_p17675690103019"></a><a name="evs_04_2078_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2078_evs_04_2013_p6087468103019"><a name="evs_04_2078_evs_04_2013_p6087468103019"></a><a name="evs_04_2078_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2078_evs_04_2013_p54787218103019"><a name="evs_04_2078_evs_04_2013_p54787218103019"></a><a name="evs_04_2078_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "meta": {
            "key1": "value1"
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


## 状态码<a name="section50039568"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

