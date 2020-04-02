# 设置云硬盘启动盘标识<a name="evs_04_3049"></a>

## 功能介绍<a name="section19390540"></a>

设置云硬盘启动盘标识。

## 接口约束<a name="section58153866104128"></a>

数据盘调用本接口设置bootable后，也不能挂载到云主机作为系统盘使用。

## URI<a name="section40297137"></a>

-   URI格式

    POST /v3/\{project\_id\}/volumes/\{volume\_id\}/action

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
    </tbody>
    </table>


## 请求消息<a name="section27129916"></a>

-   请求参数

    <a name="evs_04_2084_table42671863"></a>
    <table><thead align="left"><tr id="evs_04_2084_row12592542"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2084_p13362997"><a name="evs_04_2084_p13362997"></a><a name="evs_04_2084_p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2084_p8661001"><a name="evs_04_2084_p8661001"></a><a name="evs_04_2084_p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="evs_04_2084_p30452481"><a name="evs_04_2084_p30452481"></a><a name="evs_04_2084_p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="evs_04_2084_p50731910"><a name="evs_04_2084_p50731910"></a><a name="evs_04_2084_p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2084_row5187493615377"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2084_p4112025815377"><a name="evs_04_2084_p4112025815377"></a><a name="evs_04_2084_p4112025815377"></a>os-set_bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2084_p4240658415377"><a name="evs_04_2084_p4240658415377"></a><a name="evs_04_2084_p4240658415377"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2084_p1238131615377"><a name="evs_04_2084_p1238131615377"></a><a name="evs_04_2084_p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2084_p6336250715377"><a name="evs_04_2084_p6336250715377"></a><a name="evs_04_2084_p6336250715377"></a>标记设置云硬盘启动盘操作，请参见<a href="#evs_04_2084_li11686008105423">•os-set_bootable参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2084_li11686008105423"></a>os-set\_bootable参数说明

    <a name="evs_04_2084_table38065209105423"></a>
    <table><thead align="left"><tr id="evs_04_2084_row47014882105423"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="evs_04_2084_p50109122105423"><a name="evs_04_2084_p50109122105423"></a><a name="evs_04_2084_p50109122105423"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="evs_04_2084_p32307099105423"><a name="evs_04_2084_p32307099105423"></a><a name="evs_04_2084_p32307099105423"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="evs_04_2084_p66738196105423"><a name="evs_04_2084_p66738196105423"></a><a name="evs_04_2084_p66738196105423"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="evs_04_2084_p37084757105423"><a name="evs_04_2084_p37084757105423"></a><a name="evs_04_2084_p37084757105423"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2084_row65642867105423"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="evs_04_2084_p5950372711131"><a name="evs_04_2084_p5950372711131"></a><a name="evs_04_2084_p5950372711131"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="evs_04_2084_p45274007105423"><a name="evs_04_2084_p45274007105423"></a><a name="evs_04_2084_p45274007105423"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="evs_04_2084_p43315944105423"><a name="evs_04_2084_p43315944105423"></a><a name="evs_04_2084_p43315944105423"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="evs_04_2084_p18930541105423"><a name="evs_04_2084_p18930541105423"></a><a name="evs_04_2084_p18930541105423"></a>是否启动盘标识。</p>
    <a name="evs_04_2084_ul1334240319356"></a><a name="evs_04_2084_ul1334240319356"></a><ul id="evs_04_2084_ul1334240319356"><li>false：不启动</li><li>true：启动</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "os-set_bootable": {
            "bootable": true
        }
    }
    ```


## 响应消息<a name="section42842654"></a>

-   响应参数

    <a name="evs_04_2084_table5532594121252"></a>
    <table><thead align="left"><tr id="evs_04_2084_row60048709121252"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2084_p32107236121252"><a name="evs_04_2084_p32107236121252"></a><a name="evs_04_2084_p32107236121252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2084_p50549312121252"><a name="evs_04_2084_p50549312121252"></a><a name="evs_04_2084_p50549312121252"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2084_p2030156121252"><a name="evs_04_2084_p2030156121252"></a><a name="evs_04_2084_p2030156121252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2084_row30224973121252"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2084_p129522216412"><a name="evs_04_2084_p129522216412"></a><a name="evs_04_2084_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2084_p1595262111415"><a name="evs_04_2084_p1595262111415"></a><a name="evs_04_2084_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2084_p109527215417"><a name="evs_04_2084_p109527215417"></a><a name="evs_04_2084_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2084_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2084_li0419202382514"></a>error参数说明

    <a name="evs_04_2084_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2084_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2084_evs_04_2013_p19541716103019"><a name="evs_04_2084_evs_04_2013_p19541716103019"></a><a name="evs_04_2084_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2084_evs_04_2013_p39375186103019"><a name="evs_04_2084_evs_04_2013_p39375186103019"></a><a name="evs_04_2084_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2084_evs_04_2013_p38578950103019"><a name="evs_04_2084_evs_04_2013_p38578950103019"></a><a name="evs_04_2084_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2084_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2084_evs_04_2013_p46815658103019"><a name="evs_04_2084_evs_04_2013_p46815658103019"></a><a name="evs_04_2084_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2084_evs_04_2013_p33971979103019"><a name="evs_04_2084_evs_04_2013_p33971979103019"></a><a name="evs_04_2084_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2084_evs_04_2013_p21623243103019"><a name="evs_04_2084_evs_04_2013_p21623243103019"></a><a name="evs_04_2084_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2084_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2084_evs_04_2013_p59870541103019"><a name="evs_04_2084_evs_04_2013_p59870541103019"></a><a name="evs_04_2084_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2084_evs_04_2013_p17675690103019"><a name="evs_04_2084_evs_04_2013_p17675690103019"></a><a name="evs_04_2084_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2084_evs_04_2013_p6087468103019"><a name="evs_04_2084_evs_04_2013_p6087468103019"></a><a name="evs_04_2084_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2084_evs_04_2013_p54787218103019"><a name="evs_04_2084_evs_04_2013_p54787218103019"></a><a name="evs_04_2084_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

