# 为指定云硬盘批量删除标签<a name="evs_04_2029"></a>

## 功能介绍<a name="section5299350116935"></a>

为指定云硬盘批量删除标签。

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

    <a name="zh-cn_topic_0094910373_table54577306"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0094910373_row28922261"><th class="cellrowborder" valign="top" width="17%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0094910373_p61001774"><a name="zh-cn_topic_0094910373_p61001774"></a><a name="zh-cn_topic_0094910373_p61001774"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0094910373_p42196623"><a name="zh-cn_topic_0094910373_p42196623"></a><a name="zh-cn_topic_0094910373_p42196623"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0094910373_p62483297"><a name="zh-cn_topic_0094910373_p62483297"></a><a name="zh-cn_topic_0094910373_p62483297"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0094910373_p27982283"><a name="zh-cn_topic_0094910373_p27982283"></a><a name="zh-cn_topic_0094910373_p27982283"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0094910373_row50513961"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094910373_p52260429185445"><a name="zh-cn_topic_0094910373_p52260429185445"></a><a name="zh-cn_topic_0094910373_p52260429185445"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094910373_p5236376185445"><a name="zh-cn_topic_0094910373_p5236376185445"></a><a name="zh-cn_topic_0094910373_p5236376185445"></a>List&lt;resource_tag&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094910373_p21493324185445"><a name="zh-cn_topic_0094910373_p21493324185445"></a><a name="zh-cn_topic_0094910373_p21493324185445"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094910373_p63237647185445"><a name="zh-cn_topic_0094910373_p63237647185445"></a><a name="zh-cn_topic_0094910373_p63237647185445"></a>标签列表，请参见<a href="#li2051510427374">•resource_tag 参数数据结构说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094910373_row5477191"><td class="cellrowborder" valign="top" width="17%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094910373_p63564655185445"><a name="zh-cn_topic_0094910373_p63564655185445"></a><a name="zh-cn_topic_0094910373_p63564655185445"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094910373_p48463411185445"><a name="zh-cn_topic_0094910373_p48463411185445"></a><a name="zh-cn_topic_0094910373_p48463411185445"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094910373_p33222212185445"><a name="zh-cn_topic_0094910373_p33222212185445"></a><a name="zh-cn_topic_0094910373_p33222212185445"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094910373_p8076185185456"><a name="zh-cn_topic_0094910373_p8076185185456"></a><a name="zh-cn_topic_0094910373_p8076185185456"></a>操作标识，请注意使用小写字母。</p>
    <p id="p199258121833"><a name="p199258121833"></a><a name="p199258121833"></a>delete：删除标签</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li2051510427374"></a>resource\_tag 参数数据结构说明

    <a name="table251711423376"></a>
    <table><thead align="left"><tr id="row16518134283716"><th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.1"><p id="p75181742143717"><a name="p75181742143717"></a><a name="p75181742143717"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21%" id="mcps1.1.5.1.2"><p id="p2051804253715"><a name="p2051804253715"></a><a name="p2051804253715"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p1951816424370"><a name="p1951816424370"></a><a name="p1951816424370"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="47%" id="mcps1.1.5.1.4"><p id="p15181442193715"><a name="p15181442193715"></a><a name="p15181442193715"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row10520194220379"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p652074219372"><a name="p652074219372"></a><a name="p652074219372"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="p452094213376"><a name="p452094213376"></a><a name="p452094213376"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p13520174213710"><a name="p13520174213710"></a><a name="p13520174213710"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="47%" headers="mcps1.1.5.1.4 "><p id="p0755543174416"><a name="p0755543174416"></a><a name="p0755543174416"></a>标签键。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "action": "delete", 
        "tags": [
            {
                "key": "key1"
            }, 
            {
                "key": "key2"
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

