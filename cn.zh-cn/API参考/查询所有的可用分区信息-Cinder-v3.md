# 查询所有的可用分区信息<a name="evs_04_3045"></a>

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
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section49614245"></a>

-   请求样例：

    ```
    GET https://{endpoint}/v3/{project_id}/os-availability-zone
    ```


## 响应消息<a name="section43875021"></a>

-   响应参数

    <a name="evs_04_2081_table201437992512"></a>
    <table><thead align="left"><tr id="evs_04_2081_row1414420917255"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="evs_04_2081_p11144139152511"><a name="evs_04_2081_p11144139152511"></a><a name="evs_04_2081_p11144139152511"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="evs_04_2081_p1014419152512"><a name="evs_04_2081_p1014419152512"></a><a name="evs_04_2081_p1014419152512"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="evs_04_2081_p16144994250"><a name="evs_04_2081_p16144994250"></a><a name="evs_04_2081_p16144994250"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2081_row181446912510"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_p13144119162511"><a name="evs_04_2081_p13144119162511"></a><a name="evs_04_2081_p13144119162511"></a>availabilityZoneInfo</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_p214416911255"><a name="evs_04_2081_p214416911255"></a><a name="evs_04_2081_p214416911255"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_p01441910254"><a name="evs_04_2081_p01441910254"></a><a name="evs_04_2081_p01441910254"></a>查询请求返回的可用分区列表，请参见<a href="#evs_04_2081_li19751007201910">•availabilityZoneInfo参数说...</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2081_row6109186192812"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_p129522216412"><a name="evs_04_2081_p129522216412"></a><a name="evs_04_2081_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_p1595262111415"><a name="evs_04_2081_p1595262111415"></a><a name="evs_04_2081_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_p109527215417"><a name="evs_04_2081_p109527215417"></a><a name="evs_04_2081_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#evs_04_2081_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2081_li19751007201910"></a>availabilityZoneInfo参数说明

    <a name="evs_04_2081_table43541335201910"></a>
    <table><thead align="left"><tr id="evs_04_2081_row45002232201910"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="evs_04_2081_p21302142201910"><a name="evs_04_2081_p21302142201910"></a><a name="evs_04_2081_p21302142201910"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="evs_04_2081_p523569515640"><a name="evs_04_2081_p523569515640"></a><a name="evs_04_2081_p523569515640"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="evs_04_2081_p42702004201910"><a name="evs_04_2081_p42702004201910"></a><a name="evs_04_2081_p42702004201910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2081_row36310324201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_p55455149201910"><a name="evs_04_2081_p55455149201910"></a><a name="evs_04_2081_p55455149201910"></a>zoneState</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_p2143812515640"><a name="evs_04_2081_p2143812515640"></a><a name="evs_04_2081_p2143812515640"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_p44081575201910"><a name="evs_04_2081_p44081575201910"></a><a name="evs_04_2081_p44081575201910"></a>可用分区的状态，请参见<a href="#evs_04_2081_li11149334112511">•zoneState参数说明</a>。</p>
    </td>
    </tr>
    <tr id="evs_04_2081_row61189858201910"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_p57431491201910"><a name="evs_04_2081_p57431491201910"></a><a name="evs_04_2081_p57431491201910"></a>zoneName</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_p5876653115640"><a name="evs_04_2081_p5876653115640"></a><a name="evs_04_2081_p5876653115640"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_p58856323201910"><a name="evs_04_2081_p58856323201910"></a><a name="evs_04_2081_p58856323201910"></a>可用分区的名字。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2081_li11149334112511"></a>zoneState参数说明

    <a name="evs_04_2081_table915023482516"></a>
    <table><thead align="left"><tr id="evs_04_2081_row4150434152517"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="evs_04_2081_p1215093419253"><a name="evs_04_2081_p1215093419253"></a><a name="evs_04_2081_p1215093419253"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="evs_04_2081_p3150193412259"><a name="evs_04_2081_p3150193412259"></a><a name="evs_04_2081_p3150193412259"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="evs_04_2081_p1215014346259"><a name="evs_04_2081_p1215014346259"></a><a name="evs_04_2081_p1215014346259"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2081_row2150534192516"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_p115073413258"><a name="evs_04_2081_p115073413258"></a><a name="evs_04_2081_p115073413258"></a>available</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_p915013462516"><a name="evs_04_2081_p915013462516"></a><a name="evs_04_2081_p915013462516"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><div class="p" id="evs_04_2081_p171501234112510"><a name="evs_04_2081_p171501234112510"></a><a name="evs_04_2081_p171501234112510"></a>可用分区是否可用。<a name="evs_04_2081_ul315013410258"></a><a name="evs_04_2081_ul315013410258"></a><ul id="evs_04_2081_ul315013410258"><li>true表示可用</li><li>false表示不可用</li></ul>
    </div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2081_li0419202382514"></a>error参数说明

    <a name="evs_04_2081_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2081_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2081_evs_04_2013_p19541716103019"><a name="evs_04_2081_evs_04_2013_p19541716103019"></a><a name="evs_04_2081_evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2081_evs_04_2013_p39375186103019"><a name="evs_04_2081_evs_04_2013_p39375186103019"></a><a name="evs_04_2081_evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2081_evs_04_2013_p38578950103019"><a name="evs_04_2081_evs_04_2013_p38578950103019"></a><a name="evs_04_2081_evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2081_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_evs_04_2013_p46815658103019"><a name="evs_04_2081_evs_04_2013_p46815658103019"></a><a name="evs_04_2081_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_evs_04_2013_p33971979103019"><a name="evs_04_2081_evs_04_2013_p33971979103019"></a><a name="evs_04_2081_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_evs_04_2013_p21623243103019"><a name="evs_04_2081_evs_04_2013_p21623243103019"></a><a name="evs_04_2081_evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2081_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2081_evs_04_2013_p59870541103019"><a name="evs_04_2081_evs_04_2013_p59870541103019"></a><a name="evs_04_2081_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2081_evs_04_2013_p17675690103019"><a name="evs_04_2081_evs_04_2013_p17675690103019"></a><a name="evs_04_2081_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2081_evs_04_2013_p6087468103019"><a name="evs_04_2081_evs_04_2013_p6087468103019"></a><a name="evs_04_2081_evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2081_evs_04_2013_p54787218103019"><a name="evs_04_2081_evs_04_2013_p54787218103019"></a><a name="evs_04_2081_evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
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
                "zoneName": "az-dc-1"
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


## 状态码<a name="section59330872"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

