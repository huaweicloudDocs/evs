# 删除云硬盘<a name="evs_04_2008"></a>

## 功能介绍<a name="section10932885"></a>

删除一个云硬盘。支持企业项目授权功能。

## 调试<a name="section131821621358"></a>

您可以在[API Explorer](https://apiexplorer.developer.huaweicloud.com/apiexplorer/doc?product=EVS&api=DeleteVolume)中直接运行调试该接口。

## URI<a name="section31287108"></a>

-   URI格式

    DELETE /v2/\{project\_id\}/cloudvolumes/\{volume\_id\}

-   参数说明

    <a name="table44522499"></a>
    <table><thead align="left"><tr id="row39474480"><th class="cellrowborder" valign="top" width="26.52%" id="mcps1.1.4.1.1"><p id="p43316293"><a name="p43316293"></a><a name="p43316293"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.32%" id="mcps1.1.4.1.2"><p id="p18958859"><a name="p18958859"></a><a name="p18958859"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.16%" id="mcps1.1.4.1.3"><p id="p59272617"><a name="p59272617"></a><a name="p59272617"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row36352712"><td class="cellrowborder" valign="top" width="26.52%" headers="mcps1.1.4.1.1 "><p id="p58888592"><a name="p58888592"></a><a name="p58888592"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.1.4.1.2 "><p id="p5246632"><a name="p5246632"></a><a name="p5246632"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.16%" headers="mcps1.1.4.1.3 "><p id="p22324024"><a name="p22324024"></a><a name="p22324024"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row66698493"><td class="cellrowborder" valign="top" width="26.52%" headers="mcps1.1.4.1.1 "><p id="p33868853"><a name="p33868853"></a><a name="p33868853"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.32%" headers="mcps1.1.4.1.2 "><p id="p59022586"><a name="p59022586"></a><a name="p59022586"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.16%" headers="mcps1.1.4.1.3 "><p id="p16100147"><a name="p16100147"></a><a name="p16100147"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section13148517"></a>

-   请求样例：

    ```
    DELETE https://{endpoint}/v2/{project_id}/cloudvolumes/b104b8db-170d-441b-897a-3c8ba9c5a214
    ```


## 响应消息<a name="section51227795"></a>

-   响应参数

    <a name="evs_04_2013_table735313581437"></a>
    <table><thead align="left"><tr id="evs_04_2013_row153536585313"><th class="cellrowborder" valign="top" width="21.157884211578843%" id="mcps1.1.4.1.1"><p id="evs_04_2013_p123541158732"><a name="evs_04_2013_p123541158732"></a><a name="evs_04_2013_p123541158732"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.197880211978802%" id="mcps1.1.4.1.2"><p id="evs_04_2013_p1435411581320"><a name="evs_04_2013_p1435411581320"></a><a name="evs_04_2013_p1435411581320"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2013_p13541058036"><a name="evs_04_2013_p13541058036"></a><a name="evs_04_2013_p13541058036"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2013_row1135495819312"><td class="cellrowborder" valign="top" width="21.157884211578843%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p33545583319"><a name="evs_04_2013_p33545583319"></a><a name="evs_04_2013_p33545583319"></a>job_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.197880211978802%" headers="mcps1.1.4.1.2 "><p id="evs_04_2013_p19354165810317"><a name="evs_04_2013_p19354165810317"></a><a name="evs_04_2013_p19354165810317"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p435416581936"><a name="evs_04_2013_p435416581936"></a><a name="evs_04_2013_p435416581936"></a>正常返回时返回的任务ID。</p>
    <div class="note" id="evs_04_2013_note335410589314"><a name="evs_04_2013_note335410589314"></a><a name="evs_04_2013_note335410589314"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="evs_04_2013_p1435514588312"><a name="evs_04_2013_p1435514588312"></a><a name="evs_04_2013_p1435514588312"></a>如果需要查询job的状态，请参考<a href="查询job的状态.md">查询job的状态</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="evs_04_2013_row195162113414"><td class="cellrowborder" valign="top" width="21.157884211578843%" headers="mcps1.1.4.1.1 "><p id="evs_04_2013_p129522216412"><a name="evs_04_2013_p129522216412"></a><a name="evs_04_2013_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.197880211978802%" headers="mcps1.1.4.1.2 "><p id="evs_04_2010_p1595262111415"><a name="evs_04_2010_p1595262111415"></a><a name="evs_04_2010_p1595262111415"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2013_p109527215417"><a name="evs_04_2013_p109527215417"></a><a name="evs_04_2013_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
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
        "error": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section58396974"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

