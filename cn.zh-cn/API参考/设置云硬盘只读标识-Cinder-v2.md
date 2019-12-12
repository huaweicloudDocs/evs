# 设置云硬盘只读标识<a name="zh-cn_topic_0058626630"></a>

## 功能介绍<a name="section19390540"></a>

设置云硬盘只读标识。

## URI<a name="section40297137"></a>

-   URI格式

    POST /v2/\{project\_id\}/volumes/\{volume\_id\}/action

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="27%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section27129916"></a>

-   请求参数

    <a name="table42671863"></a>
    <table><thead align="left"><tr id="row12592542"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="p13362997"><a name="p13362997"></a><a name="p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.1.5.1.2"><p id="p8661001"><a name="p8661001"></a><a name="p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p30452481"><a name="p30452481"></a><a name="p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.524752475247524%" id="mcps1.1.5.1.4"><p id="p50731910"><a name="p50731910"></a><a name="p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5187493615377"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p4112025815377"><a name="p4112025815377"></a><a name="p4112025815377"></a>os-update_readonly_flag</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.1.5.1.2 "><p id="p4240658415377"><a name="p4240658415377"></a><a name="p4240658415377"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1238131615377"><a name="p1238131615377"></a><a name="p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.1.5.1.4 "><p id="p6336250715377"><a name="p6336250715377"></a><a name="p6336250715377"></a>标记设置云硬盘只读标识操作，请参见<a href="#li55520608111457">•os-update_readonly_flag...</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li55520608111457"></a>os-update\_readonly\_flag参数说明

    <a name="table38065209105423"></a>
    <table><thead align="left"><tr id="row47014882105423"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.1"><p id="p50109122105423"><a name="p50109122105423"></a><a name="p50109122105423"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.191919191919194%" id="mcps1.1.5.1.2"><p id="p32307099105423"><a name="p32307099105423"></a><a name="p32307099105423"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="p66738196105423"><a name="p66738196105423"></a><a name="p66738196105423"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47.474747474747474%" id="mcps1.1.5.1.4"><p id="p37084757105423"><a name="p37084757105423"></a><a name="p37084757105423"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row65642867105423"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="p1874528111511"><a name="p1874528111511"></a><a name="p1874528111511"></a>readonly</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.191919191919194%" headers="mcps1.1.5.1.2 "><p id="p45274007105423"><a name="p45274007105423"></a><a name="p45274007105423"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="p43315944105423"><a name="p43315944105423"></a><a name="p43315944105423"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47.474747474747474%" headers="mcps1.1.5.1.4 "><div class="p" id="p18930541105423"><a name="p18930541105423"></a><a name="p18930541105423"></a>是否只读标识。<a name="ul4954137112218"></a><a name="ul4954137112218"></a><ul id="ul4954137112218"><li>true：表示只读。</li><li>false：表示非只读。</li></ul>
    </div>
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


## 响应消息<a name="section42842654"></a>

-   响应参数

    <a name="table5532594121252"></a>
    <table><thead align="left"><tr id="row60048709121252"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p32107236121252"><a name="p32107236121252"></a><a name="p32107236121252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p50549312121252"><a name="p50549312121252"></a><a name="p50549312121252"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p2030156121252"><a name="p2030156121252"></a><a name="p2030156121252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row30224973121252"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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


## 状态码<a name="section50039568"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

