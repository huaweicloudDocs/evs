# 查询job的状态<a name="ZH-CN_TOPIC_0020235138"></a>

## 功能介绍<a name="section48616240"></a>

查询job的状态，可用于查询创建云硬盘，扩容云硬盘，删除云硬盘等API的执行状态。

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


## 请求<a name="section45601378"></a>

无

## 响应<a name="section7759225"></a>

-   响应参数

    <a name="table50130391201921"></a>
    <table><thead align="left"><tr id="row66097272201921"><th class="cellrowborder" valign="top" width="20.48%" id="mcps1.1.4.1.1"><p id="p52278782201921"><a name="p52278782201921"></a><a name="p52278782201921"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.69%" id="mcps1.1.4.1.2"><p id="p2711067815824"><a name="p2711067815824"></a><a name="p2711067815824"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.830000000000005%" id="mcps1.1.4.1.3"><p id="p7687988201921"><a name="p7687988201921"></a><a name="p7687988201921"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18747316201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p42137645201921"><a name="p42137645201921"></a><a name="p42137645201921"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p4848132715824"><a name="p4848132715824"></a><a name="p4848132715824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p4804017891027"><a name="p4804017891027"></a><a name="p4804017891027"></a>job的状态。</p>
    <a name="ul2970842091027"></a><a name="ul2970842091027"></a><ul id="ul2970842091027"><li>SUCCESS：成功。</li><li>RUNNING：运行中。</li><li>FAIL：失败。</li><li>INIT：正在初始化。</li></ul>
    </td>
    </tr>
    <tr id="row57564514201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p32214083201921"><a name="p32214083201921"></a><a name="p32214083201921"></a>entities</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p3467338415824"><a name="p3467338415824"></a><a name="p3467338415824"></a>map&lt;string, object&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p30792195201921"><a name="p30792195201921"></a><a name="p30792195201921"></a>job的响应信息。不同的类型的job，其中的内容不同。</p>
    </td>
    </tr>
    <tr id="row8694306201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p33150149201921"><a name="p33150149201921"></a><a name="p33150149201921"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p5708068115824"><a name="p5708068115824"></a><a name="p5708068115824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p65414495201921"><a name="p65414495201921"></a><a name="p65414495201921"></a>job ID。</p>
    </td>
    </tr>
    <tr id="row51859545201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p39873610201921"><a name="p39873610201921"></a><a name="p39873610201921"></a>job_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p6013244315824"><a name="p6013244315824"></a><a name="p6013244315824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p20403760201921"><a name="p20403760201921"></a><a name="p20403760201921"></a>job的类型。</p>
    <a name="ul15245145655114"></a><a name="ul15245145655114"></a><ul id="ul15245145655114"><li>createVolume：创建单个云硬盘。</li><li>batchCreateVolume：批量创建云硬盘。</li><li>deleteVolume：删除单个云硬盘。</li><li>extendVolume：扩容云硬盘。</li><li>bulkDeleteVolume：批量删除云硬盘。</li><li>deleteSingleVolume：批量删除时逐个删除单个云硬盘。</li></ul>
    </td>
    </tr>
    <tr id="row49416119201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p43282735201921"><a name="p43282735201921"></a><a name="p43282735201921"></a>begin_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p3888970115824"><a name="p3888970115824"></a><a name="p3888970115824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p40422711201921"><a name="p40422711201921"></a><a name="p40422711201921"></a>开始时间。</p>
    </td>
    </tr>
    <tr id="row28260084201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p7365468201921"><a name="p7365468201921"></a><a name="p7365468201921"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p6305809615824"><a name="p6305809615824"></a><a name="p6305809615824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p6457786201921"><a name="p6457786201921"></a><a name="p6457786201921"></a>结束时间。</p>
    </td>
    </tr>
    <tr id="row58120078201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p10105857201921"><a name="p10105857201921"></a><a name="p10105857201921"></a>error_code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p743216415824"><a name="p743216415824"></a><a name="p743216415824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p971080201921"><a name="p971080201921"></a><a name="p971080201921"></a>job执行失败时的错误码。</p>
    </td>
    </tr>
    <tr id="row8739724201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p36829011201921"><a name="p36829011201921"></a><a name="p36829011201921"></a>fail_reason</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p6513437515824"><a name="p6513437515824"></a><a name="p6513437515824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p43235704201921"><a name="p43235704201921"></a><a name="p43235704201921"></a>job执行失败时的错误原因。</p>
    </td>
    </tr>
    <tr id="row53577021201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p44771411201921"><a name="p44771411201921"></a><a name="p44771411201921"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p4139306015824"><a name="p4139306015824"></a><a name="p4139306015824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p9733033201921"><a name="p9733033201921"></a><a name="p9733033201921"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="row20488440201921"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p48950919201921"><a name="p48950919201921"></a><a name="p48950919201921"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p6450355315824"><a name="p6450355315824"></a><a name="p6450355315824"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p51067587201921"><a name="p51067587201921"></a><a name="p51067587201921"></a>出现错误时，返回的错误码。</p>
    <p id="p56955100201921"><a name="p56955100201921"></a><a name="p56955100201921"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    <tr id="row500064349137"><td class="cellrowborder" valign="top" width="20.48%" headers="mcps1.1.4.1.1 "><p id="p239893649137"><a name="p239893649137"></a><a name="p239893649137"></a>sub_jobs</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.69%" headers="mcps1.1.4.1.2 "><p id="p640903559137"><a name="p640903559137"></a><a name="p640903559137"></a>list</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.830000000000005%" headers="mcps1.1.4.1.3 "><p id="p597890789137"><a name="p597890789137"></a><a name="p597890789137"></a>每个子job的执行信息。没有子job时为空列表。每个子job的结构与父job类似。</p>
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


## 返回值<a name="section2724161"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

