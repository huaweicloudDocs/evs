# 查询云硬盘快照的单个元数据<a name="ZH-CN_TOPIC_0102724001"></a>

## 功能介绍<a name="section4805694511340"></a>

查询云硬盘快照的单个元数据。

## URI<a name="section268627411340"></a>

-   URI格式

    GET /v3/\{project\_id\}/snapshots/\{snapshot\_id\}/metadata/\{key\}

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
    </td>
    </tr>
    <tr id="row2657914711340"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p542726811340"><a name="p542726811340"></a><a name="p542726811340"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p3695552511340"><a name="p3695552511340"></a><a name="p3695552511340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p4060754311340"><a name="p4060754311340"></a><a name="p4060754311340"></a>快照ID。</p>
    </td>
    </tr>
    <tr id="row8510929141217"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p18296649141217"><a name="p18296649141217"></a><a name="p18296649141217"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p5633614141217"><a name="p5633614141217"></a><a name="p5633614141217"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p53669575141217"><a name="p53669575141217"></a><a name="p53669575141217"></a>待查询的元数据的键。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section87667311340"></a>

无

## 响应<a name="section5147449911340"></a>

-   响应参数

    <a name="zh-cn_topic_0058626636_table11977025201856"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626636_row8102228201856"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626636_p52300707201856"><a name="zh-cn_topic_0058626636_p52300707201856"></a><a name="zh-cn_topic_0058626636_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626636_p3642697315541"><a name="zh-cn_topic_0058626636_p3642697315541"></a><a name="zh-cn_topic_0058626636_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626636_p17319263201856"><a name="zh-cn_topic_0058626636_p17319263201856"></a><a name="zh-cn_topic_0058626636_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626636_row60683035201856"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626636_p16378828201856"><a name="zh-cn_topic_0058626636_p16378828201856"></a><a name="zh-cn_topic_0058626636_p16378828201856"></a>meta</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626636_p6490369115541"><a name="zh-cn_topic_0058626636_p6490369115541"></a><a name="zh-cn_topic_0058626636_p6490369115541"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626636_p20205612201856"><a name="zh-cn_topic_0058626636_p20205612201856"></a><a name="zh-cn_topic_0058626636_p20205612201856"></a>键值对，云硬盘快照的单个元数据信息。</p>
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


