# 将云硬盘导出为镜像<a name="ZH-CN_TOPIC_0114215954"></a>

## 功能介绍<a name="section54187005111229"></a>

将系统盘或数据盘的数据导出为IMS镜像，导出的镜像在IMS的私有镜像列表中可以查看并使用。

## URI<a name="section44750704111229"></a>

-   URI格式

    POST /v3/\{project\_id\}/volumes/\{volume\_id\}/action

-   参数说明

    <a name="table16835088111229"></a>
    <table><thead align="left"><tr id="row36762725111229"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.4.1.1"><p id="p24990771111229"><a name="p24990771111229"></a><a name="p24990771111229"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.4.1.2"><p id="p10986545111229"><a name="p10986545111229"></a><a name="p10986545111229"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44%" id="mcps1.1.4.1.3"><p id="p17494919111229"><a name="p17494919111229"></a><a name="p17494919111229"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row7802334111229"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.1 "><p id="p28009309111229"><a name="p28009309111229"></a><a name="p28009309111229"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.2 "><p id="p54161581111229"><a name="p54161581111229"></a><a name="p54161581111229"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.1.4.1.3 "><p id="p25011958111229"><a name="p25011958111229"></a><a name="p25011958111229"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row22284688111229"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.1 "><p id="p60229298111229"><a name="p60229298111229"></a><a name="p60229298111229"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.4.1.2 "><p id="p46734956111229"><a name="p46734956111229"></a><a name="p46734956111229"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44%" headers="mcps1.1.4.1.3 "><p id="p27435111111229"><a name="p27435111111229"></a><a name="p27435111111229"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section2478043111340"></a>

