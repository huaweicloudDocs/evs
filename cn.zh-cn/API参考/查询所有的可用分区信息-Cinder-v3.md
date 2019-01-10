# 查询所有的可用分区信息<a name="ZH-CN_TOPIC_0102666148"></a>

## 功能介绍<a name="section54465313"></a>

查询所有的可用分区信息。

## URI<a name="section20425774"></a>

-   URI格式

    GET /v3/\{project\_id\}/os-availability-zone

-   参数说明

    <a name="table34934986"></a>
    <table><thead align="left"><tr id="row15816986"><th class="cellrowborder" valign="top" width="29.68296829682968%" id="mcps1.1.4.1.1"><p id="p6107499"><a name="p6107499"></a><a name="p6107499"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.012401240124014%" id="mcps1.1.4.1.2"><p id="p24945412"><a name="p24945412"></a><a name="p24945412"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="46.30463046304631%" id="mcps1.1.4.1.3"><p id="p7312526"><a name="p7312526"></a><a name="p7312526"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row55443761"><td class="cellrowborder" valign="top" width="29.68296829682968%" headers="mcps1.1.4.1.1 "><p id="p61759636"><a name="p61759636"></a><a name="p61759636"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.012401240124014%" headers="mcps1.1.4.1.2 "><p id="p36474591"><a name="p36474591"></a><a name="p36474591"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.30463046304631%" headers="mcps1.1.4.1.3 "><p id="p1651899"><a name="p1651899"></a><a name="p1651899"></a>项目ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section49614245"></a>

无

## 响应<a name="section43875021"></a>

-   响应参数

    <a name="zh-cn_topic_0020235137_table43541335201910"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235137_row45002232201910"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235137_p21302142201910"><a name="zh-cn_topic_0020235137_p21302142201910"></a><a name="zh-cn_topic_0020235137_p21302142201910"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235137_p523569515640"><a name="zh-cn_topic_0020235137_p523569515640"></a><a name="zh-cn_topic_0020235137_p523569515640"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235137_p42702004201910"><a name="zh-cn_topic_0020235137_p42702004201910"></a><a name="zh-cn_topic_0020235137_p42702004201910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235137_row3638641516742"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p6161852216742"><a name="zh-cn_topic_0020235137_p6161852216742"></a><a name="zh-cn_topic_0020235137_p6161852216742"></a>availabilityZoneInfo</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p2504439816742"><a name="zh-cn_topic_0020235137_p2504439816742"></a><a name="zh-cn_topic_0020235137_p2504439816742"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p3379652616742"><a name="zh-cn_topic_0020235137_p3379652616742"></a><a name="zh-cn_topic_0020235137_p3379652616742"></a>查询请求返回的可用分区列表。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235137_row36310324201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p55455149201910"><a name="zh-cn_topic_0020235137_p55455149201910"></a><a name="zh-cn_topic_0020235137_p55455149201910"></a>zoneState</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p2143812515640"><a name="zh-cn_topic_0020235137_p2143812515640"></a><a name="zh-cn_topic_0020235137_p2143812515640"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p44081575201910"><a name="zh-cn_topic_0020235137_p44081575201910"></a><a name="zh-cn_topic_0020235137_p44081575201910"></a>可用分区的状态。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235137_row61189858201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p57431491201910"><a name="zh-cn_topic_0020235137_p57431491201910"></a><a name="zh-cn_topic_0020235137_p57431491201910"></a>zoneName</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p5876653115640"><a name="zh-cn_topic_0020235137_p5876653115640"></a><a name="zh-cn_topic_0020235137_p5876653115640"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p58856323201910"><a name="zh-cn_topic_0020235137_p58856323201910"></a><a name="zh-cn_topic_0020235137_p58856323201910"></a>可用分区的名字。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235137_row40412735222822"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p11764098222825"><a name="zh-cn_topic_0020235137_p11764098222825"></a><a name="zh-cn_topic_0020235137_p11764098222825"></a>available</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p13367842222825"><a name="zh-cn_topic_0020235137_p13367842222825"></a><a name="zh-cn_topic_0020235137_p13367842222825"></a>boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p62236015222825"><a name="zh-cn_topic_0020235137_p62236015222825"></a><a name="zh-cn_topic_0020235137_p62236015222825"></a>可用分区是否可用。（true表示可用，false表示不可用）</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235137_row59944866201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p23695941201910"><a name="zh-cn_topic_0020235137_p23695941201910"></a><a name="zh-cn_topic_0020235137_p23695941201910"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p6246857015640"><a name="zh-cn_topic_0020235137_p6246857015640"></a><a name="zh-cn_topic_0020235137_p6246857015640"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p44946143201910"><a name="zh-cn_topic_0020235137_p44946143201910"></a><a name="zh-cn_topic_0020235137_p44946143201910"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235137_row1862105201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235137_p16612810201910"><a name="zh-cn_topic_0020235137_p16612810201910"></a><a name="zh-cn_topic_0020235137_p16612810201910"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235137_p2678940115640"><a name="zh-cn_topic_0020235137_p2678940115640"></a><a name="zh-cn_topic_0020235137_p2678940115640"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235137_p11851696201910"><a name="zh-cn_topic_0020235137_p11851696201910"></a><a name="zh-cn_topic_0020235137_p11851696201910"></a>出现错误时，返回的错误码，具体含义参考下面的返回值列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "availabilityZoneInfo": [
            {
                "zoneState": {
                    "available": true
                }, 
                "zoneName": "az1.dc1"
            }
        ]
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


## 返回值<a name="section59330872"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

