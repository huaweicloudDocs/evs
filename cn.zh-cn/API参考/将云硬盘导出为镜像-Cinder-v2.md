# 将云硬盘导出为镜像<a name="evs_04_2086"></a>

## 功能介绍<a name="section54187005111229"></a>

将系统盘或数据盘的数据导出为IMS镜像，导出的镜像在IMS的私有镜像列表中可以查看并使用。

## 调试<a name="section16985133917353"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EVS&api=CinderExportToImage)中直接运行调试该接口。

## URI<a name="section44750704111229"></a>

-   URI格式

    POST /v2/\{project\_id\}/volumes/\{volume\_id\}/action

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
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
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


## 请求消息<a name="section2478043111340"></a>

-   请求参数

    <a name="table28675530111340"></a>
    <table><thead align="left"><tr id="row30444615111340"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p50094757111340"><a name="p50094757111340"></a><a name="p50094757111340"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p31143556111340"><a name="p31143556111340"></a><a name="p31143556111340"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p39600140111340"><a name="p39600140111340"></a><a name="p39600140111340"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p53494756111340"><a name="p53494756111340"></a><a name="p53494756111340"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row38107956111340"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p66845605111340"><a name="p66845605111340"></a><a name="p66845605111340"></a>os-volume_upload_image</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p45784926111340"><a name="p45784926111340"></a><a name="p45784926111340"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p17591560111340"><a name="p17591560111340"></a><a name="p17591560111340"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p15630283111340"><a name="p15630283111340"></a><a name="p15630283111340"></a>标记将云硬盘导出为镜像的操作，请参见<a href="#li49734540111454">•os-volume_upload_image参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li49734540111454"></a>os-volume\_upload\_image参数说明

    <a name="table1029161111454"></a>
    <table><thead align="left"><tr id="row17873550111454"><th class="cellrowborder" valign="top" width="19%" id="mcps1.1.5.1.1"><p id="p61357386111454"><a name="p61357386111454"></a><a name="p61357386111454"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p3892401111454"><a name="p3892401111454"></a><a name="p3892401111454"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15%" id="mcps1.1.5.1.3"><p id="p46849027111454"><a name="p46849027111454"></a><a name="p46849027111454"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p36674858111454"><a name="p36674858111454"></a><a name="p36674858111454"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row34643012111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="p38471446111454"><a name="p38471446111454"></a><a name="p38471446111454"></a>disk_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p29179435111454"><a name="p29179435111454"></a><a name="p29179435111454"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p14724020111454"><a name="p14724020111454"></a><a name="p14724020111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p846816504210"><a name="p846816504210"></a><a name="p846816504210"></a>云硬盘导出镜像的格式。</p>
    <p id="p51794970111454"><a name="p51794970111454"></a><a name="p51794970111454"></a>目前支持vhd、zvhd、zvhd2、raw、qcow2。默认是zvhd2。</p>
    </td>
    </tr>
    <tr id="row65355785111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="p43351654111454"><a name="p43351654111454"></a><a name="p43351654111454"></a>image_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p21823090111454"><a name="p21823090111454"></a><a name="p21823090111454"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p22839862111454"><a name="p22839862111454"></a><a name="p22839862111454"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><div class="p" id="p38089563111454"><a name="p38089563111454"></a><a name="p38089563111454"></a>云硬盘导出镜像的名称。<a name="ul728185834617"></a><a name="ul728185834617"></a><ul id="ul728185834617"><li>名称的首尾字母不能为空格。</li><li>名称的长度范围为1～128位。</li><li>名称包含以下字符：大写字母、小写字母、中文、数字、特殊字符包含“-”、“.”、“_”和空格。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row28028525111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="p51331154111454"><a name="p51331154111454"></a><a name="p51331154111454"></a>force</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p64182815111454"><a name="p64182815111454"></a><a name="p64182815111454"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p31425545111454"><a name="p31425545111454"></a><a name="p31425545111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p62441207111454"><a name="p62441207111454"></a><a name="p62441207111454"></a>强制导出镜像的标示，默认值是false。</p>
    <a name="ul24573010111454"></a><a name="ul24573010111454"></a><ul id="ul24573010111454"><li>当force标记为false时，云硬盘处于正在使用状态时，不能强制导出镜像。</li></ul>
    <a name="ul44256769111454"></a><a name="ul44256769111454"></a><ul id="ul44256769111454"><li>当force标记为true时，即使云硬盘处于正在使用状态时，仍可以导出镜像。</li></ul>
    </td>
    </tr>
    <tr id="row43451869111454"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="p50930133111454"><a name="p50930133111454"></a><a name="p50930133111454"></a>container_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p31700070111454"><a name="p31700070111454"></a><a name="p31700070111454"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p17568872111454"><a name="p17568872111454"></a><a name="p17568872111454"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p18456652114510"><a name="p18456652114510"></a><a name="p18456652114510"></a>云硬盘导出镜像的容器类型。</p>
    <p id="p13792514111454"><a name="p13792514111454"></a><a name="p13792514111454"></a>目前支持ami、ari、aki、ovf、bare。默认是bare。</p>
    </td>
    </tr>
    <tr id="row148648415911"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.1.5.1.1 "><p id="p846811317910"><a name="p846811317910"></a><a name="p846811317910"></a>__os_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p946810131899"><a name="p946810131899"></a><a name="p946810131899"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15%" headers="mcps1.1.5.1.3 "><p id="p12469713496"><a name="p12469713496"></a><a name="p12469713496"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p246912131294"><a name="p246912131294"></a><a name="p246912131294"></a>云硬盘导出镜像的系统类型。目前只支持“windows”和“linux”，默认值是“linux”。</p>
    <div class="note" id="note18753145612918"><a name="note18753145612918"></a><a name="note18753145612918"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul198423111019"></a><a name="ul198423111019"></a><ul id="ul198423111019"><li>参数名“os”前面为两个“_”，“os”后面为一个“_”。</li><li>只有云硬盘的volume_image_metadata信息中无“__os_type”字段且云硬盘状态为“available”时，设置的__os_type才会生效。</li><li>如果不传递该参数，则使用默认的“linux”值作为镜像的系统类型。</li></ul>
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