-   请求参数

    <a name="zh-cn_topic_0094104100_table28675530111340"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0094104100_row30444615111340"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0094104100_p50094757111340"><a name="zh-cn_topic_0094104100_p50094757111340"></a><a name="zh-cn_topic_0094104100_p50094757111340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0094104100_p31143556111340"><a name="zh-cn_topic_0094104100_p31143556111340"></a><a name="zh-cn_topic_0094104100_p31143556111340"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0094104100_p39600140111340"><a name="zh-cn_topic_0094104100_p39600140111340"></a><a name="zh-cn_topic_0094104100_p39600140111340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0094104100_p53494756111340"><a name="zh-cn_topic_0094104100_p53494756111340"></a><a name="zh-cn_topic_0094104100_p53494756111340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0094104100_row38107956111340"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p66845605111340"><a name="zh-cn_topic_0094104100_p66845605111340"></a><a name="zh-cn_topic_0094104100_p66845605111340"></a>os-volume_upload_image</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p45784926111340"><a name="zh-cn_topic_0094104100_p45784926111340"></a><a name="zh-cn_topic_0094104100_p45784926111340"></a>map&lt;string,  map&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p17591560111340"><a name="zh-cn_topic_0094104100_p17591560111340"></a><a name="zh-cn_topic_0094104100_p17591560111340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p15630283111340"><a name="zh-cn_topic_0094104100_p15630283111340"></a><a name="zh-cn_topic_0094104100_p15630283111340"></a>标记将云硬盘导出为镜像的操作。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   os-volume\_upload\_image参数说明

    <a name="zh-cn_topic_0094104100_table1029161111454"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0094104100_row17873550111454"><th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0094104100_p61357386111454"><a name="zh-cn_topic_0094104100_p61357386111454"></a><a name="zh-cn_topic_0094104100_p61357386111454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0094104100_p3892401111454"><a name="zh-cn_topic_0094104100_p3892401111454"></a><a name="zh-cn_topic_0094104100_p3892401111454"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0094104100_p46849027111454"><a name="zh-cn_topic_0094104100_p46849027111454"></a><a name="zh-cn_topic_0094104100_p46849027111454"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0094104100_p36674858111454"><a name="zh-cn_topic_0094104100_p36674858111454"></a><a name="zh-cn_topic_0094104100_p36674858111454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0094104100_row34643012111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p38471446111454"><a name="zh-cn_topic_0094104100_p38471446111454"></a><a name="zh-cn_topic_0094104100_p38471446111454"></a>disk_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p29179435111454"><a name="zh-cn_topic_0094104100_p29179435111454"></a><a name="zh-cn_topic_0094104100_p29179435111454"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p14724020111454"><a name="zh-cn_topic_0094104100_p14724020111454"></a><a name="zh-cn_topic_0094104100_p14724020111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p51794970111454"><a name="zh-cn_topic_0094104100_p51794970111454"></a><a name="zh-cn_topic_0094104100_p51794970111454"></a>云硬盘导出镜像的格式。默认值是“vhd”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row65355785111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p43351654111454"><a name="zh-cn_topic_0094104100_p43351654111454"></a><a name="zh-cn_topic_0094104100_p43351654111454"></a>image_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p21823090111454"><a name="zh-cn_topic_0094104100_p21823090111454"></a><a name="zh-cn_topic_0094104100_p21823090111454"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p22839862111454"><a name="zh-cn_topic_0094104100_p22839862111454"></a><a name="zh-cn_topic_0094104100_p22839862111454"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p38089563111454"><a name="zh-cn_topic_0094104100_p38089563111454"></a><a name="zh-cn_topic_0094104100_p38089563111454"></a>云硬盘导出镜像的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row28028525111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p51331154111454"><a name="zh-cn_topic_0094104100_p51331154111454"></a><a name="zh-cn_topic_0094104100_p51331154111454"></a>force</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p64182815111454"><a name="zh-cn_topic_0094104100_p64182815111454"></a><a name="zh-cn_topic_0094104100_p64182815111454"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p31425545111454"><a name="zh-cn_topic_0094104100_p31425545111454"></a><a name="zh-cn_topic_0094104100_p31425545111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p62441207111454"><a name="zh-cn_topic_0094104100_p62441207111454"></a><a name="zh-cn_topic_0094104100_p62441207111454"></a>强制导出镜像的标示，默认值是false。</p>
    <a name="zh-cn_topic_0094104100_ul24573010111454"></a><a name="zh-cn_topic_0094104100_ul24573010111454"></a><ul id="zh-cn_topic_0094104100_ul24573010111454"><li>当force标记为false时，云硬盘处于正在使用状态时，不能强制导出镜像。</li></ul>
    <a name="zh-cn_topic_0094104100_ul44256769111454"></a><a name="zh-cn_topic_0094104100_ul44256769111454"></a><ul id="zh-cn_topic_0094104100_ul44256769111454"><li>当force标记为true时，即使云硬盘处于正在使用状态时，仍可以导出镜像。</li></ul>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row43451869111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p50930133111454"><a name="zh-cn_topic_0094104100_p50930133111454"></a><a name="zh-cn_topic_0094104100_p50930133111454"></a>container_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p31700070111454"><a name="zh-cn_topic_0094104100_p31700070111454"></a><a name="zh-cn_topic_0094104100_p31700070111454"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p17568872111454"><a name="zh-cn_topic_0094104100_p17568872111454"></a><a name="zh-cn_topic_0094104100_p17568872111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p13792514111454"><a name="zh-cn_topic_0094104100_p13792514111454"></a><a name="zh-cn_topic_0094104100_p13792514111454"></a>云硬盘导出镜像的容器类型，默认值是“bare”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row148648415911"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0094104100_p846811317910"><a name="zh-cn_topic_0094104100_p846811317910"></a><a name="zh-cn_topic_0094104100_p846811317910"></a>__os_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0094104100_p946810131899"><a name="zh-cn_topic_0094104100_p946810131899"></a><a name="zh-cn_topic_0094104100_p946810131899"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0094104100_p12469713496"><a name="zh-cn_topic_0094104100_p12469713496"></a><a name="zh-cn_topic_0094104100_p12469713496"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0094104100_p246912131294"><a name="zh-cn_topic_0094104100_p246912131294"></a><a name="zh-cn_topic_0094104100_p246912131294"></a>云硬盘导出镜像的系统类型。目前只支持“windows”和“linux”，默认值是“linux”。</p>
    <div class="note" id="zh-cn_topic_0094104100_note18753145612918"><a name="zh-cn_topic_0094104100_note18753145612918"></a><a name="zh-cn_topic_0094104100_note18753145612918"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="zh-cn_topic_0094104100_ul198423111019"></a><a name="zh-cn_topic_0094104100_ul198423111019"></a><ul id="zh-cn_topic_0094104100_ul198423111019"><li>参数名“os”前面为两个“_”，“os”后面为一个“_”。</li><li>只有云硬盘的volume_image_metadata信息中无“__os_type”字段且云硬盘状态为“available”时，设置的__os_type才会生效。</li><li>如果不传递该参数，则使用默认的“linux”值作为镜像的系统类型。</li></ul>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "os-volume_upload_image": {
            "image_name": "sxmatch2", 
            "force": true, 
            "container_format": "bare", 
            "disk_format": "vhd",
            "__os_type": "linux"
        }
    }
    ```


## 响应<a name="section5535081111830"></a>

-   响应参数

    <a name="zh-cn_topic_0094104100_table9775027111830"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0094104100_row50835692111830"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0094104100_p24050370111830"><a name="zh-cn_topic_0094104100_p24050370111830"></a><a name="zh-cn_topic_0094104100_p24050370111830"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0094104100_p1922990111830"><a name="zh-cn_topic_0094104100_p1922990111830"></a><a name="zh-cn_topic_0094104100_p1922990111830"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0094104100_p271585111830"><a name="zh-cn_topic_0094104100_p271585111830"></a><a name="zh-cn_topic_0094104100_p271585111830"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0094104100_row21998458111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p37044679111830"><a name="zh-cn_topic_0094104100_p37044679111830"></a><a name="zh-cn_topic_0094104100_p37044679111830"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p47829041111830"><a name="zh-cn_topic_0094104100_p47829041111830"></a><a name="zh-cn_topic_0094104100_p47829041111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p5292410111830"><a name="zh-cn_topic_0094104100_p5292410111830"></a><a name="zh-cn_topic_0094104100_p5292410111830"></a>云硬盘导出镜像后的状态，正常值为“uploading”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row47631691111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p32961780111830"><a name="zh-cn_topic_0094104100_p32961780111830"></a><a name="zh-cn_topic_0094104100_p32961780111830"></a>image_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p52658493111830"><a name="zh-cn_topic_0094104100_p52658493111830"></a><a name="zh-cn_topic_0094104100_p52658493111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p15940816111830"><a name="zh-cn_topic_0094104100_p15940816111830"></a><a name="zh-cn_topic_0094104100_p15940816111830"></a>云硬盘导出镜像的ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row9249618111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p11021632111830"><a name="zh-cn_topic_0094104100_p11021632111830"></a><a name="zh-cn_topic_0094104100_p11021632111830"></a>image_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p20337010111830"><a name="zh-cn_topic_0094104100_p20337010111830"></a><a name="zh-cn_topic_0094104100_p20337010111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p18706116111830"><a name="zh-cn_topic_0094104100_p18706116111830"></a><a name="zh-cn_topic_0094104100_p18706116111830"></a>云硬盘导出镜像的名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row34137321111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p13659606111830"><a name="zh-cn_topic_0094104100_p13659606111830"></a><a name="zh-cn_topic_0094104100_p13659606111830"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p32686283111830"><a name="zh-cn_topic_0094104100_p32686283111830"></a><a name="zh-cn_topic_0094104100_p32686283111830"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p41886703111830"><a name="zh-cn_topic_0094104100_p41886703111830"></a><a name="zh-cn_topic_0094104100_p41886703111830"></a>云硬盘类型的信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row41436015111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p874086111830"><a name="zh-cn_topic_0094104100_p874086111830"></a><a name="zh-cn_topic_0094104100_p874086111830"></a>container_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p3692104111830"><a name="zh-cn_topic_0094104100_p3692104111830"></a><a name="zh-cn_topic_0094104100_p3692104111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p64707827111830"><a name="zh-cn_topic_0094104100_p64707827111830"></a><a name="zh-cn_topic_0094104100_p64707827111830"></a>云硬盘导出镜像的容器类型。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row45499535111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p61583720111830"><a name="zh-cn_topic_0094104100_p61583720111830"></a><a name="zh-cn_topic_0094104100_p61583720111830"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p22225458111830"><a name="zh-cn_topic_0094104100_p22225458111830"></a><a name="zh-cn_topic_0094104100_p22225458111830"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p60782776111830"><a name="zh-cn_topic_0094104100_p60782776111830"></a><a name="zh-cn_topic_0094104100_p60782776111830"></a>云硬盘容量。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row10174073111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p18793567111830"><a name="zh-cn_topic_0094104100_p18793567111830"></a><a name="zh-cn_topic_0094104100_p18793567111830"></a>disk_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p45883995111830"><a name="zh-cn_topic_0094104100_p45883995111830"></a><a name="zh-cn_topic_0094104100_p45883995111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p61636782111830"><a name="zh-cn_topic_0094104100_p61636782111830"></a><a name="zh-cn_topic_0094104100_p61636782111830"></a>云硬盘导出镜像的格式。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row17860134111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p37384724111830"><a name="zh-cn_topic_0094104100_p37384724111830"></a><a name="zh-cn_topic_0094104100_p37384724111830"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p8263770111830"><a name="zh-cn_topic_0094104100_p8263770111830"></a><a name="zh-cn_topic_0094104100_p8263770111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p61744912111830"><a name="zh-cn_topic_0094104100_p61744912111830"></a><a name="zh-cn_topic_0094104100_p61744912111830"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row18833303111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p49102550111830"><a name="zh-cn_topic_0094104100_p49102550111830"></a><a name="zh-cn_topic_0094104100_p49102550111830"></a>display_description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p17883602111830"><a name="zh-cn_topic_0094104100_p17883602111830"></a><a name="zh-cn_topic_0094104100_p17883602111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p28018462111830"><a name="zh-cn_topic_0094104100_p28018462111830"></a><a name="zh-cn_topic_0094104100_p28018462111830"></a>云硬盘描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row50839573111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p24364735111830"><a name="zh-cn_topic_0094104100_p24364735111830"></a><a name="zh-cn_topic_0094104100_p24364735111830"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p27386538111830"><a name="zh-cn_topic_0094104100_p27386538111830"></a><a name="zh-cn_topic_0094104100_p27386538111830"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p32651105111830"><a name="zh-cn_topic_0094104100_p32651105111830"></a><a name="zh-cn_topic_0094104100_p32651105111830"></a>云硬盘更新时间。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   volume\_type参数说明

    <a name="zh-cn_topic_0094104100_table58500796111957"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0094104100_row41681908111957"><th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0094104100_p20791387111957"><a name="zh-cn_topic_0094104100_p20791387111957"></a><a name="zh-cn_topic_0094104100_p20791387111957"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0094104100_p6380778111957"><a name="zh-cn_topic_0094104100_p6380778111957"></a><a name="zh-cn_topic_0094104100_p6380778111957"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0094104100_p55467427111957"><a name="zh-cn_topic_0094104100_p55467427111957"></a><a name="zh-cn_topic_0094104100_p55467427111957"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0094104100_row63676572111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p57528669111957"><a name="zh-cn_topic_0094104100_p57528669111957"></a><a name="zh-cn_topic_0094104100_p57528669111957"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p29310607111957"><a name="zh-cn_topic_0094104100_p29310607111957"></a><a name="zh-cn_topic_0094104100_p29310607111957"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p39999332111957"><a name="zh-cn_topic_0094104100_p39999332111957"></a><a name="zh-cn_topic_0094104100_p39999332111957"></a>云硬盘类型ID。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row24449673111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p34266520111957"><a name="zh-cn_topic_0094104100_p34266520111957"></a><a name="zh-cn_topic_0094104100_p34266520111957"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p24124731111957"><a name="zh-cn_topic_0094104100_p24124731111957"></a><a name="zh-cn_topic_0094104100_p24124731111957"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p39662687111957"><a name="zh-cn_topic_0094104100_p39662687111957"></a><a name="zh-cn_topic_0094104100_p39662687111957"></a>云硬盘类型名称。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row21419866111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p57287600111957"><a name="zh-cn_topic_0094104100_p57287600111957"></a><a name="zh-cn_topic_0094104100_p57287600111957"></a>deleted</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p9784030111957"><a name="zh-cn_topic_0094104100_p9784030111957"></a><a name="zh-cn_topic_0094104100_p9784030111957"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p36953317111957"><a name="zh-cn_topic_0094104100_p36953317111957"></a><a name="zh-cn_topic_0094104100_p36953317111957"></a>云硬盘类型是否被删除标识。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row64144399111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p28313846111957"><a name="zh-cn_topic_0094104100_p28313846111957"></a><a name="zh-cn_topic_0094104100_p28313846111957"></a>is_public</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p11720218111957"><a name="zh-cn_topic_0094104100_p11720218111957"></a><a name="zh-cn_topic_0094104100_p11720218111957"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p56704311111957"><a name="zh-cn_topic_0094104100_p56704311111957"></a><a name="zh-cn_topic_0094104100_p56704311111957"></a>云硬盘类型是否是public类型。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row40576753111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p65491588111957"><a name="zh-cn_topic_0094104100_p65491588111957"></a><a name="zh-cn_topic_0094104100_p65491588111957"></a>extra_spec</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p3218391111957"><a name="zh-cn_topic_0094104100_p3218391111957"></a><a name="zh-cn_topic_0094104100_p3218391111957"></a>map&lt;string, string&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p43680990111957"><a name="zh-cn_topic_0094104100_p43680990111957"></a><a name="zh-cn_topic_0094104100_p43680990111957"></a>云硬盘类型的规格。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row57584594111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p33840505111957"><a name="zh-cn_topic_0094104100_p33840505111957"></a><a name="zh-cn_topic_0094104100_p33840505111957"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p56726405111957"><a name="zh-cn_topic_0094104100_p56726405111957"></a><a name="zh-cn_topic_0094104100_p56726405111957"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p63298283111957"><a name="zh-cn_topic_0094104100_p63298283111957"></a><a name="zh-cn_topic_0094104100_p63298283111957"></a>云硬盘类型的描述信息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row32813641111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p40659264111957"><a name="zh-cn_topic_0094104100_p40659264111957"></a><a name="zh-cn_topic_0094104100_p40659264111957"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p5066079111957"><a name="zh-cn_topic_0094104100_p5066079111957"></a><a name="zh-cn_topic_0094104100_p5066079111957"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p19661880111957"><a name="zh-cn_topic_0094104100_p19661880111957"></a><a name="zh-cn_topic_0094104100_p19661880111957"></a>云硬盘类型的创建时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row42739193111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p39322569111957"><a name="zh-cn_topic_0094104100_p39322569111957"></a><a name="zh-cn_topic_0094104100_p39322569111957"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p31011493111957"><a name="zh-cn_topic_0094104100_p31011493111957"></a><a name="zh-cn_topic_0094104100_p31011493111957"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p59444132111957"><a name="zh-cn_topic_0094104100_p59444132111957"></a><a name="zh-cn_topic_0094104100_p59444132111957"></a>云硬盘类型的更新时间。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0094104100_row65235145111957"><td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0094104100_p49555405111957"><a name="zh-cn_topic_0094104100_p49555405111957"></a><a name="zh-cn_topic_0094104100_p49555405111957"></a>deleted_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0094104100_p54564832111957"><a name="zh-cn_topic_0094104100_p54564832111957"></a><a name="zh-cn_topic_0094104100_p54564832111957"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0094104100_p41188442111957"><a name="zh-cn_topic_0094104100_p41188442111957"></a><a name="zh-cn_topic_0094104100_p41188442111957"></a>云硬盘类型的删除时间。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   响应样例

    ```
    {
        "os-volume_upload_image": {
            "status": "uploading", 
            "size": 40, 
            "id": "16369c5d-384d-4e64-b37a-56d898769362", 
            "image_id": "c5333daa-fbc8-4d1d-bf79-b0567bb45d15", 
            "image_name": "evs-ims-test1027", 
            "volume_type": {
                "description": "None", 
                "deleted": false, 
                "created_at": "2015-05-24T14:47:22.132268", 
                "updated_at": "2017-07-29T11:29:33.730076", 
                "extra_specs": {
                    "volume_backend_name": "<or> FusionStorage_SATA <or> FusionStorage_SAS <or> fusionstoragesata", 
                    "XX:availability_zone": "kvmxen.dc1"
                }, 
                "is_public": true, 
                "deleted_at": null, 
                "id": "8247b6ed-37f0-4c48-8ef1-f0027fb332bc", 
                "name": "SATA"
            }, 
            "container_format": "bare", 
            "disk_format": "vhd", 
            "display_description": "", 
            "updated_at": "2018-01-11T01:50:25.800931"
        }
    }
    ```

    或者

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


## 返回值<a name="section28290342112319"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

