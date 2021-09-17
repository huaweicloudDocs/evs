# 查询job的状态<a name="evs_04_0054"></a>

## 功能介绍<a name="section48616240"></a>

查询job的状态，可用于查询创建云硬盘，扩容云硬盘，删除云硬盘等API的执行状态。

## 调试<a name="section459923965710"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EVS&api=ShowJob)中直接运行调试该接口。

## URI<a name="section34892981"></a>

-   URI格式

    GET /v1/\{project\_id\}/jobs/\{job\_id\}

-   参数说明

    <a name="table64553311"></a>
    <table><thead align="left"><tr id="row24013807"><th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.1.4.1.1"><p id="p66070243"><a name="p66070243"></a><a name="p66070243"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23%" id="mcps1.1.4.1.2"><p id="p50089467"><a name="p50089467"></a><a name="p50089467"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.4.1.3"><p id="p188321746194612"><a name="p188321746194612"></a><a name="p188321746194612"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4890297"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.4.1.1 "><p id="p60569775"><a name="p60569775"></a><a name="p60569775"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.4.1.2 "><p id="p7204713"><a name="p7204713"></a><a name="p7204713"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.4.1.3 "><p id="p46710863"><a name="p46710863"></a><a name="p46710863"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row17744591"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.4.1.1 "><p id="p28025763"><a name="p28025763"></a><a name="p28025763"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23%" headers="mcps1.1.4.1.2 "><p id="p55494360"><a name="p55494360"></a><a name="p55494360"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.4.1.3 "><p id="p65858198"><a name="p65858198"></a><a name="p65858198"></a>job ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45601378"></a>

以查询jod\_id为ff808081692a62c70169b4dcf9514264的状态为例。

-   请求样例：

    ```
     GET https://{endpoint}/v1/{project_id}/jobs/ff808081692a62c70169b4dcf9514264
    ```


## 响应消息<a name="section7759225"></a>

