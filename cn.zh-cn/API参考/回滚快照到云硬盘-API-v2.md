# 回滚快照到云硬盘<a name="zh-cn_topic_0142374138"></a>

## 功能介绍<a name="section29798282112049"></a>

将快照数据回滚到云硬盘。支持企业项目授权功能。

## 接口约束<a name="section18412201112049"></a>

-   只支持快照回滚到源云硬盘，不支持快照回滚到其它指定云硬盘。
-   只有云硬盘状态处于“available“或“error\_rollbacking“状态才允许快照回滚到源云硬盘。
-   名称以autobk\_snapshot\_为前缀的快照是创建云硬盘备份时系统自动创建的，请不要进行“回滚快照到云硬盘”操作。

## URI<a name="section56404342112049"></a>

-   URI格式

    POST /v2/\{project\_id\}/cloudsnapshots/\{snapshot\_id\}/rollback


-   参数说明

    <a name="zh-cn_topic_0051408629_table37114383112049"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_row4845983112049"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408629_p56980371112049"><a name="zh-cn_topic_0051408629_p56980371112049"></a><a name="zh-cn_topic_0051408629_p56980371112049"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408629_p52007339112049"><a name="zh-cn_topic_0051408629_p52007339112049"></a><a name="zh-cn_topic_0051408629_p52007339112049"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408629_p51844944112049"><a name="zh-cn_topic_0051408629_p51844944112049"></a><a name="zh-cn_topic_0051408629_p51844944112049"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_row38690921112049"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_p46956895112049"><a name="zh-cn_topic_0051408629_p46956895112049"></a><a name="zh-cn_topic_0051408629_p46956895112049"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_p45412121112049"><a name="zh-cn_topic_0051408629_p45412121112049"></a><a name="zh-cn_topic_0051408629_p45412121112049"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_p54503167112049"><a name="zh-cn_topic_0051408629_p54503167112049"></a><a name="zh-cn_topic_0051408629_p54503167112049"></a>项目ID。</p>
    <p id="zh-cn_topic_0051408629_p55811451337"><a name="zh-cn_topic_0051408629_p55811451337"></a><a name="zh-cn_topic_0051408629_p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408629_row20766463112049"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_p4361939112049"><a name="zh-cn_topic_0051408629_p4361939112049"></a><a name="zh-cn_topic_0051408629_p4361939112049"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_p17772808112049"><a name="zh-cn_topic_0051408629_p17772808112049"></a><a name="zh-cn_topic_0051408629_p17772808112049"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_p30311366112049"><a name="zh-cn_topic_0051408629_p30311366112049"></a><a name="zh-cn_topic_0051408629_p30311366112049"></a>快照ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section54272198112126"></a>

