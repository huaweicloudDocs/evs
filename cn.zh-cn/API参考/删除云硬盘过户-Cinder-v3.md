# 删除云硬盘过户<a name="ZH-CN_TOPIC_0102728950"></a>

## 功能介绍<a name="zh-cn_topic_0092902034_section44805042171914"></a>

当云硬盘过户未被接受时，您可以删除云硬盘过户记录，接受后则无法执行删除操作。

## URI<a name="zh-cn_topic_0092887872_section21748494171940"></a>

-   URI格式

    DELETE /v3/\{project\_id\}/os-volume-transfer/\{transfer\_id\}

-   参数说明

    <a name="table5162674110529"></a>
    <table><thead align="left"><tr id="row4741724810529"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p1559190910529"><a name="p1559190910529"></a><a name="p1559190910529"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p5498513910529"><a name="p5498513910529"></a><a name="p5498513910529"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p2461124910529"><a name="p2461124910529"></a><a name="p2461124910529"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4735411910529"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p18428135952510"><a name="p18428135952510"></a><a name="p18428135952510"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p4344649310529"><a name="p4344649310529"></a><a name="p4344649310529"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p2950506910529"><a name="p2950506910529"></a><a name="p2950506910529"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row22943135111210"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p52246671151847"><a name="p52246671151847"></a><a name="p52246671151847"></a>transfer_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p4121938151847"><a name="p4121938151847"></a><a name="p4121938151847"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p65441533151847"><a name="p65441533151847"></a><a name="p65441533151847"></a>云硬盘过户记录ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="zh-cn_topic_0092902034_section3832507172056"></a>

无

## 响应<a name="zh-cn_topic_0092902034_section23586530172122"></a>

无

## 返回值<a name="zh-cn_topic_0092902034_section10353980172239"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