-   响应参数

    <a name="table50130391201921"></a>
    <table><thead align="left"><tr id="row66097272201921"><th class="cellrowborder" valign="top" width="20.65%" id="mcps1.1.4.1.1"><p id="p52278782201921"><a name="p52278782201921"></a><a name="p52278782201921"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.52%" id="mcps1.1.4.1.2"><p id="p2711067815824"><a name="p2711067815824"></a><a name="p2711067815824"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.830000000000005%" id="mcps1.1.4.1.3"><p id="p7687988201921"><a name="p7687988201921"></a><a name="p7687988201921"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18747316201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p42137645201921"><a name="p42137645201921"></a><a name="p42137645201921"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p4848132715824"><a name="p4848132715824"></a><a name="p4848132715824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p4804017891027"><a name="p4804017891027"></a><a name="p4804017891027"></a>job的状态。</p>
    <a name="ul2970842091027"></a><a name="ul2970842091027"></a><ul id="ul2970842091027"><li>SUCCESS：成功。</li><li>RUNNING：运行中。</li><li>FAIL：失败。</li><li>INIT：正在初始化。</li></ul>
    </td>
    </tr>
    <tr id="row57564514201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p32214083201921"><a name="p32214083201921"></a><a name="p32214083201921"></a>entities</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p3467338415824"><a name="p3467338415824"></a><a name="p3467338415824"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p1736414177101"><a name="p1736414177101"></a><a name="p1736414177101"></a>job的响应信息。具体请参见<a href="#li134182540818">•entities参数说明</a>。</p>
    <p id="p30792195201921"><a name="p30792195201921"></a><a name="p30792195201921"></a>不同的类型的job，其中的内容不同。</p>
    </td>
    </tr>
    <tr id="row8694306201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p33150149201921"><a name="p33150149201921"></a><a name="p33150149201921"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p5708068115824"><a name="p5708068115824"></a><a name="p5708068115824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p65414495201921"><a name="p65414495201921"></a><a name="p65414495201921"></a>job ID。</p>
    </td>
    </tr>
    <tr id="row51859545201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p39873610201921"><a name="p39873610201921"></a><a name="p39873610201921"></a>job_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p6013244315824"><a name="p6013244315824"></a><a name="p6013244315824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p20403760201921"><a name="p20403760201921"></a><a name="p20403760201921"></a>job的类型。</p>
    <a name="ul15245145655114"></a><a name="ul15245145655114"></a><ul id="ul15245145655114"><li>createVolume：创建单个云硬盘。</li><li>batchCreateVolume：批量创建云硬盘。</li><li>deleteVolume：删除单个云硬盘。</li><li>extendVolume：扩容云硬盘。</li><li>bulkDeleteVolume：批量删除云硬盘。</li><li>deleteSingleVolume：批量删除时逐个删除单个云硬盘。</li></ul>
    </td>
    </tr>
    <tr id="row49416119201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p43282735201921"><a name="p43282735201921"></a><a name="p43282735201921"></a>begin_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p3888970115824"><a name="p3888970115824"></a><a name="p3888970115824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p40422711201921"><a name="p40422711201921"></a><a name="p40422711201921"></a>开始时间。</p>
    <p id="p221831420710"><a name="p221831420710"></a><a name="p221831420710"></a>时间格式为：YYYY-MM-DDTHH:MM:SS.SSS'Z'</p>
    </td>
    </tr>
    <tr id="row28260084201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p7365468201921"><a name="p7365468201921"></a><a name="p7365468201921"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p6305809615824"><a name="p6305809615824"></a><a name="p6305809615824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p6457786201921"><a name="p6457786201921"></a><a name="p6457786201921"></a>结束时间。</p>
    <p id="p5536657812"><a name="p5536657812"></a><a name="p5536657812"></a>时间格式为：YYYY-MM-DDTHH:MM:SS.SSS'Z'</p>
    </td>
    </tr>
    <tr id="row58120078201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p10105857201921"><a name="p10105857201921"></a><a name="p10105857201921"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p743216415824"><a name="p743216415824"></a><a name="p743216415824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p971080201921"><a name="p971080201921"></a><a name="p971080201921"></a>job执行失败时的错误码。</p>
    </td>
    </tr>
    <tr id="row8739724201921"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p36829011201921"><a name="p36829011201921"></a><a name="p36829011201921"></a>fail_reason</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p6513437515824"><a name="p6513437515824"></a><a name="p6513437515824"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p43235704201921"><a name="p43235704201921"></a><a name="p43235704201921"></a>job执行失败时的错误原因。</p>
    </td>
    </tr>
    <tr id="row208351118145015"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="evs_04_2010_p1595262111415"><a name="evs_04_2010_p1595262111415"></a><a name="evs_04_2010_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li134182540818"></a>entities参数说明

    <a name="table165761957483"></a>
    <table><thead align="left"><tr id="row1957611571285"><th class="cellrowborder" valign="top" width="20.23202320232023%" id="mcps1.1.4.1.1"><p id="p1276131916910"><a name="p1276131916910"></a><a name="p1276131916910"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.972197219721973%" id="mcps1.1.4.1.2"><p id="p14276101916912"><a name="p14276101916912"></a><a name="p14276101916912"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.795779577957795%" id="mcps1.1.4.1.3"><p id="p627610191596"><a name="p627610191596"></a><a name="p627610191596"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1028619115326"><td class="cellrowborder" valign="top" width="20.23202320232023%" headers="mcps1.1.4.1.1 "><p id="p1128616115329"><a name="p1128616115329"></a><a name="p1128616115329"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.972197219721973%" headers="mcps1.1.4.1.2 "><p id="p2028661116321"><a name="p2028661116321"></a><a name="p2028661116321"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.795779577957795%" headers="mcps1.1.4.1.3 "><p id="p8720124117328"><a name="p8720124117328"></a><a name="p8720124117328"></a>云硬盘的名称。</p>
    </td>
    </tr>
    <tr id="row37149393213"><td class="cellrowborder" valign="top" width="20.23202320232023%" headers="mcps1.1.4.1.1 "><p id="p97140353219"><a name="p97140353219"></a><a name="p97140353219"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.972197219721973%" headers="mcps1.1.4.1.2 "><p id="p97141633323"><a name="p97141633323"></a><a name="p97141633323"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.795779577957795%" headers="mcps1.1.4.1.3 "><p id="p12714031327"><a name="p12714031327"></a><a name="p12714031327"></a>云硬盘的容量，单位为GB。</p>
    </td>
    </tr>
    <tr id="row135768571586"><td class="cellrowborder" valign="top" width="20.23202320232023%" headers="mcps1.1.4.1.1 "><p id="p239893649137"><a name="p239893649137"></a><a name="p239893649137"></a>sub_jobs</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.972197219721973%" headers="mcps1.1.4.1.2 "><p id="p640903559137"><a name="p640903559137"></a><a name="p640903559137"></a>Array of Objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.795779577957795%" headers="mcps1.1.4.1.3 "><p id="p597890789137"><a name="p597890789137"></a><a name="p597890789137"></a>子job的信息。具体请参见<a href="#li1622214314366">•sub_jobs参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row7775144323420"><td class="cellrowborder" valign="top" width="20.23202320232023%" headers="mcps1.1.4.1.1 "><p id="p37754438347"><a name="p37754438347"></a><a name="p37754438347"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.972197219721973%" headers="mcps1.1.4.1.2 "><p id="p17346191720356"><a name="p17346191720356"></a><a name="p17346191720356"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.795779577957795%" headers="mcps1.1.4.1.3 "><p id="p477534323411"><a name="p477534323411"></a><a name="p477534323411"></a>云硬盘的ID。</p>
    </td>
    </tr>
    <tr id="row178791646153418"><td class="cellrowborder" valign="top" width="20.23202320232023%" headers="mcps1.1.4.1.1 "><p id="p1226219733512"><a name="p1226219733512"></a><a name="p1226219733512"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.972197219721973%" headers="mcps1.1.4.1.2 "><p id="p13158151817356"><a name="p13158151817356"></a><a name="p13158151817356"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.795779577957795%" headers="mcps1.1.4.1.3 "><p id="p18794465347"><a name="p18794465347"></a><a name="p18794465347"></a>云硬盘的类型。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li1622214314366"></a>sub\_jobs参数说明

    <a name="table6865512113719"></a>
    <table><thead align="left"><tr id="row297153474016"><th class="cellrowborder" valign="top" width="20.65%" id="mcps1.1.4.1.1"><p id="p1797113341404"><a name="p1797113341404"></a><a name="p1797113341404"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.52%" id="mcps1.1.4.1.2"><p id="p49711134164013"><a name="p49711134164013"></a><a name="p49711134164013"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.830000000000005%" id="mcps1.1.4.1.3"><p id="p15971834164010"><a name="p15971834164010"></a><a name="p15971834164010"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row189771734174015"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p1397633444016"><a name="p1397633444016"></a><a name="p1397633444016"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p297653410404"><a name="p297653410404"></a><a name="p297653410404"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p1397683416404"><a name="p1397683416404"></a><a name="p1397683416404"></a>job的状态。</p>
    <a name="ul29772349401"></a><a name="ul29772349401"></a><ul id="ul29772349401"><li>SUCCESS：成功。</li><li>RUNNING：运行中。</li><li>FAIL：失败。</li><li>INIT：正在初始化。</li></ul>
    </td>
    </tr>
    <tr id="row119772034184010"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p8977113424018"><a name="p8977113424018"></a><a name="p8977113424018"></a>entities</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p179771343406"><a name="p179771343406"></a><a name="p179771343406"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p1977334104014"><a name="p1977334104014"></a><a name="p1977334104014"></a>job的响应信息。具体请参见<a href="#li7735129144218">•entities参数说明</a>。</p>
    <p id="p897715340404"><a name="p897715340404"></a><a name="p897715340404"></a>不同的类型的job，其中的内容不同。</p>
    </td>
    </tr>
    <tr id="row1197793494011"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p19977173415408"><a name="p19977173415408"></a><a name="p19977173415408"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p129776340403"><a name="p129776340403"></a><a name="p129776340403"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p2977133424012"><a name="p2977133424012"></a><a name="p2977133424012"></a>job ID。</p>
    </td>
    </tr>
    <tr id="row19977203420405"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p29771134164010"><a name="p29771134164010"></a><a name="p29771134164010"></a>job_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p097763417405"><a name="p097763417405"></a><a name="p097763417405"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p8977143419406"><a name="p8977143419406"></a><a name="p8977143419406"></a>job的类型。</p>
    <a name="ul1697753474012"></a><a name="ul1697753474012"></a><ul id="ul1697753474012"><li>createVolume：创建单个云硬盘。</li><li>batchCreateVolume：批量创建云硬盘。</li><li>deleteVolume：删除单个云硬盘。</li><li>extendVolume：扩容云硬盘。</li><li>bulkDeleteVolume：批量删除云硬盘。</li><li>deleteSingleVolume：批量删除时逐个删除单个云硬盘。</li></ul>
    </td>
    </tr>
    <tr id="row18977123413409"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p8977123420406"><a name="p8977123420406"></a><a name="p8977123420406"></a>begin_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p79771234134018"><a name="p79771234134018"></a><a name="p79771234134018"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p1697783424017"><a name="p1697783424017"></a><a name="p1697783424017"></a>开始时间。</p>
    <p id="p79771134174010"><a name="p79771134174010"></a><a name="p79771134174010"></a>时间格式为：YYYY-MM-DDTHH:MM:SS.SSS'Z'</p>
    </td>
    </tr>
    <tr id="row1697723410405"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p997714340402"><a name="p997714340402"></a><a name="p997714340402"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p1977113412405"><a name="p1977113412405"></a><a name="p1977113412405"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p597733416409"><a name="p597733416409"></a><a name="p597733416409"></a>结束时间。</p>
    <p id="p189771634164018"><a name="p189771634164018"></a><a name="p189771634164018"></a>时间格式为：YYYY-MM-DDTHH:MM:SS.SSS'Z'</p>
    </td>
    </tr>
    <tr id="row16977133416400"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p189771034134013"><a name="p189771034134013"></a><a name="p189771034134013"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p597712347401"><a name="p597712347401"></a><a name="p597712347401"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p1797793412407"><a name="p1797793412407"></a><a name="p1797793412407"></a>job执行失败时的错误码。</p>
    </td>
    </tr>
    <tr id="row69780343405"><td class="cellrowborder" valign="top" width="20.65%" headers="mcps1.1.4.1.1 "><p id="p19977834204015"><a name="p19977834204015"></a><a name="p19977834204015"></a>fail_reason</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.52%" headers="mcps1.1.4.1.2 "><p id="p8977153411401"><a name="p8977153411401"></a><a name="p8977153411401"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p69787349406"><a name="p69787349406"></a><a name="p69787349406"></a>job执行失败时的错误原因。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li7735129144218"></a>entities参数说明

    <a name="table20171524315"></a>
    <table><thead align="left"><tr id="row01615124316"><th class="cellrowborder" valign="top" width="20.652065206520653%" id="mcps1.1.4.1.1"><p id="p37001534154314"><a name="p37001534154314"></a><a name="p37001534154314"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.832183218321834%" id="mcps1.1.4.1.2"><p id="p1470023413436"><a name="p1470023413436"></a><a name="p1470023413436"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.515751575157516%" id="mcps1.1.4.1.3"><p id="p2700834134312"><a name="p2700834134312"></a><a name="p2700834134312"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row11315194319"><td class="cellrowborder" valign="top" width="20.652065206520653%" headers="mcps1.1.4.1.1 "><p id="p18700934114318"><a name="p18700934114318"></a><a name="p18700934114318"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.832183218321834%" headers="mcps1.1.4.1.2 "><p id="p6700334194318"><a name="p6700334194318"></a><a name="p6700334194318"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.515751575157516%" headers="mcps1.1.4.1.3 "><p id="p570013424318"><a name="p570013424318"></a><a name="p570013424318"></a>云硬盘的名称。</p>
    </td>
    </tr>
    <tr id="row7111157438"><td class="cellrowborder" valign="top" width="20.652065206520653%" headers="mcps1.1.4.1.1 "><p id="p1700193484314"><a name="p1700193484314"></a><a name="p1700193484314"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.832183218321834%" headers="mcps1.1.4.1.2 "><p id="p97001834114319"><a name="p97001834114319"></a><a name="p97001834114319"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.515751575157516%" headers="mcps1.1.4.1.3 "><p id="p12700163444315"><a name="p12700163444315"></a><a name="p12700163444315"></a>云硬盘的容量，单位为GB。</p>
    </td>
    </tr>
    <tr id="row4110151438"><td class="cellrowborder" valign="top" width="20.652065206520653%" headers="mcps1.1.4.1.1 "><p id="p1823415517435"><a name="p1823415517435"></a><a name="p1823415517435"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.832183218321834%" headers="mcps1.1.4.1.2 "><p id="p023445194310"><a name="p023445194310"></a><a name="p023445194310"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.515751575157516%" headers="mcps1.1.4.1.3 "><p id="p20234145114311"><a name="p20234145114311"></a><a name="p20234145114311"></a>云硬盘的ID。</p>
    </td>
    </tr>
    <tr id="row181161513436"><td class="cellrowborder" valign="top" width="20.652065206520653%" headers="mcps1.1.4.1.1 "><p id="p192341751164316"><a name="p192341751164316"></a><a name="p192341751164316"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.832183218321834%" headers="mcps1.1.4.1.2 "><p id="p1123565124315"><a name="p1123565124315"></a><a name="p1123565124315"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.515751575157516%" headers="mcps1.1.4.1.3 "><p id="p16235115154318"><a name="p16235115154318"></a><a name="p16235115154318"></a>云硬盘的类型。</p>
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
        "status": "RUNNING", 
        "entities": {
            "volume_id": "bdf1bb37-f20f-4266-9a04-f43e0a127376"
        }, 
        "job_id": "4010a32d535527910153552b492c0002", 
        "job_type": "createVolume", 
        "begin_time": "2016-03-08T07:40:13.219Z", 
        "end_time": "", 
        "error_code": null, 
        "fail_reason": null
    }
    ```

    或

    ```
    {
        "status": "SUCCESS", 
        "entities": {
            "sub_jobs": [
                {
                    "status": "SUCCESS", 
                    "entities": {
                        "volume_id": "0b549095-4937-4849-8e4c-52aa027d64f7"
                    }, 
                    "job_id": "21917a8d52a19b040152a9f2f2e50041", 
                    "job_type": "createVolume", 
                    "begin_time": "2016-02-04T01:43:37.445Z", 
                    "end_time": "2016-02-04T01:44:02.239Z", 
                    "error_code": null, 
                    "fail_reason": null
                }, 
                {
                    "status": "SUCCESS", 
                    "entities": {
                        "volume_id": "e7bca1a2-d3ed-434f-86f4-a1f11aa80072"
                    }, 
                    "job_id": "21917a8d52a19b040152a9f2f2f60042", 
                    "job_type": "createVolume", 
                    "begin_time": "2016-02-04T01:43:37.462Z", 
                    "end_time": "2016-02-04T01:44:02.245Z", 
                    "error_code": null, 
                    "fail_reason": null
                }
            ]
        }, 
        "job_id": "21917a8d52a19b040152a9f2f1eb003e", 
        "job_type": "batchCreateVolume", 
        "begin_time": "2016-02-04T01:43:37.193Z", 
        "end_time": "2016-02-04T01:44:08.283Z", 
        "error_code": null, 
        "fail_reason": null
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


## 状态码<a name="section2724161"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