-   请求参数

    <a name="zh-cn_topic_0051408629_table9185191931813"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_row418511198189"><th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0051408629_p7185219111814"><a name="zh-cn_topic_0051408629_p7185219111814"></a><a name="zh-cn_topic_0051408629_p7185219111814"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0051408629_p17185419171810"><a name="zh-cn_topic_0051408629_p17185419171810"></a><a name="zh-cn_topic_0051408629_p17185419171810"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0051408629_p918520193181"><a name="zh-cn_topic_0051408629_p918520193181"></a><a name="zh-cn_topic_0051408629_p918520193181"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0051408629_p31851819151817"><a name="zh-cn_topic_0051408629_p31851819151817"></a><a name="zh-cn_topic_0051408629_p31851819151817"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_row201857197184"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408629_p11186181941818"><a name="zh-cn_topic_0051408629_p11186181941818"></a><a name="zh-cn_topic_0051408629_p11186181941818"></a>rollback</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408629_p5186101971818"><a name="zh-cn_topic_0051408629_p5186101971818"></a><a name="zh-cn_topic_0051408629_p5186101971818"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408629_p218641911810"><a name="zh-cn_topic_0051408629_p218641911810"></a><a name="zh-cn_topic_0051408629_p218641911810"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408629_p14186519171816"><a name="zh-cn_topic_0051408629_p14186519171816"></a><a name="zh-cn_topic_0051408629_p14186519171816"></a>快照回滚信息，请参见<a href="#zh-cn_topic_0051408629_li37311846112126">•rollback参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="zh-cn_topic_0051408629_li37311846112126"></a>rollback参数说明

    <a name="zh-cn_topic_0051408629_table262294112126"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_row15086975112126"><th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.1"><p id="zh-cn_topic_0051408629_p14085481112126"><a name="zh-cn_topic_0051408629_p14085481112126"></a><a name="zh-cn_topic_0051408629_p14085481112126"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.1.5.1.2"><p id="zh-cn_topic_0051408629_p73303112126"><a name="zh-cn_topic_0051408629_p73303112126"></a><a name="zh-cn_topic_0051408629_p73303112126"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.1.5.1.3"><p id="zh-cn_topic_0051408629_p5937586112126"><a name="zh-cn_topic_0051408629_p5937586112126"></a><a name="zh-cn_topic_0051408629_p5937586112126"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.51485148514851%" id="mcps1.1.5.1.4"><p id="zh-cn_topic_0051408629_p11182433112126"><a name="zh-cn_topic_0051408629_p11182433112126"></a><a name="zh-cn_topic_0051408629_p11182433112126"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_row47675000112126"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408629_p36469802112126"><a name="zh-cn_topic_0051408629_p36469802112126"></a><a name="zh-cn_topic_0051408629_p36469802112126"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408629_p1264009112126"><a name="zh-cn_topic_0051408629_p1264009112126"></a><a name="zh-cn_topic_0051408629_p1264009112126"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408629_p35275900112126"><a name="zh-cn_topic_0051408629_p35275900112126"></a><a name="zh-cn_topic_0051408629_p35275900112126"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408629_p16492175643818"><a name="zh-cn_topic_0051408629_p16492175643818"></a><a name="zh-cn_topic_0051408629_p16492175643818"></a>回滚的目标云硬盘的ID。</p>
    <p id="zh-cn_topic_0051408629_p38775660112126"><a name="zh-cn_topic_0051408629_p38775660112126"></a><a name="zh-cn_topic_0051408629_p38775660112126"></a>查询目标磁盘的ID，请参见<a href="查询单个云硬盘快照详细信息-API-v2.md">查询单个云硬盘快照详细信息</a>中的响应“volume_id”。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408629_row13436622112126"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.1 "><p id="zh-cn_topic_0051408629_p14624579112126"><a name="zh-cn_topic_0051408629_p14624579112126"></a><a name="zh-cn_topic_0051408629_p14624579112126"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.1.5.1.2 "><p id="zh-cn_topic_0051408629_p43740265112126"><a name="zh-cn_topic_0051408629_p43740265112126"></a><a name="zh-cn_topic_0051408629_p43740265112126"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.1.5.1.3 "><p id="zh-cn_topic_0051408629_p53300583112126"><a name="zh-cn_topic_0051408629_p53300583112126"></a><a name="zh-cn_topic_0051408629_p53300583112126"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.51485148514851%" headers="mcps1.1.5.1.4 "><p id="zh-cn_topic_0051408629_p22380006112126"><a name="zh-cn_topic_0051408629_p22380006112126"></a><a name="zh-cn_topic_0051408629_p22380006112126"></a>回滚的目标云硬盘名称。<span id="zh-cn_topic_0051408629_text9102076152627"><a name="zh-cn_topic_0051408629_text9102076152627"></a><a name="zh-cn_topic_0051408629_text9102076152627"></a>最大支持255个字节。</span></p>
    <p id="zh-cn_topic_0051408629_p33311644194012"><a name="zh-cn_topic_0051408629_p33311644194012"></a><a name="zh-cn_topic_0051408629_p33311644194012"></a>查询目标磁盘的名称，请参见<a href="查询单个云硬盘详情-API-v3.md">查询单个云硬盘详情</a>中的响应“name”。</p>
    <div class="note" id="zh-cn_topic_0051408629_note6490498915441"><a name="zh-cn_topic_0051408629_note6490498915441"></a><a name="zh-cn_topic_0051408629_note6490498915441"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0051408629_p4727398915441"><a name="zh-cn_topic_0051408629_p4727398915441"></a><a name="zh-cn_topic_0051408629_p4727398915441"></a>name不能单独传，若传name，必须带上对应的volume_id。</p>
    </div></div>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "rollback": {
            "name": "test-001",
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635"
        }
    }
    ```


## 响应消息<a name="section50618846112239"></a>

-   响应参数

    <a name="zh-cn_topic_0051408629_table55593749112239"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_row12503066112239"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408629_p6115391112239"><a name="zh-cn_topic_0051408629_p6115391112239"></a><a name="zh-cn_topic_0051408629_p6115391112239"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408629_p25584640112239"><a name="zh-cn_topic_0051408629_p25584640112239"></a><a name="zh-cn_topic_0051408629_p25584640112239"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408629_p21559929112239"><a name="zh-cn_topic_0051408629_p21559929112239"></a><a name="zh-cn_topic_0051408629_p21559929112239"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_row59821639112239"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_p13714567112239"><a name="zh-cn_topic_0051408629_p13714567112239"></a><a name="zh-cn_topic_0051408629_p13714567112239"></a>rollback</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_p37138152112239"><a name="zh-cn_topic_0051408629_p37138152112239"></a><a name="zh-cn_topic_0051408629_p37138152112239"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_p58242347112239"><a name="zh-cn_topic_0051408629_p58242347112239"></a><a name="zh-cn_topic_0051408629_p58242347112239"></a>快照回滚信息，请参见<a href="#zh-cn_topic_0051408629_li1951113011190">•rollback参数说明</a>。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408629_row434455911170"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_p129522216412"><a name="zh-cn_topic_0051408629_p129522216412"></a><a name="zh-cn_topic_0051408629_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_p1595262111415"><a name="zh-cn_topic_0051408629_p1595262111415"></a><a name="zh-cn_topic_0051408629_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_p109527215417"><a name="zh-cn_topic_0051408629_p109527215417"></a><a name="zh-cn_topic_0051408629_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#zh-cn_topic_0051408629_li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0051408629_li1951113011190"></a>rollback参数说明

    <a name="zh-cn_topic_0051408629_table051223010193"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_row1351211309194"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408629_p1551203041918"><a name="zh-cn_topic_0051408629_p1551203041918"></a><a name="zh-cn_topic_0051408629_p1551203041918"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.810000000000002%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408629_p11512183013191"><a name="zh-cn_topic_0051408629_p11512183013191"></a><a name="zh-cn_topic_0051408629_p11512183013191"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408629_p451263020195"><a name="zh-cn_topic_0051408629_p451263020195"></a><a name="zh-cn_topic_0051408629_p451263020195"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_row13513173071913"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_p25133307192"><a name="zh-cn_topic_0051408629_p25133307192"></a><a name="zh-cn_topic_0051408629_p25133307192"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.810000000000002%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_p1151353011199"><a name="zh-cn_topic_0051408629_p1151353011199"></a><a name="zh-cn_topic_0051408629_p1151353011199"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_p451323041912"><a name="zh-cn_topic_0051408629_p451323041912"></a><a name="zh-cn_topic_0051408629_p451323041912"></a>快照回滚的目标云硬盘的ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="zh-cn_topic_0051408629_li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0051408629_zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "rollback": {
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635"
        }
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

    其中error是泛指的错误，有badRequest、itemNotFound等，如报错：

    ```
    {
        "badRequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 状态码<a name="section16529200112352"></a>

-   正常

    202


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