## 响应消息<a name="section5535081111830"></a>

-   响应参数

    <a name="table5532594121252"></a>
    <table><thead align="left"><tr id="row60048709121252"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p32107236121252"><a name="p32107236121252"></a><a name="p32107236121252"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p50549312121252"><a name="p50549312121252"></a><a name="p50549312121252"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p2030156121252"><a name="p2030156121252"></a><a name="p2030156121252"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1599615332144"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p799653310145"><a name="p799653310145"></a><a name="p799653310145"></a>os-volume_upload_image</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p499603310144"><a name="p499603310144"></a><a name="p499603310144"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p159971233141420"><a name="p159971233141420"></a><a name="p159971233141420"></a>标记将云硬盘导出为镜像的操作，请参见<a href="#li8542654111830">•os-volume_upload_image参...</a>。</p>
    </td>
    </tr>
    <tr id="row30224973121252"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li8542654111830"></a>os-volume\_upload\_image参数说明

    <a name="table9775027111830"></a>
    <table><thead align="left"><tr id="row50835692111830"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p24050370111830"><a name="p24050370111830"></a><a name="p24050370111830"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p1922990111830"><a name="p1922990111830"></a><a name="p1922990111830"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p271585111830"><a name="p271585111830"></a><a name="p271585111830"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row21998458111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p37044679111830"><a name="p37044679111830"></a><a name="p37044679111830"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p47829041111830"><a name="p47829041111830"></a><a name="p47829041111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p5292410111830"><a name="p5292410111830"></a><a name="p5292410111830"></a>云硬盘导出镜像后的状态，正常值为“uploading”。</p>
    </td>
    </tr>
    <tr id="row47631691111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p32961780111830"><a name="p32961780111830"></a><a name="p32961780111830"></a>image_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p52658493111830"><a name="p52658493111830"></a><a name="p52658493111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p15940816111830"><a name="p15940816111830"></a><a name="p15940816111830"></a>云硬盘导出镜像的ID。</p>
    </td>
    </tr>
    <tr id="row9249618111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p11021632111830"><a name="p11021632111830"></a><a name="p11021632111830"></a>image_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p20337010111830"><a name="p20337010111830"></a><a name="p20337010111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p18706116111830"><a name="p18706116111830"></a><a name="p18706116111830"></a>云硬盘导出镜像的名称。</p>
    </td>
    </tr>
    <tr id="row34137321111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p13659606111830"><a name="p13659606111830"></a><a name="p13659606111830"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p32686283111830"><a name="p32686283111830"></a><a name="p32686283111830"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p41886703111830"><a name="p41886703111830"></a><a name="p41886703111830"></a>云硬盘类型的信息，请参见<a href="#li28869709111957">•volume_type参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row41436015111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p874086111830"><a name="p874086111830"></a><a name="p874086111830"></a>container_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p3692104111830"><a name="p3692104111830"></a><a name="p3692104111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p64707827111830"><a name="p64707827111830"></a><a name="p64707827111830"></a>云硬盘导出镜像的容器类型。</p>
    <p id="p1432717114914"><a name="p1432717114914"></a><a name="p1432717114914"></a>目前支持ami、ari、aki、ovf、bare。默认是bare。</p>
    </td>
    </tr>
    <tr id="row45499535111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p61583720111830"><a name="p61583720111830"></a><a name="p61583720111830"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p22225458111830"><a name="p22225458111830"></a><a name="p22225458111830"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p60782776111830"><a name="p60782776111830"></a><a name="p60782776111830"></a>云硬盘容量，单位为GB。</p>
    </td>
    </tr>
    <tr id="row10174073111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p18793567111830"><a name="p18793567111830"></a><a name="p18793567111830"></a>disk_format</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p45883995111830"><a name="p45883995111830"></a><a name="p45883995111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p61636782111830"><a name="p61636782111830"></a><a name="p61636782111830"></a>云硬盘导出镜像的格式。</p>
    <p id="p110543734915"><a name="p110543734915"></a><a name="p110543734915"></a>目前支持vhd、zvhd、zvhd2、raw、qcow2。默认是vhd。</p>
    </td>
    </tr>
    <tr id="row17860134111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p37384724111830"><a name="p37384724111830"></a><a name="p37384724111830"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p8263770111830"><a name="p8263770111830"></a><a name="p8263770111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p61744912111830"><a name="p61744912111830"></a><a name="p61744912111830"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row18833303111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p49102550111830"><a name="p49102550111830"></a><a name="p49102550111830"></a>display_description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p17883602111830"><a name="p17883602111830"></a><a name="p17883602111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p28018462111830"><a name="p28018462111830"></a><a name="p28018462111830"></a>云硬盘描述信息。</p>
    </td>
    </tr>
    <tr id="row50839573111830"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p24364735111830"><a name="p24364735111830"></a><a name="p24364735111830"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p27386538111830"><a name="p27386538111830"></a><a name="p27386538111830"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p32651105111830"><a name="p32651105111830"></a><a name="p32651105111830"></a>云硬盘更新时间。</p>
    <p id="p22151829479"><a name="p22151829479"></a><a name="p22151829479"></a><span id="text982374294912"><a name="text982374294912"></a><a name="text982374294912"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li28869709111957"></a>volume\_type参数说明

    <a name="table58500796111957"></a>
    <table><thead align="left"><tr id="row41681908111957"><th class="cellrowborder" valign="top" width="22.38%" id="mcps1.1.4.1.1"><p id="p20791387111957"><a name="p20791387111957"></a><a name="p20791387111957"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.15%" id="mcps1.1.4.1.2"><p id="p6380778111957"><a name="p6380778111957"></a><a name="p6380778111957"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="p55467427111957"><a name="p55467427111957"></a><a name="p55467427111957"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row63676572111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p57528669111957"><a name="p57528669111957"></a><a name="p57528669111957"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p29310607111957"><a name="p29310607111957"></a><a name="p29310607111957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p39999332111957"><a name="p39999332111957"></a><a name="p39999332111957"></a>云硬盘类型ID。</p>
    </td>
    </tr>
    <tr id="row24449673111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p34266520111957"><a name="p34266520111957"></a><a name="p34266520111957"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p24124731111957"><a name="p24124731111957"></a><a name="p24124731111957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p39662687111957"><a name="p39662687111957"></a><a name="p39662687111957"></a>云硬盘类型名称。</p>
    </td>
    </tr>
    <tr id="row21419866111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p57287600111957"><a name="p57287600111957"></a><a name="p57287600111957"></a>deleted</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p9784030111957"><a name="p9784030111957"></a><a name="p9784030111957"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p36953317111957"><a name="p36953317111957"></a><a name="p36953317111957"></a>云硬盘类型是否被删除标识。</p>
    </td>
    </tr>
    <tr id="row64144399111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p28313846111957"><a name="p28313846111957"></a><a name="p28313846111957"></a>is_public</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p11720218111957"><a name="p11720218111957"></a><a name="p11720218111957"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p56704311111957"><a name="p56704311111957"></a><a name="p56704311111957"></a><span id="text10706161911492"><a name="text10706161911492"></a><a name="text10706161911492"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="row40576753111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p65491588111957"><a name="p65491588111957"></a><a name="p65491588111957"></a>extra_spec</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p3218391111957"><a name="p3218391111957"></a><a name="p3218391111957"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p43680990111957"><a name="p43680990111957"></a><a name="p43680990111957"></a>云硬盘类型的规格，请参见<a href="#li105361616191716">•extra_specs参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row57584594111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p33840505111957"><a name="p33840505111957"></a><a name="p33840505111957"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p56726405111957"><a name="p56726405111957"></a><a name="p56726405111957"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p63298283111957"><a name="p63298283111957"></a><a name="p63298283111957"></a>云硬盘类型的描述信息。</p>
    </td>
    </tr>
    <tr id="row32813641111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p40659264111957"><a name="p40659264111957"></a><a name="p40659264111957"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p5066079111957"><a name="p5066079111957"></a><a name="p5066079111957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p19661880111957"><a name="p19661880111957"></a><a name="p19661880111957"></a>云硬盘类型的创建时间。</p>
    <p id="p1176814616477"><a name="p1176814616477"></a><a name="p1176814616477"></a><span id="text62451486493"><a name="text62451486493"></a><a name="text62451486493"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row42739193111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p39322569111957"><a name="p39322569111957"></a><a name="p39322569111957"></a>updated_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p31011493111957"><a name="p31011493111957"></a><a name="p31011493111957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p59444132111957"><a name="p59444132111957"></a><a name="p59444132111957"></a>云硬盘类型的更新时间。</p>
    <p id="p12839783477"><a name="p12839783477"></a><a name="p12839783477"></a><span id="text23111349184911"><a name="text23111349184911"></a><a name="text23111349184911"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row65235145111957"><td class="cellrowborder" valign="top" width="22.38%" headers="mcps1.1.4.1.1 "><p id="p49555405111957"><a name="p49555405111957"></a><a name="p49555405111957"></a>deleted_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.4.1.2 "><p id="p54564832111957"><a name="p54564832111957"></a><a name="p54564832111957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p41188442111957"><a name="p41188442111957"></a><a name="p41188442111957"></a>云硬盘类型的删除时间。</p>
    <p id="p1971441016471"><a name="p1971441016471"></a><a name="p1971441016471"></a><span id="text112018513495"><a name="text112018513495"></a><a name="text112018513495"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li105361616191716"></a>extra\_specs参数说明

    <a name="evs_04_2071_table1763545695210"></a>
    <table><thead align="left"><tr id="evs_04_2071_row16361656165213"><th class="cellrowborder" valign="top" width="21.45%" id="mcps1.1.4.1.1"><p id="evs_04_2071_p1763619566527"><a name="evs_04_2071_p1763619566527"></a><a name="evs_04_2071_p1763619566527"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.41%" id="mcps1.1.4.1.2"><p id="evs_04_2071_p18636105619529"><a name="evs_04_2071_p18636105619529"></a><a name="evs_04_2071_p18636105619529"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2071_p186361556155214"><a name="evs_04_2071_p186361556155214"></a><a name="evs_04_2071_p186361556155214"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2071_row56365565526"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p063625610529"><a name="evs_04_2071_p063625610529"></a><a name="evs_04_2071_p063625610529"></a>volume_backend_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p3636165635219"><a name="evs_04_2071_p3636165635219"></a><a name="evs_04_2071_p3636165635219"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p17636185614527"><a name="evs_04_2071_p17636185614527"></a><a name="evs_04_2071_p17636185614527"></a><span id="evs_04_2071_text205233101097"><a name="evs_04_2071_text205233101097"></a><a name="evs_04_2071_text205233101097"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row156362568523"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p863675695214"><a name="evs_04_2071_p863675695214"></a><a name="evs_04_2071_p863675695214"></a>availability-zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p8636175665214"><a name="evs_04_2071_p8636175665214"></a><a name="evs_04_2071_p8636175665214"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p18636356185213"><a name="evs_04_2071_p18636356185213"></a><a name="evs_04_2071_p18636356185213"></a><span id="evs_04_2071_text533914121390"><a name="evs_04_2071_text533914121390"></a><a name="evs_04_2071_text533914121390"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row17844276596"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p178418274593"><a name="evs_04_2071_p178418274593"></a><a name="evs_04_2071_p178418274593"></a>HW:availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p168416276599"><a name="evs_04_2071_p168416276599"></a><a name="evs_04_2071_p168416276599"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p1540410211408"><a name="evs_04_2071_p1540410211408"></a><a name="evs_04_2071_p1540410211408"></a><span id="evs_04_2071_evs_04_2071_text533914121390"><a name="evs_04_2071_evs_04_2071_text533914121390"></a><a name="evs_04_2071_evs_04_2071_text533914121390"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2071_row3637135611527"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p163710561529"><a name="evs_04_2071_p163710561529"></a><a name="evs_04_2071_p163710561529"></a>RESKEY:availability_zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p166374562525"><a name="evs_04_2071_p166374562525"></a><a name="evs_04_2071_p166374562525"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p3637756205214"><a name="evs_04_2071_p3637756205214"></a><a name="evs_04_2071_p3637756205214"></a>支持当前云硬盘类型的AZ列表。</p>
    </td>
    </tr>
    <tr id="evs_04_2071_row16371656175219"><td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.1.4.1.1 "><p id="evs_04_2071_p1363716565526"><a name="evs_04_2071_p1363716565526"></a><a name="evs_04_2071_p1363716565526"></a>os-vendor-extended:sold_out_availability_zones</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.41%" headers="mcps1.1.4.1.2 "><p id="evs_04_2071_p0637456155216"><a name="evs_04_2071_p0637456155216"></a><a name="evs_04_2071_p0637456155216"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2071_p1063725695214"><a name="evs_04_2071_p1063725695214"></a><a name="evs_04_2071_p1063725695214"></a>当前云硬盘类型售罄的AZ列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li0419202382514"></a>error参数说明

    <a name="evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2013_p19541716103019"><a name="evs_04_2013_p19541716103019"></a><a name="evs_04_2013_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2013_p39375186103019"><a name="evs_04_2013_p39375186103019"></a><a name="evs_04_2013_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2013_p38578950103019"><a name="evs_04_2013_p38578950103019"></a><a name="evs_04_2013_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p46815658103019"><a name="evs_04_2013_p46815658103019"></a><a name="evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p33971979103019"><a name="evs_04_2013_p33971979103019"></a><a name="evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p21623243103019"><a name="evs_04_2013_p21623243103019"></a><a name="evs_04_2013_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p59870541103019"><a name="evs_04_2013_p59870541103019"></a><a name="evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p17675690103019"><a name="evs_04_2013_p17675690103019"></a><a name="evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p6087468103019"><a name="evs_04_2013_p6087468103019"></a><a name="evs_04_2013_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="evs_04_2013_p54787218103019"><a name="evs_04_2013_p54787218103019"></a><a name="evs_04_2013_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码.md">错误码</a>。</p>
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
                    "volume_backend_name": "<or> iaas blockstorage_SATA <or> iaas blockstorage_SAS <or> iaas blockstoragesata", 
                    "XX:availability_zone": "az-dc-1"
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


## 状态码<a name="section28290342112319"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

