# 查询云硬盘标签<a name="evs_04_2031"></a>

## 功能介绍<a name="section5299350116935"></a>

查询指定云硬盘的标签信息。

## 接口约束<a name="section4466609116935"></a>

无

## URI<a name="section1378135716935"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudvolumes/\{volume\_id\}/tags

-   参数说明

    <a name="table28484833104128"></a>
    <table><thead align="left"><tr id="row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p5384679104128"><a name="p5384679104128"></a><a name="p5384679104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p33505894104128"><a name="p33505894104128"></a><a name="p33505894104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p29622926104128"><a name="p29622926104128"></a><a name="p29622926104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50646790104128"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p39499107192824"><a name="p39499107192824"></a><a name="p39499107192824"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p45311124192824"><a name="p45311124192824"></a><a name="p45311124192824"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p46322466192824"><a name="p46322466192824"></a><a name="p46322466192824"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row40869685152038"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p13319579192824"><a name="p13319579192824"></a><a name="p13319579192824"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p5144078192824"><a name="p5144078192824"></a><a name="p5144078192824"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p14017211192824"><a name="p14017211192824"></a><a name="p14017211192824"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section565234819217"></a>

无

## 响应消息<a name="section3215934016935"></a>

-   响应参数

    <a name="table716338716935"></a>
    <table><thead align="left"><tr id="row2937460716935"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.4.1.1"><p id="p3053299616935"><a name="p3053299616935"></a><a name="p3053299616935"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.53%" id="mcps1.1.4.1.2"><p id="p5725363416935"><a name="p5725363416935"></a><a name="p5725363416935"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="p3278200616935"><a name="p3278200616935"></a><a name="p3278200616935"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row63271571172633"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.4.1.1 "><p id="p4610476519311"><a name="p4610476519311"></a><a name="p4610476519311"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.53%" headers="mcps1.1.4.1.2 "><p id="p4349852319311"><a name="p4349852319311"></a><a name="p4349852319311"></a>List&lt;resource_tag&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p5468710519318"><a name="p5468710519318"></a><a name="p5468710519318"></a>标签列表，请参见<a href="#li8528152083214">•resource_tag 参数数据结构说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li8528152083214"></a>resource\_tag 参数数据结构说明

    <a name="table205290203323"></a>
    <table><thead align="left"><tr id="row13530142033210"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="p19530182011329"><a name="p19530182011329"></a><a name="p19530182011329"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="p20530120163211"><a name="p20530120163211"></a><a name="p20530120163211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.95%" id="mcps1.1.4.1.3"><p id="p18533172017325"><a name="p18533172017325"></a><a name="p18533172017325"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row253510208321"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p17535320203220"><a name="p17535320203220"></a><a name="p17535320203220"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p175351020123212"><a name="p175351020123212"></a><a name="p175351020123212"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.95%" headers="mcps1.1.4.1.3 "><p id="p118083133491"><a name="p118083133491"></a><a name="p118083133491"></a>标签键。</p>
    </td>
    </tr>
    <tr id="row853810204325"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p1053816201325"><a name="p1053816201325"></a><a name="p1053816201325"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p13538520153211"><a name="p13538520153211"></a><a name="p13538520153211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.95%" headers="mcps1.1.4.1.3 "><p id="p656419560501"><a name="p656419560501"></a><a name="p656419560501"></a>标签值。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "tags": [
            {
                "value": "value1", 
                "key": "key1"
            }, 
            {
                "value": "value2", 
                "key": "key2"
            }
        ]
    }
    ```


## 状态码<a name="section6050296116935"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

