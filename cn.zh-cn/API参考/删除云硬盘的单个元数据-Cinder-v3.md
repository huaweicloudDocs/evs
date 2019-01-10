# 删除云硬盘的单个元数据<a name="ZH-CN_TOPIC_0102659992"></a>

## 功能介绍<a name="section19390540"></a>

删除云硬盘的单个元数据。

## URI<a name="section40297137"></a>

-   URI格式

    DELETE /v3/\{project\_id\}/volumes/\{volume\_id\}/metadata/\{key\}

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
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="28.92%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row21272210213647"><td class="cellrowborder" valign="top" width="28.92%" headers="mcps1.1.4.1.1 "><p id="p45327484213647"><a name="p45327484213647"></a><a name="p45327484213647"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.07%" headers="mcps1.1.4.1.2 "><p id="p47647615213647"><a name="p47647615213647"></a><a name="p47647615213647"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p34251586213647"><a name="p34251586213647"></a><a name="p34251586213647"></a>需要删除的元数据的键。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

无

## 响应<a name="section42842654"></a>

-   响应参数

    <a name="zh-cn_topic_0058626623_table5532594121252"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626623_row60048709121252"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626623_p32107236121252"><a name="zh-cn_topic_0058626623_p32107236121252"></a><a name="zh-cn_topic_0058626623_p32107236121252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626623_p50549312121252"><a name="zh-cn_topic_0058626623_p50549312121252"></a><a name="zh-cn_topic_0058626623_p50549312121252"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626623_p2030156121252"><a name="zh-cn_topic_0058626623_p2030156121252"></a><a name="zh-cn_topic_0058626623_p2030156121252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626623_row30224973121252"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626623_p32303787121252"><a name="zh-cn_topic_0058626623_p32303787121252"></a><a name="zh-cn_topic_0058626623_p32303787121252"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626623_p66469965121252"><a name="zh-cn_topic_0058626623_p66469965121252"></a><a name="zh-cn_topic_0058626623_p66469965121252"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626623_p36047231121252"><a name="zh-cn_topic_0058626623_p36047231121252"></a><a name="zh-cn_topic_0058626623_p36047231121252"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058626623_row55989628121252"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626623_p38866009121252"><a name="zh-cn_topic_0058626623_p38866009121252"></a><a name="zh-cn_topic_0058626623_p38866009121252"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626623_p61139006121252"><a name="zh-cn_topic_0058626623_p61139006121252"></a><a name="zh-cn_topic_0058626623_p61139006121252"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626623_p23342658121252"><a name="zh-cn_topic_0058626623_p23342658121252"></a><a name="zh-cn_topic_0058626623_p23342658121252"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0058626623_p8757338121252"><a name="zh-cn_topic_0058626623_p8757338121252"></a><a name="zh-cn_topic_0058626623_p8757338121252"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    无

    或

    ```
    {
        "error": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```

    其中error是泛指的错误，有badrequest、itemNotFound等，如报错：

    ```
    {
        "itemNotFound": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 返回值<a name="section50039568"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

