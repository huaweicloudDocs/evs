# 扩容云硬盘<a name="ZH-CN_TOPIC_0103340189"></a>

## 功能介绍<a name="section19390540"></a>

扩容云硬盘。

-   扩容状态为available的云硬盘时，没有约束限制。
-   扩容状态为in-use的云硬盘时，有以下约束：
    -   不支持共享云硬盘，即multiattach参数值必须为false。
    -   云硬盘所挂载的云服务器状态必须为ACTIVE、PAUSED、SUSPENDED、SHUTOFF才支持扩容。


## URI<a name="section40297137"></a>

-   URI格式

    POST /v3/\{project\_id\}/volumes/\{volume\_id\}/action

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="29.25%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.74%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="29.25%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="29.25%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID（非包周期）。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

-   请求参数

    <a name="zh-cn_topic_0058626625_table42671863"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626625_row12592542"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626625_p13362997"><a name="zh-cn_topic_0058626625_p13362997"></a><a name="zh-cn_topic_0058626625_p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626625_p8661001"><a name="zh-cn_topic_0058626625_p8661001"></a><a name="zh-cn_topic_0058626625_p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626625_p30452481"><a name="zh-cn_topic_0058626625_p30452481"></a><a name="zh-cn_topic_0058626625_p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626625_p50731910"><a name="zh-cn_topic_0058626625_p50731910"></a><a name="zh-cn_topic_0058626625_p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626625_row5187493615377"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626625_p4112025815377"><a name="zh-cn_topic_0058626625_p4112025815377"></a><a name="zh-cn_topic_0058626625_p4112025815377"></a>os-extend</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626625_p4240658415377"><a name="zh-cn_topic_0058626625_p4240658415377"></a><a name="zh-cn_topic_0058626625_p4240658415377"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626625_p1238131615377"><a name="zh-cn_topic_0058626625_p1238131615377"></a><a name="zh-cn_topic_0058626625_p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626625_p6336250715377"><a name="zh-cn_topic_0058626625_p6336250715377"></a><a name="zh-cn_topic_0058626625_p6336250715377"></a>标记扩容云硬盘操作。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   os-extend参数说明

    <a name="zh-cn_topic_0058626625_table38065209105423"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626625_row47014882105423"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626625_p50109122105423"><a name="zh-cn_topic_0058626625_p50109122105423"></a><a name="zh-cn_topic_0058626625_p50109122105423"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626625_p32307099105423"><a name="zh-cn_topic_0058626625_p32307099105423"></a><a name="zh-cn_topic_0058626625_p32307099105423"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626625_p66738196105423"><a name="zh-cn_topic_0058626625_p66738196105423"></a><a name="zh-cn_topic_0058626625_p66738196105423"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626625_p37084757105423"><a name="zh-cn_topic_0058626625_p37084757105423"></a><a name="zh-cn_topic_0058626625_p37084757105423"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626625_row65642867105423"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626625_p15472019105423"><a name="zh-cn_topic_0058626625_p15472019105423"></a><a name="zh-cn_topic_0058626625_p15472019105423"></a>new_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626625_p45274007105423"><a name="zh-cn_topic_0058626625_p45274007105423"></a><a name="zh-cn_topic_0058626625_p45274007105423"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626625_p43315944105423"><a name="zh-cn_topic_0058626625_p43315944105423"></a><a name="zh-cn_topic_0058626625_p43315944105423"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626625_p2427893615559"><a name="zh-cn_topic_0058626625_p2427893615559"></a><a name="zh-cn_topic_0058626625_p2427893615559"></a>扩容后云硬盘容量。扩容后的云硬盘容量必须大于扩容前云硬盘容量。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "os-extend": {
            "new_size": 100
        }
    }
    ```


## 响应<a name="section42842654"></a>

-   响应参数

    <a name="zh-cn_topic_0058626625_table46654279102454"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626625_row6664264102454"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626625_p2934472102454"><a name="zh-cn_topic_0058626625_p2934472102454"></a><a name="zh-cn_topic_0058626625_p2934472102454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626625_p1338569102927"><a name="zh-cn_topic_0058626625_p1338569102927"></a><a name="zh-cn_topic_0058626625_p1338569102927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626625_p23036595102454"><a name="zh-cn_topic_0058626625_p23036595102454"></a><a name="zh-cn_topic_0058626625_p23036595102454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626625_row12419334102454"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626625_p66442012102454"><a name="zh-cn_topic_0058626625_p66442012102454"></a><a name="zh-cn_topic_0058626625_p66442012102454"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626625_p58201874102927"><a name="zh-cn_topic_0058626625_p58201874102927"></a><a name="zh-cn_topic_0058626625_p58201874102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626625_p9725329102454"><a name="zh-cn_topic_0058626625_p9725329102454"></a><a name="zh-cn_topic_0058626625_p9725329102454"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058626625_row20419099102454"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626625_p43334338102454"><a name="zh-cn_topic_0058626625_p43334338102454"></a><a name="zh-cn_topic_0058626625_p43334338102454"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626625_p16731376102927"><a name="zh-cn_topic_0058626625_p16731376102927"></a><a name="zh-cn_topic_0058626625_p16731376102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626625_p29729347102454"><a name="zh-cn_topic_0058626625_p29729347102454"></a><a name="zh-cn_topic_0058626625_p29729347102454"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0058626625_p66237533102454"><a name="zh-cn_topic_0058626625_p66237533102454"></a><a name="zh-cn_topic_0058626625_p66237533102454"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

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

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

