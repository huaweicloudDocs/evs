# 获取云硬盘资源的所有标签<a name="evs_04_2026"></a>

## 功能介绍<a name="section5299350116935"></a>

获取某个租户的云硬盘资源的所有标签。

## 接口约束<a name="section4466609116935"></a>

无

## URI<a name="section1378135716935"></a>

-   URI格式

    GET /v2/\{project\_id\}/cloudvolumes/tags

-   参数说明

    <a name="table5247312516935"></a>
    <table><thead align="left"><tr id="row1996914916935"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p688839816935"><a name="p688839816935"></a><a name="p688839816935"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p2108940416935"><a name="p2108940416935"></a><a name="p2108940416935"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p3052017416935"><a name="p3052017416935"></a><a name="p3052017416935"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5621505316935"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p5712544016935"><a name="p5712544016935"></a><a name="p5712544016935"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p6375793616935"><a name="p6375793616935"></a><a name="p6375793616935"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p6411917216935"><a name="p6411917216935"></a><a name="p6411917216935"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section5573802716935"></a>

无

## 响应消息<a name="section3215934016935"></a>

-   响应参数

    <a name="table716338716935"></a>
    <table><thead align="left"><tr id="row2937460716935"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="p3053299616935"><a name="p3053299616935"></a><a name="p3053299616935"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="p5725363416935"><a name="p5725363416935"></a><a name="p5725363416935"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p3278200616935"><a name="p3278200616935"></a><a name="p3278200616935"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row3809682916935"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p6594430016935"><a name="p6594430016935"></a><a name="p6594430016935"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p3988810816935"><a name="p3988810816935"></a><a name="p3988810816935"></a>tag_list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p4842047816935"><a name="p4842047816935"></a><a name="p4842047816935"></a>所有云硬盘的标签信息，请参见<a href="#li24152017161222">•tag_list 参数数据结构说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li24152017161222"></a>tag\_list 参数数据结构说明

    <a name="table16041561161222"></a>
    <table><thead align="left"><tr id="row54431449161222"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="p39942516161238"><a name="p39942516161238"></a><a name="p39942516161238"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="p14118386161238"><a name="p14118386161238"></a><a name="p14118386161238"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p20499366161238"><a name="p20499366161238"></a><a name="p20499366161238"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row62887839161222"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p60750213161222"><a name="p60750213161222"></a><a name="p60750213161222"></a>key-value</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="p21820227161222"><a name="p21820227161222"></a><a name="p21820227161222"></a>list&lt;String&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p25757443175931"><a name="p25757443175931"></a><a name="p25757443175931"></a>键值对。</p>
    <p id="p19308906161222"><a name="p19308906161222"></a><a name="p19308906161222"></a>键是 String类型，value 是 list&lt;String&gt;类型。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "tags": {
            "key_0": [
                "value_0"
            ], 
            "key_1": [
                "value_1", 
                "value_2", 
                "value_3", 
                "value_4"
            ]
        }
    }
    ```


## 状态码<a name="section6050296116935"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

