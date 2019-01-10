# 设置云硬盘只读标识<a name="ZH-CN_TOPIC_0103340193"></a>

## 功能介绍<a name="section19390540"></a>

设置云硬盘只读标识。

## URI<a name="section40297137"></a>

-   URI格式

    POST /v3/\{project\_id\}/volumes/\{volume\_id\}/action

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="30%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.990000000000002%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.990000000000002%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="30%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.990000000000002%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

-   请求参数

    <a name="zh-cn_topic_0058626630_table42671863"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626630_row12592542"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626630_p13362997"><a name="zh-cn_topic_0058626630_p13362997"></a><a name="zh-cn_topic_0058626630_p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626630_p8661001"><a name="zh-cn_topic_0058626630_p8661001"></a><a name="zh-cn_topic_0058626630_p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626630_p30452481"><a name="zh-cn_topic_0058626630_p30452481"></a><a name="zh-cn_topic_0058626630_p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.524752475247524%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626630_p50731910"><a name="zh-cn_topic_0058626630_p50731910"></a><a name="zh-cn_topic_0058626630_p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626630_row5187493615377"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626630_p4112025815377"><a name="zh-cn_topic_0058626630_p4112025815377"></a><a name="zh-cn_topic_0058626630_p4112025815377"></a>os-update_readonly_flag</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626630_p4240658415377"><a name="zh-cn_topic_0058626630_p4240658415377"></a><a name="zh-cn_topic_0058626630_p4240658415377"></a>map&lt;string, Boolean&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626630_p1238131615377"><a name="zh-cn_topic_0058626630_p1238131615377"></a><a name="zh-cn_topic_0058626630_p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626630_p6336250715377"><a name="zh-cn_topic_0058626630_p6336250715377"></a><a name="zh-cn_topic_0058626630_p6336250715377"></a>标记设置云硬盘只读标识操作。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   os-update\_readonly\_flag参数说明

    <a name="zh-cn_topic_0058626630_table38065209105423"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626630_row47014882105423"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0058626630_p50109122105423"><a name="zh-cn_topic_0058626630_p50109122105423"></a><a name="zh-cn_topic_0058626630_p50109122105423"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.191919191919194%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0058626630_p32307099105423"><a name="zh-cn_topic_0058626630_p32307099105423"></a><a name="zh-cn_topic_0058626630_p32307099105423"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0058626630_p66738196105423"><a name="zh-cn_topic_0058626630_p66738196105423"></a><a name="zh-cn_topic_0058626630_p66738196105423"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.474747474747474%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0058626630_p37084757105423"><a name="zh-cn_topic_0058626630_p37084757105423"></a><a name="zh-cn_topic_0058626630_p37084757105423"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626630_row65642867105423"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0058626630_p1874528111511"><a name="zh-cn_topic_0058626630_p1874528111511"></a><a name="zh-cn_topic_0058626630_p1874528111511"></a>readonly</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0058626630_p45274007105423"><a name="zh-cn_topic_0058626630_p45274007105423"></a><a name="zh-cn_topic_0058626630_p45274007105423"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0058626630_p43315944105423"><a name="zh-cn_topic_0058626630_p43315944105423"></a><a name="zh-cn_topic_0058626630_p43315944105423"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.474747474747474%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0058626630_p18930541105423"><a name="zh-cn_topic_0058626630_p18930541105423"></a><a name="zh-cn_topic_0058626630_p18930541105423"></a>是否只读标识。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "os-update_readonly_flag": {
            "readonly": true
        }
    }
    ```


## 响应<a name="section42842654"></a>

-   响应参数

    <a name="zh-cn_topic_0058626630_table46654279102454"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0058626630_row6664264102454"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0058626630_p2934472102454"><a name="zh-cn_topic_0058626630_p2934472102454"></a><a name="zh-cn_topic_0058626630_p2934472102454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0058626630_p1338569102927"><a name="zh-cn_topic_0058626630_p1338569102927"></a><a name="zh-cn_topic_0058626630_p1338569102927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0058626630_p23036595102454"><a name="zh-cn_topic_0058626630_p23036595102454"></a><a name="zh-cn_topic_0058626630_p23036595102454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0058626630_row12419334102454"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626630_p66442012102454"><a name="zh-cn_topic_0058626630_p66442012102454"></a><a name="zh-cn_topic_0058626630_p66442012102454"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626630_p58201874102927"><a name="zh-cn_topic_0058626630_p58201874102927"></a><a name="zh-cn_topic_0058626630_p58201874102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626630_p9725329102454"><a name="zh-cn_topic_0058626630_p9725329102454"></a><a name="zh-cn_topic_0058626630_p9725329102454"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0058626630_row20419099102454"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0058626630_p43334338102454"><a name="zh-cn_topic_0058626630_p43334338102454"></a><a name="zh-cn_topic_0058626630_p43334338102454"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0058626630_p16731376102927"><a name="zh-cn_topic_0058626630_p16731376102927"></a><a name="zh-cn_topic_0058626630_p16731376102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0058626630_p29729347102454"><a name="zh-cn_topic_0058626630_p29729347102454"></a><a name="zh-cn_topic_0058626630_p29729347102454"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0058626630_p66237533102454"><a name="zh-cn_topic_0058626630_p66237533102454"></a><a name="zh-cn_topic_0058626630_p66237533102454"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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
        "itemNotFound": {
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

