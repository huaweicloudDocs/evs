# 为指定云硬盘批量添加标签<a name="zh-cn_topic_0094910373"></a>

## 功能介绍<a name="section5299350116935"></a>

为指定云硬盘批量添加标签。

-   添加标签时，如果云硬盘的标签已存在相同key，则会覆盖已有标签。
-   单个云硬盘最多支持创建10个标签。

## 接口约束<a name="section4466609116935"></a>

无

## URI<a name="section1378135716935"></a>

-   URI格式

    POST /v2/\{project\_id\}/cloudvolumes/\{volume\_id\}/tags/action

-   参数说明

    <a name="table28484833104128"></a>
    <table><thead align="left"><tr id="row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p5384679104128"><a name="p5384679104128"></a><a name="p5384679104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.340000000000003%" id="mcps1.1.4.1.2"><p id="p33505894104128"><a name="p33505894104128"></a><a name="p33505894104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.09%" id="mcps1.1.4.1.3"><p id="p29622926104128"><a name="p29622926104128"></a><a name="p29622926104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50646790104128"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p16385142185226"><a name="p16385142185226"></a><a name="p16385142185226"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.340000000000003%" headers="mcps1.1.4.1.2 "><p id="p52128135185226"><a name="p52128135185226"></a><a name="p52128135185226"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.09%" headers="mcps1.1.4.1.3 "><p id="p50566709185232"><a name="p50566709185232"></a><a name="p50566709185232"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row40869685152038"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p66238361185240"><a name="p66238361185240"></a><a name="p66238361185240"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.340000000000003%" headers="mcps1.1.4.1.2 "><p id="p63707038185240"><a name="p63707038185240"></a><a name="p63707038185240"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.09%" headers="mcps1.1.4.1.3 "><p id="p42707547152038"><a name="p42707547152038"></a><a name="p42707547152038"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section5573802716935"></a>

-   请求参数

    <a name="table54577306"></a>
    <table><thead align="left"><tr id="row28922261"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="p61001774"><a name="p61001774"></a><a name="p61001774"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21%" id="mcps1.1.5.1.2"><p id="p42196623"><a name="p42196623"></a><a name="p42196623"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p62483297"><a name="p62483297"></a><a name="p62483297"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47%" id="mcps1.1.5.1.4"><p id="p27982283"><a name="p27982283"></a><a name="p27982283"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50513961"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p52260429185445"><a name="p52260429185445"></a><a name="p52260429185445"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="p5236376185445"><a name="p5236376185445"></a><a name="p5236376185445"></a>List&lt;resource_tag&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p21493324185445"><a name="p21493324185445"></a><a name="p21493324185445"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p63237647185445"><a name="p63237647185445"></a><a name="p63237647185445"></a>标签列表，请参见<a href="#li4495404118563">•resource_tag 参数数据结构说明</a>。</p>
    </td>
    </tr>
    <tr id="row5477191"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p63564655185445"><a name="p63564655185445"></a><a name="p63564655185445"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="p48463411185445"><a name="p48463411185445"></a><a name="p48463411185445"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p33222212185445"><a name="p33222212185445"></a><a name="p33222212185445"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p8076185185456"><a name="p8076185185456"></a><a name="p8076185185456"></a>操作标识，请注意使用小写字母。</p>
    <p id="p1055696513"><a name="p1055696513"></a><a name="p1055696513"></a>create：添加标签</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li4495404118563"></a>resource\_tag 参数数据结构说明

    <a name="table24916402185553"></a>
    <table><thead align="left"><tr id="row45194334185553"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="p36862455185553"><a name="p36862455185553"></a><a name="p36862455185553"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.2"><p id="p33068848185553"><a name="p33068848185553"></a><a name="p33068848185553"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p61330993185553"><a name="p61330993185553"></a><a name="p61330993185553"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47%" id="mcps1.1.5.1.4"><p id="p1754531185553"><a name="p1754531185553"></a><a name="p1754531185553"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7899309185553"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p27402824185630"><a name="p27402824185630"></a><a name="p27402824185630"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p5036281185630"><a name="p5036281185630"></a><a name="p5036281185630"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p5285618185630"><a name="p5285618185630"></a><a name="p5285618185630"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><div class="p" id="p5281357101813"><a name="p5281357101813"></a><a name="p5281357101813"></a>标签键。同一资源的key值不能重复。<a name="ul17970183916119"></a><a name="ul17970183916119"></a><ul id="ul17970183916119"><li>最大长度36个字符。</li><li>字符集：A-Z，a-z ， 0-9，‘-’，‘_’，UNICODE字符（\u4E00-\u9FFF）。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row55890127185553"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="p54294233185630"><a name="p54294233185630"></a><a name="p54294233185630"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.2 "><p id="p35756723185630"><a name="p35756723185630"></a><a name="p35756723185630"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p10613433185630"><a name="p10613433185630"></a><a name="p10613433185630"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><div class="p" id="p1647151518204"><a name="p1647151518204"></a><a name="p1647151518204"></a>标签值。<a name="ul44344813212"></a><a name="ul44344813212"></a><ul id="ul44344813212"><li>每个值最大长度43个字符，可以为空字符串。</li><li>字符集：A-Z，a-z ， 0-9，‘.’，‘-’，‘_’，UNICODE字符（\u4E00-\u9FFF）。</li></ul>
    </div>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "action": "create", 
        "tags": [
            {
                "key": "key1", 
                "value": "value1"
            }, 
            {
                "key": "key2", 
                "value": "value3"
            }
        ]
    }
    ```


## 响应消息<a name="section3215934016935"></a>

无

## 状态码<a name="section6050296116935"></a>

-   正常

    204


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

