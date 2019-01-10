# 更新云硬盘的元数据<a name="ZH-CN_TOPIC_0102653908"></a>

## 功能介绍<a name="section19390540"></a>

更新云硬盘的元数据。

## URI<a name="section40297137"></a>

-   URI格式

    PUT /v3/\{project\_id\}/volumes/\{volume\_id\}/metadata

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="28.49%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.5%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="28.49%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.5%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="28.49%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.5%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

-   请求参数

    <a name="zh-cn_topic_0058626621_table31588048"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626621_row57330849"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626621_p13287175"><a name="zh-cn_topic_0058626621_p13287175"></a><a name="zh-cn_topic_0058626621_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626621_p2519427"><a name="zh-cn_topic_0058626621_p2519427"></a><a name="zh-cn_topic_0058626621_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626621_p2747002"><a name="zh-cn_topic_0058626621_p2747002"></a><a name="zh-cn_topic_0058626621_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626621_p21180630"><a name="zh-cn_topic_0058626621_p21180630"></a><a name="zh-cn_topic_0058626621_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626621_row53167494153413"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626621_p11599783153413"><a name="zh-cn_topic_0058626621_p11599783153413"></a><a name="zh-cn_topic_0058626621_p11599783153413"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626621_p58405153413"><a name="zh-cn_topic_0058626621_p58405153413"></a><a name="zh-cn_topic_0058626621_p58405153413"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626621_p4730855153413"><a name="zh-cn_topic_0058626621_p4730855153413"></a><a name="zh-cn_topic_0058626621_p4730855153413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626621_p47654998153413"><a name="zh-cn_topic_0058626621_p47654998153413"></a><a name="zh-cn_topic_0058626621_p47654998153413"></a>需要更新的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   metadata参数说明

    <a name="zh-cn_topic_0058626621_table32717123212358"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626621_row2280240212358"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626621_p1603155994915"><a name="zh-cn_topic_0058626621_p1603155994915"></a><a name="zh-cn_topic_0058626621_p1603155994915"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.191919191919194%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626621_p62487767212358"><a name="zh-cn_topic_0058626621_p62487767212358"></a><a name="zh-cn_topic_0058626621_p62487767212358"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626621_p28344363212358"><a name="zh-cn_topic_0058626621_p28344363212358"></a><a name="zh-cn_topic_0058626621_p28344363212358"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.474747474747474%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626621_p14192096212358"><a name="zh-cn_topic_0058626621_p14192096212358"></a><a name="zh-cn_topic_0058626621_p14192096212358"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626621_row8709150212358"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626621_p34352524212358"><a name="zh-cn_topic_0058626621_p34352524212358"></a><a name="zh-cn_topic_0058626621_p34352524212358"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626621_p31091026212358"><a name="zh-cn_topic_0058626621_p31091026212358"></a><a name="zh-cn_topic_0058626621_p31091026212358"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626621_p35345177212358"><a name="zh-cn_topic_0058626621_p35345177212358"></a><a name="zh-cn_topic_0058626621_p35345177212358"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.474747474747474%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626621_p44387080212358"><a name="zh-cn_topic_0058626621_p44387080212358"></a><a name="zh-cn_topic_0058626621_p44387080212358"></a>一个或多个键值对形式的元数据信息。</p>
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


## 响应<a name="section42842654"></a>

-   响应参数

    <a name="zh-cn_topic_0058626621_table11977025201856"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626621_row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626621_p52300707201856"><a name="zh-cn_topic_0058626621_p52300707201856"></a><a name="zh-cn_topic_0058626621_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626621_p3642697315541"><a name="zh-cn_topic_0058626621_p3642697315541"></a><a name="zh-cn_topic_0058626621_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626621_p17319263201856"><a name="zh-cn_topic_0058626621_p17319263201856"></a><a name="zh-cn_topic_0058626621_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626621_row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626621_p16378828201856"><a name="zh-cn_topic_0058626621_p16378828201856"></a><a name="zh-cn_topic_0058626621_p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626621_p6490369115541"><a name="zh-cn_topic_0058626621_p6490369115541"></a><a name="zh-cn_topic_0058626621_p6490369115541"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626621_p20205612201856"><a name="zh-cn_topic_0058626621_p20205612201856"></a><a name="zh-cn_topic_0058626621_p20205612201856"></a>键值对，云硬盘的元数据信息。</p>
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


## 返回值<a name="section50039568"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

