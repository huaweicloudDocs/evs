# 扩容云硬盘<a name="evs_04_2004"></a>

## 功能介绍<a name="section4445458"></a>

本接口兼容“[扩容云硬盘（废弃）](扩容云硬盘（废弃）.md)”接口功能，同时支持对包周期的云硬盘进行扩容。支持企业项目授权功能。

在成功调用本接口扩容包周期云硬盘后：

-   如果您需要查看订单可用的优惠券，请参考[查询订单可用优惠券](https://support.huaweicloud.com/api-oce/zh-cn_topic_0092953630.html)。
-   如果您需要支付订单，请参考[支付包周期产品订单](https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html)。
-   如果您需要查询订单的资源开通详情，请参考[查询订单的资源开通详情](https://support.huaweicloud.com/api-oce/api_order_00001.html)。
-   如果您需要退订该包周期资源，请参考“[退订包周期资源](https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html)”。

## 接口约束<a name="section134617281249"></a>

-   扩容状态为available的云硬盘时，没有约束限制。
-   扩容状态为in-use的云硬盘时，有以下约束：
    -   不支持共享云硬盘，即multiattach参数值必须为false。
    -   云硬盘所挂载的云服务器状态必须为ACTIVE、PAUSED、SUSPENDED、SHUTOFF才支持扩容。


## 调试<a name="section168911230193913"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EVS&api=ResizeVolume)中直接运行调试该接口。

## URI<a name="section40009126"></a>

-   URI格式

    POST /v2.1/\{project\_id\}/cloudvolumes/\{volume\_id\}/action

-   参数说明

    <a name="table30668413"></a>
    <table><thead align="left"><tr id="row58200784"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p16643039"><a name="p16643039"></a><a name="p16643039"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p5908907"><a name="p5908907"></a><a name="p5908907"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p8859419"><a name="p8859419"></a><a name="p8859419"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row46524311"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p10372872"><a name="p10372872"></a><a name="p10372872"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p34896342"><a name="p34896342"></a><a name="p34896342"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p8031464"><a name="p8031464"></a><a name="p8031464"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row5174319"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p16466658"><a name="p16466658"></a><a name="p16466658"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p58730959"><a name="p58730959"></a><a name="p58730959"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p59587228"><a name="p59587228"></a><a name="p59587228"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section24537816"></a>

-   请求参数

    <a name="table42671863"></a>
    <table><thead align="left"><tr id="row12592542"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="p13362997"><a name="p13362997"></a><a name="p13362997"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.2"><p id="p8661001"><a name="p8661001"></a><a name="p8661001"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="p30452481"><a name="p30452481"></a><a name="p30452481"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="p50731910"><a name="p50731910"></a><a name="p50731910"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5187493615377"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p4112025815377"><a name="p4112025815377"></a><a name="p4112025815377"></a>os-extend</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p4240658415377"><a name="p4240658415377"></a><a name="p4240658415377"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p1238131615377"><a name="p1238131615377"></a><a name="p1238131615377"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p6336250715377"><a name="p6336250715377"></a><a name="p6336250715377"></a>标记扩容云硬盘操作，请参见<a href="#li64197069143443">•os-extend参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row33316241143416"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="p45799263143421"><a name="p45799263143421"></a><a name="p45799263143421"></a>bssParam</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="p18752856143421"><a name="p18752856143421"></a><a name="p18752856143421"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="p42586373143421"><a name="p42586373143421"></a><a name="p42586373143421"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="p26944207143421"><a name="p26944207143421"></a><a name="p26944207143421"></a>运营参数，请参见<a href="#li17948921143530">•bssParam参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li64197069143443"></a>os-extend参数说明

    <a name="table902604143432"></a>
    <table><thead align="left"><tr id="row15159441143432"><th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.1"><p id="p8165188154819"><a name="p8165188154819"></a><a name="p8165188154819"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.181818181818183%" id="mcps1.1.5.1.2"><p id="p71673811487"><a name="p71673811487"></a><a name="p71673811487"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.1.5.1.3"><p id="p117058104816"><a name="p117058104816"></a><a name="p117058104816"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.5.1.4"><p id="p15170198164813"><a name="p15170198164813"></a><a name="p15170198164813"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row54092444143432"><td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.1 "><p id="p19411832143432"><a name="p19411832143432"></a><a name="p19411832143432"></a>new_size</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.181818181818183%" headers="mcps1.1.5.1.2 "><p id="p28854520143432"><a name="p28854520143432"></a><a name="p28854520143432"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.1.5.1.3 "><p id="p55514756143432"><a name="p55514756143432"></a><a name="p55514756143432"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.5.1.4 "><p id="p401413143432"><a name="p401413143432"></a><a name="p401413143432"></a>扩容后的云硬盘大小，单位为GB。</p>
    <p id="p3612725143432"><a name="p3612725143432"></a><a name="p3612725143432"></a>扩容后的云硬盘容量范围：大于原有云硬盘容量~云硬盘最大容量（数据盘为32768GB；系统盘为1024GB）</p>
    <div class="note" id="note32514531143432"><a name="note32514531143432"></a><a name="note32514531143432"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p5070492815911"><a name="evs_04_2013_p5070492815911"></a><a name="evs_04_2013_p5070492815911"></a>如果发送请求时，将参数值设置为小数，则默认取小数点前的整数。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li17948921143530"></a>bssParam参数说明

    <a name="table44576521143530"></a>
    <table><thead align="left"><tr id="row39289743143530"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p144831219485"><a name="p144831219485"></a><a name="p144831219485"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p6511512164819"><a name="p6511512164819"></a><a name="p6511512164819"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p854141217486"><a name="p854141217486"></a><a name="p854141217486"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p125571204816"><a name="p125571204816"></a><a name="p125571204816"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row30416269143530"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p3821005143842"><a name="p3821005143842"></a><a name="p3821005143842"></a>isAutoPay</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p41065988143842"><a name="p41065988143842"></a><a name="p41065988143842"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p38010723143842"><a name="p38010723143842"></a><a name="p38010723143842"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><a name="ul29355244143849"></a><a name="ul29355244143849"></a><ul id="ul29355244143849"><li>功能说明：是否立即支付。该参数只有在云硬盘为包周期的情况下有意义。默认值为false。</li><li>取值范围<a name="ul62644497143911"></a><a name="ul62644497143911"></a><ul id="ul62644497143911"><li>false：不立即支付，创建订单暂不支付</li><li>true：立即支付，从帐户余额中自动扣费</li></ul>
    </li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   请求样例

    ```
    {
        "os-extend": {
            "new_size": 100
        }, 
        "bssParam": {
            "isAutoPay": "true"
        }
    }
    ```


## 响应消息<a name="section19513753"></a>

-   响应参数

    <a name="table15441099103019"></a>
    <table><thead align="left"><tr id="row54094047103019"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="p19541716103019"><a name="p19541716103019"></a><a name="p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p39375186103019"><a name="p39375186103019"></a><a name="p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="58.330000000000005%" id="mcps1.1.4.1.3"><p id="p38578950103019"><a name="p38578950103019"></a><a name="p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1924315017243"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p33545583319"><a name="p33545583319"></a><a name="p33545583319"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p19354165810317"><a name="p19354165810317"></a><a name="p19354165810317"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p435416581936"><a name="p435416581936"></a><a name="p435416581936"></a>任务ID，扩容按需云硬盘时返回该参数。</p>
    <div class="note" id="note335410589314"><a name="note335410589314"></a><a name="note335410589314"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1435514588312"><a name="p1435514588312"></a><a name="p1435514588312"></a>如果需要查询job的状态，请参考<a href="查询job的状态.md">查询job的状态</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row11017750143220"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p24400321143233"><a name="p24400321143233"></a><a name="p24400321143233"></a>order_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p30268984143233"><a name="p30268984143233"></a><a name="p30268984143233"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p19678023143233"><a name="p19678023143233"></a><a name="p19678023143233"></a>订单号，扩容包周期云硬盘时返回该参数。</p>
    <div class="note" id="note118971174719"><a name="note118971174719"></a><a name="note118971174719"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p38985719710"><a name="p38985719710"></a><a name="p38985719710"></a>如果需要支付订单，请参考<a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">支付包周期产品订单</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row45731334253"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2010_p1595262111415"><a name="evs_04_2010_p1595262111415"></a><a name="evs_04_2010_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="58.330000000000005%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
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
        "job_id": "70a599e0-31e7-49b7-b260-868f441e862b"
    }
    ```

    或

    ```
    {
        "order_id": "CS1711152257C60TL"
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


## 状态码<a name="section41406050"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

