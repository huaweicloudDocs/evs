# 更新云硬盘的单个元数据<a name="ZH-CN_TOPIC_0102657761"></a>

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
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

-   请求参数

    <a name="zh-cn_topic_0058626622_table31588048"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626622_row57330849"><th class="cellrowborder" valign="top" width="17.171717171717173%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626622_p13287175"><a name="zh-cn_topic_0058626622_p13287175"></a><a name="zh-cn_topic_0058626622_p13287175"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626622_p2519427"><a name="zh-cn_topic_0058626622_p2519427"></a><a name="zh-cn_topic_0058626622_p2519427"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626622_p2747002"><a name="zh-cn_topic_0058626622_p2747002"></a><a name="zh-cn_topic_0058626622_p2747002"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626622_p21180630"><a name="zh-cn_topic_0058626622_p21180630"></a><a name="zh-cn_topic_0058626622_p21180630"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626622_row53167494153413"><td class="cellrowborder" valign="top" width="17.171717171717173%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626622_p11599783153413"><a name="zh-cn_topic_0058626622_p11599783153413"></a><a name="zh-cn_topic_0058626622_p11599783153413"></a>meta</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626622_p58405153413"><a name="zh-cn_topic_0058626622_p58405153413"></a><a name="zh-cn_topic_0058626622_p58405153413"></a>map&lt;string,string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626622_p4730855153413"><a name="zh-cn_topic_0058626622_p4730855153413"></a><a name="zh-cn_topic_0058626622_p4730855153413"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626622_p47654998153413"><a name="zh-cn_topic_0058626622_p47654998153413"></a><a name="zh-cn_topic_0058626622_p47654998153413"></a>需要更新的元数据信息。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   meta参数说明

    <a name="zh-cn_topic_0058626622_table32717123212358"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626622_row2280240212358"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626622_p50481723212358"><a name="zh-cn_topic_0058626622_p50481723212358"></a><a name="zh-cn_topic_0058626622_p50481723212358"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626622_p62487767212358"><a name="zh-cn_topic_0058626622_p62487767212358"></a><a name="zh-cn_topic_0058626622_p62487767212358"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626622_p28344363212358"><a name="zh-cn_topic_0058626622_p28344363212358"></a><a name="zh-cn_topic_0058626622_p28344363212358"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626622_p14192096212358"><a name="zh-cn_topic_0058626622_p14192096212358"></a><a name="zh-cn_topic_0058626622_p14192096212358"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626622_row8709150212358"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626622_p34352524212358"><a name="zh-cn_topic_0058626622_p34352524212358"></a><a name="zh-cn_topic_0058626622_p34352524212358"></a>key_val</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626622_p31091026212358"><a name="zh-cn_topic_0058626622_p31091026212358"></a><a name="zh-cn_topic_0058626622_p31091026212358"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626622_p35345177212358"><a name="zh-cn_topic_0058626622_p35345177212358"></a><a name="zh-cn_topic_0058626622_p35345177212358"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626622_p44387080212358"><a name="zh-cn_topic_0058626622_p44387080212358"></a><a name="zh-cn_topic_0058626622_p44387080212358"></a>一个键值对形式的元数据信息。</p>
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


## 响应<a name="section42842654"></a>

-   响应参数

    <a name="zh-cn_topic_0058626622_table11977025201856"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626622_row8102228201856"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626622_p52300707201856"><a name="zh-cn_topic_0058626622_p52300707201856"></a><a name="zh-cn_topic_0058626622_p52300707201856"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626622_p3642697315541"><a name="zh-cn_topic_0058626622_p3642697315541"></a><a name="zh-cn_topic_0058626622_p3642697315541"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626622_p17319263201856"><a name="zh-cn_topic_0058626622_p17319263201856"></a><a name="zh-cn_topic_0058626622_p17319263201856"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626622_row60683035201856"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626622_p16378828201856"><a name="zh-cn_topic_0058626622_p16378828201856"></a><a name="zh-cn_topic_0058626622_p16378828201856"></a>meta</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626622_p6490369115541"><a name="zh-cn_topic_0058626622_p6490369115541"></a><a name="zh-cn_topic_0058626622_p6490369115541"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626622_p20205612201856"><a name="zh-cn_topic_0058626622_p20205612201856"></a><a name="zh-cn_topic_0058626622_p20205612201856"></a>键值对，云硬盘的单个元数据信息。</p>
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


## 返回值<a name="section50039568"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

