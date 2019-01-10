# 添加云硬盘快照的元数据<a name="ZH-CN_TOPIC_0102707574"></a>

## 功能介绍<a name="section4805694511340"></a>

添加云硬盘快照的元数据。

## URI<a name="section268627411340"></a>

-   URI格式

    POST /v3/\{project\_id\}/snapshots/\{snapshot\_id\}/metadata

-   参数说明

    <a name="table5655293911340"></a>
    <table><thead align="left"><tr id="row4718979611340"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p6427715211340"><a name="p6427715211340"></a><a name="p6427715211340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p3906685711340"><a name="p3906685711340"></a><a name="p3906685711340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p1029885411340"><a name="p1029885411340"></a><a name="p1029885411340"></a>说明</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2890086411340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p116468178394"><a name="p116468178394"></a><a name="p116468178394"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3603037711340"><a name="p3603037711340"></a><a name="p3603037711340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p3277940011340"><a name="p3277940011340"></a><a name="p3277940011340"></a>项目ID。</p>
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


## 请求<a name="section87667311340"></a>

-   请求参数

    <a name="zh-cn_topic_0058626632_table9796961112814"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626632_row1541837112814"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626632_p51734634112841"><a name="zh-cn_topic_0058626632_p51734634112841"></a><a name="zh-cn_topic_0058626632_p51734634112841"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626632_p29755832112841"><a name="zh-cn_topic_0058626632_p29755832112841"></a><a name="zh-cn_topic_0058626632_p29755832112841"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626632_p61412231112841"><a name="zh-cn_topic_0058626632_p61412231112841"></a><a name="zh-cn_topic_0058626632_p61412231112841"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626632_p8334847112841"><a name="zh-cn_topic_0058626632_p8334847112841"></a><a name="zh-cn_topic_0058626632_p8334847112841"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626632_row15415933112814"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626632_p40731045112814"><a name="zh-cn_topic_0058626632_p40731045112814"></a><a name="zh-cn_topic_0058626632_p40731045112814"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626632_p10880325112814"><a name="zh-cn_topic_0058626632_p10880325112814"></a><a name="zh-cn_topic_0058626632_p10880325112814"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626632_p8891142112814"><a name="zh-cn_topic_0058626632_p8891142112814"></a><a name="zh-cn_topic_0058626632_p8891142112814"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626632_p49093903112814"><a name="zh-cn_topic_0058626632_p49093903112814"></a><a name="zh-cn_topic_0058626632_p49093903112814"></a>待添加的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   metadata参数说明

    <a name="zh-cn_topic_0058626632_table17183241112814"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626632_row29429246112814"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626632_p59908985112845"><a name="zh-cn_topic_0058626632_p59908985112845"></a><a name="zh-cn_topic_0058626632_p59908985112845"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626632_p20789580112845"><a name="zh-cn_topic_0058626632_p20789580112845"></a><a name="zh-cn_topic_0058626632_p20789580112845"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626632_p6234457112845"><a name="zh-cn_topic_0058626632_p6234457112845"></a><a name="zh-cn_topic_0058626632_p6234457112845"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626632_p35228998112845"><a name="zh-cn_topic_0058626632_p35228998112845"></a><a name="zh-cn_topic_0058626632_p35228998112845"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626632_row40467139112814"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626632_p56612845112814"><a name="zh-cn_topic_0058626632_p56612845112814"></a><a name="zh-cn_topic_0058626632_p56612845112814"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626632_p22237723112814"><a name="zh-cn_topic_0058626632_p22237723112814"></a><a name="zh-cn_topic_0058626632_p22237723112814"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626632_p56425142112814"><a name="zh-cn_topic_0058626632_p56425142112814"></a><a name="zh-cn_topic_0058626632_p56425142112814"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626632_p7033765112814"><a name="zh-cn_topic_0058626632_p7033765112814"></a><a name="zh-cn_topic_0058626632_p7033765112814"></a>一个或多个键值对形式的元数据信息。</p>
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


## 响应<a name="section5147449911340"></a>

-   响应参数

    <a name="zh-cn_topic_0058626632_table11977025201856"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626632_row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626632_p52300707201856"><a name="zh-cn_topic_0058626632_p52300707201856"></a><a name="zh-cn_topic_0058626632_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626632_p3642697315541"><a name="zh-cn_topic_0058626632_p3642697315541"></a><a name="zh-cn_topic_0058626632_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626632_p17319263201856"><a name="zh-cn_topic_0058626632_p17319263201856"></a><a name="zh-cn_topic_0058626632_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626632_row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626632_p16378828201856"><a name="zh-cn_topic_0058626632_p16378828201856"></a><a name="zh-cn_topic_0058626632_p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626632_p6490369115541"><a name="zh-cn_topic_0058626632_p6490369115541"></a><a name="zh-cn_topic_0058626632_p6490369115541"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626632_p20205612201856"><a name="zh-cn_topic_0058626632_p20205612201856"></a><a name="zh-cn_topic_0058626632_p20205612201856"></a>键值对，云硬盘快照的元数据信息。</p>
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


## 返回值<a name="section1751558211340"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

