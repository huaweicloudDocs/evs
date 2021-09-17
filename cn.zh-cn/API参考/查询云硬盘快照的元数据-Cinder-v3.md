# 查询云硬盘快照的元数据<a name="evs_04_3063"></a>

## 功能介绍<a name="section4805694511340"></a>

查询云硬盘快照的元数据。

## URI<a name="section268627411340"></a>

-   URI格式

    GET /v3/\{project\_id\}/snapshots/\{snapshot\_id\}/metadata

-   参数说明

    <a name="table5655293911340"></a>
    <table><thead align="left"><tr id="row4718979611340"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p6427715211340"><a name="p6427715211340"></a><a name="p6427715211340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p3906685711340"><a name="p3906685711340"></a><a name="p3906685711340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1029885411340"><a name="p1029885411340"></a><a name="p1029885411340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2890086411340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p5926863811340"><a name="p5926863811340"></a><a name="p5926863811340"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3603037711340"><a name="p3603037711340"></a><a name="p3603037711340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p3277940011340"><a name="p3277940011340"></a><a name="p3277940011340"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row2657914711340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p542726811340"><a name="p542726811340"></a><a name="p542726811340"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3695552511340"><a name="p3695552511340"></a><a name="p3695552511340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4060754311340"><a name="p4060754311340"></a><a name="p4060754311340"></a>快照ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section87667311340"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v3/{project_id}/snapshots/f9faf7df-fdc1-4093-9ef3-5cba06eef995/metadata
    ```


## 响应消息<a name="section5147449911340"></a>

-   响应参数

    <a name="evs_04_2100_table11977025201856"></a>
    <table><thead align="left"><tr id="evs_04_2100_row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="evs_04_2100_p52300707201856"><a name="evs_04_2100_p52300707201856"></a><a name="evs_04_2100_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2100_p3642697315541"><a name="evs_04_2100_p3642697315541"></a><a name="evs_04_2100_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2100_p17319263201856"><a name="evs_04_2100_p17319263201856"></a><a name="evs_04_2100_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2100_row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2100_p16378828201856"><a name="evs_04_2100_p16378828201856"></a><a name="evs_04_2100_p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2100_p6490369115541"><a name="evs_04_2100_p6490369115541"></a><a name="evs_04_2100_p6490369115541"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2100_p20205612201856"><a name="evs_04_2100_p20205612201856"></a><a name="evs_04_2100_p20205612201856"></a>键值对，云硬盘快照的元数据信息。</p>
    <p id="evs_04_2100_p2691143564618"><a name="evs_04_2100_p2691143564618"></a><a name="evs_04_2100_p2691143564618"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="evs_04_2100_row147215921119"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2100_p129522216412"><a name="evs_04_2100_p129522216412"></a><a name="evs_04_2100_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2100_p1595262111415"><a name="evs_04_2100_p1595262111415"></a><a name="evs_04_2100_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2100_p109527215417"><a name="evs_04_2100_p109527215417"></a><a name="evs_04_2100_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2100_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2100_li0419202382514"></a>error参数说明

    <a name="evs_04_2100_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2100_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2100_evs_04_2013_p19541716103019"><a name="evs_04_2100_evs_04_2013_p19541716103019"></a><a name="evs_04_2100_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2100_evs_04_2013_p39375186103019"><a name="evs_04_2100_evs_04_2013_p39375186103019"></a><a name="evs_04_2100_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2100_evs_04_2013_p38578950103019"><a name="evs_04_2100_evs_04_2013_p38578950103019"></a><a name="evs_04_2100_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2100_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2100_evs_04_2013_p46815658103019"><a name="evs_04_2100_evs_04_2013_p46815658103019"></a><a name="evs_04_2100_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2100_evs_04_2013_p33971979103019"><a name="evs_04_2100_evs_04_2013_p33971979103019"></a><a name="evs_04_2100_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2100_evs_04_2013_p21623243103019"><a name="evs_04_2100_evs_04_2013_p21623243103019"></a><a name="evs_04_2100_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2100_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2100_evs_04_2013_p59870541103019"><a name="evs_04_2100_evs_04_2013_p59870541103019"></a><a name="evs_04_2100_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2100_evs_04_2013_p17675690103019"><a name="evs_04_2100_evs_04_2013_p17675690103019"></a><a name="evs_04_2100_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2100_evs_04_2013_p6087468103019"><a name="evs_04_2100_evs_04_2013_p6087468103019"></a><a name="evs_04_2100_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2100_evs_04_2013_p54787218103019"><a name="evs_04_2100_evs_04_2013_p54787218103019"></a><a name="evs_04_2100_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

    ```
    {
        "badRequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section1751558211340"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

