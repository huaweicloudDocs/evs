# 设置云硬盘启动盘标识<a name="ZH-CN_TOPIC_0058626629"></a>

## 功能介绍<a name="section19390540"></a>

设置云硬盘启动盘标识。

## 约束<a name="section58153866104128"></a>

数据盘调用本接口设置bootable后，也不能挂载到云主机作为系统盘使用。

## URI<a name="section40297137"></a>

-   URI格式

    POST /v2/\{project\_id\}/volumes/\{volume\_id\}/action

-   参数说明

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="26%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="51%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="26%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="51%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section27129916"></a>

-   请求参数

    <a name="table42671863"></a>
    <table><thead align="left"><tr id="row12592542"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p13362997"><a name="p13362997"></a><a name="p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p8661001"><a name="p8661001"></a><a name="p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p30452481"><a name="p30452481"></a><a name="p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p50731910"><a name="p50731910"></a><a name="p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5187493615377"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p4112025815377"><a name="p4112025815377"></a><a name="p4112025815377"></a>os-set_bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p4240658415377"><a name="p4240658415377"></a><a name="p4240658415377"></a>map&lt;string, Boolean&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p1238131615377"><a name="p1238131615377"></a><a name="p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p6336250715377"><a name="p6336250715377"></a><a name="p6336250715377"></a>标记设置云硬盘启动盘操作。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   os-set\_bootable参数说明

    <a name="table38065209105423"></a>
    <table><thead align="left"><tr id="row47014882105423"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p50109122105423"><a name="p50109122105423"></a><a name="p50109122105423"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p32307099105423"><a name="p32307099105423"></a><a name="p32307099105423"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p66738196105423"><a name="p66738196105423"></a><a name="p66738196105423"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p37084757105423"><a name="p37084757105423"></a><a name="p37084757105423"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row65642867105423"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p5950372711131"><a name="p5950372711131"></a><a name="p5950372711131"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p45274007105423"><a name="p45274007105423"></a><a name="p45274007105423"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p43315944105423"><a name="p43315944105423"></a><a name="p43315944105423"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p18930541105423"><a name="p18930541105423"></a><a name="p18930541105423"></a>是否启动盘标识。</p>
    <a name="ul1334240319356"></a><a name="ul1334240319356"></a><ul id="ul1334240319356"><li>false：不启动</li><li>true：启动</li></ul>
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


## 响应<a name="section42842654"></a>

-   响应参数

    <a name="table46654279102454"></a>
    <table><thead align="left"><tr id="row6664264102454"><th class="cellrowborder" valign="top" width="20.48%" id="mcps1.1.4.1.1"><p id="p2934472102454"><a name="p2934472102454"></a><a name="p2934472102454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.69%" id="mcps1.1.4.1.2"><p id="p1338569102927"><a name="p1338569102927"></a><a name="p1338569102927"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.830000000000005%" id="mcps1.1.4.1.3"><p id="p23036595102454"><a name="p23036595102454"></a><a name="p23036595102454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row12419334102454"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p66442012102454"><a name="p66442012102454"></a><a name="p66442012102454"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p58201874102927"><a name="p58201874102927"></a><a name="p58201874102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p9725329102454"><a name="p9725329102454"></a><a name="p9725329102454"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="row20419099102454"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p43334338102454"><a name="p43334338102454"></a><a name="p43334338102454"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p16731376102927"><a name="p16731376102927"></a><a name="p16731376102927"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p29729347102454"><a name="p29729347102454"></a><a name="p29729347102454"></a>出现错误时，返回的错误码。</p>
    <p id="p66237533102454"><a name="p66237533102454"></a><a name="p66237533102454"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
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

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

