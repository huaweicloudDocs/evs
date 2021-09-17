# 查询云硬盘过户记录列表详情<a name="evs_04_3074"></a>

## 功能介绍<a name="zh-cn_topic_0092902037_section44805042171914"></a>

查询当前租户下所有云硬盘的过户记录列表的详细信息，比如过户记录创建时间、ID以及名称等信息。

## URI<a name="zh-cn_topic_0092887872_section21748494171940"></a>

-   URI格式

    GET /v3/\{project\_id\}/os-volume-transfer/detail

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
    <tbody><tr id="row4735411910529"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p1047843010529"><a name="p1047843010529"></a><a name="p1047843010529"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p4344649310529"><a name="p4344649310529"></a><a name="p4344649310529"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p2950506910529"><a name="p2950506910529"></a><a name="p2950506910529"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request filter参数说明

    <a name="evs_04_2110_table114096539515"></a>
    <table><thead align="left"><tr id="evs_04_2110_row64913538519"><th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.1"><p id="evs_04_2110_p14491115311514"><a name="evs_04_2110_p14491115311514"></a><a name="evs_04_2110_p14491115311514"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.1.5.1.2"><p id="evs_04_2110_p54911753125116"><a name="evs_04_2110_p54911753125116"></a><a name="evs_04_2110_p54911753125116"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.772277227722775%" id="mcps1.1.5.1.3"><p id="evs_04_2110_p10491105315113"><a name="evs_04_2110_p10491105315113"></a><a name="evs_04_2110_p10491105315113"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="41.584158415841586%" id="mcps1.1.5.1.4"><p id="evs_04_2110_p16491553125110"><a name="evs_04_2110_p16491553125110"></a><a name="evs_04_2110_p16491553125110"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2110_row64916530515"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="evs_04_2110_p14491953135112"><a name="evs_04_2110_p14491953135112"></a><a name="evs_04_2110_p14491953135112"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="evs_04_2110_p15491185365111"><a name="evs_04_2110_p15491185365111"></a><a name="evs_04_2110_p15491185365111"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.772277227722775%" headers="mcps1.1.5.1.3 "><p id="evs_04_2110_p349155345117"><a name="evs_04_2110_p349155345117"></a><a name="evs_04_2110_p349155345117"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.584158415841586%" headers="mcps1.1.5.1.4 "><p id="evs_04_2110_p12491175314513"><a name="evs_04_2110_p12491175314513"></a><a name="evs_04_2110_p12491175314513"></a>返回结果个数限制。</p>
    <p id="evs_04_2110_p116095293163"><a name="evs_04_2110_p116095293163"></a><a name="evs_04_2110_p116095293163"></a><span id="evs_04_2110_text138349551887"><a name="evs_04_2110_text138349551887"></a><a name="evs_04_2110_text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    </td>
    </tr>
    <tr id="evs_04_2110_row12491135365118"><td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.1 "><p id="evs_04_2110_p54911153165115"><a name="evs_04_2110_p54911153165115"></a><a name="evs_04_2110_p54911153165115"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.1.5.1.2 "><p id="evs_04_2110_p0491145315116"><a name="evs_04_2110_p0491145315116"></a><a name="evs_04_2110_p0491145315116"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.772277227722775%" headers="mcps1.1.5.1.3 "><p id="evs_04_2110_p549165318518"><a name="evs_04_2110_p549165318518"></a><a name="evs_04_2110_p549165318518"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.584158415841586%" headers="mcps1.1.5.1.4 "><p id="evs_04_2110_p164913532515"><a name="evs_04_2110_p164913532515"></a><a name="evs_04_2110_p164913532515"></a>偏移量，偏移量为一个大于0小于云硬盘过户记录总个数的整数，表示查询该偏移量后面的所有的云硬盘过户记录。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section45527389"></a>

以查询云硬盘过户记录的返回结果最大50个为例。

-   请求样例

    ```
    GET https://{endpoint}/v3/{project_id}/os-volume-transfer/detail?limit=50
    ```


## 响应参数<a name="zh-cn_topic_0092902037_section23586530172122"></a>

-   响应参数

    <a name="evs_04_2111_table44421424377"></a>
    <table><thead align="left"><tr id="evs_04_2111_row16442202183720"><th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.1"><p id="evs_04_2111_p044210213713"><a name="evs_04_2111_p044210213713"></a><a name="evs_04_2111_p044210213713"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.377662233776622%" id="mcps1.1.4.1.2"><p id="evs_04_2111_p1944232103719"><a name="evs_04_2111_p1944232103719"></a><a name="evs_04_2111_p1944232103719"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.24467553244675%" id="mcps1.1.4.1.3"><p id="evs_04_2111_p104421529376"><a name="evs_04_2111_p104421529376"></a><a name="evs_04_2111_p104421529376"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2111_row1944316223713"><td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_p124437213370"><a name="evs_04_2111_p124437213370"></a><a name="evs_04_2111_p124437213370"></a>transfers</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.377662233776622%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_p1944332193718"><a name="evs_04_2111_p1944332193718"></a><a name="evs_04_2111_p1944332193718"></a>List&lt;Transfer&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_p124439263715"><a name="evs_04_2111_p124439263715"></a><a name="evs_04_2111_p124439263715"></a>云硬盘过户记录列表详情，请参见<a href="#evs_04_2111_li39411666114933">•transfers参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="evs_04_2111_li39411666114933"></a>transfers参数说明

    <a name="evs_04_2111_zh-cn_topic_0092902037_table6685576181553"></a>
    <table><thead align="left"><tr id="evs_04_2111_zh-cn_topic_0092902037_row1296752181553"><th class="cellrowborder" valign="top" width="23.41765823417658%" id="mcps1.1.4.1.1"><p id="evs_04_2111_p6080130411503"><a name="evs_04_2111_p6080130411503"></a><a name="evs_04_2111_p6080130411503"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="23.337666233376662%" id="mcps1.1.4.1.2"><p id="evs_04_2111_p2595862911503"><a name="evs_04_2111_p2595862911503"></a><a name="evs_04_2111_p2595862911503"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.24467553244675%" id="mcps1.1.4.1.3"><p id="evs_04_2111_p5937927111503"><a name="evs_04_2111_p5937927111503"></a><a name="evs_04_2111_p5937927111503"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2111_zh-cn_topic_0092902037_row12974480107"><td class="cellrowborder" valign="top" width="23.41765823417658%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_zh-cn_topic_0092902037_p1097410819109"><a name="evs_04_2111_zh-cn_topic_0092902037_p1097410819109"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p1097410819109"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.337666233376662%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_zh-cn_topic_0092902037_p797448121011"><a name="evs_04_2111_zh-cn_topic_0092902037_p797448121011"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p797448121011"></a>List&lt; Dict &gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_p62103920115039"><a name="evs_04_2111_p62103920115039"></a><a name="evs_04_2111_p62103920115039"></a>云硬盘过户记录的链接。</p>
    </td>
    </tr>
    <tr id="evs_04_2111_zh-cn_topic_0092902037_row862121220101"><td class="cellrowborder" valign="top" width="23.41765823417658%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_zh-cn_topic_0092902037_p1762112141010"><a name="evs_04_2111_zh-cn_topic_0092902037_p1762112141010"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p1762112141010"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.337666233376662%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_zh-cn_topic_0092902037_p4623123109"><a name="evs_04_2111_zh-cn_topic_0092902037_p4623123109"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p4623123109"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_zh-cn_topic_0092902037_p186221213104"><a name="evs_04_2111_zh-cn_topic_0092902037_p186221213104"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p186221213104"></a>云硬盘过户记录的创建时间。</p>
    <p id="evs_04_2111_p418335273815"><a name="evs_04_2111_p418335273815"></a><a name="evs_04_2111_p418335273815"></a><span id="evs_04_2111_text164869573817"><a name="evs_04_2111_text164869573817"></a><a name="evs_04_2111_text164869573817"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="evs_04_2111_zh-cn_topic_0092902037_row569771417102"><td class="cellrowborder" valign="top" width="23.41765823417658%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_zh-cn_topic_0092902037_p369761461010"><a name="evs_04_2111_zh-cn_topic_0092902037_p369761461010"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p369761461010"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.337666233376662%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_zh-cn_topic_0092902037_p769712143104"><a name="evs_04_2111_zh-cn_topic_0092902037_p769712143104"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p769712143104"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_zh-cn_topic_0092902037_p56979145107"><a name="evs_04_2111_zh-cn_topic_0092902037_p56979145107"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p56979145107"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2111_zh-cn_topic_0092902037_row2457217151019"><td class="cellrowborder" valign="top" width="23.41765823417658%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_zh-cn_topic_0092902037_p94571174106"><a name="evs_04_2111_zh-cn_topic_0092902037_p94571174106"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p94571174106"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.337666233376662%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_zh-cn_topic_0092902037_p174577172105"><a name="evs_04_2111_zh-cn_topic_0092902037_p174577172105"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p174577172105"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_p20497649115033"><a name="evs_04_2111_p20497649115033"></a><a name="evs_04_2111_p20497649115033"></a>云硬盘过户记录的ID。</p>
    </td>
    </tr>
    <tr id="evs_04_2111_zh-cn_topic_0092902037_row527752431012"><td class="cellrowborder" valign="top" width="23.41765823417658%" headers="mcps1.1.4.1.1 "><p id="evs_04_2111_zh-cn_topic_0092902037_p10277112415105"><a name="evs_04_2111_zh-cn_topic_0092902037_p10277112415105"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p10277112415105"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="23.337666233376662%" headers="mcps1.1.4.1.2 "><p id="evs_04_2111_zh-cn_topic_0092902037_p4277132441017"><a name="evs_04_2111_zh-cn_topic_0092902037_p4277132441017"></a><a name="evs_04_2111_zh-cn_topic_0092902037_p4277132441017"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.24467553244675%" headers="mcps1.1.4.1.3 "><p id="evs_04_2111_p44618758115033"><a name="evs_04_2111_p44618758115033"></a><a name="evs_04_2111_p44618758115033"></a>云硬盘过户记录的名称。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "transfers": [
            {
                "id": "cac5c677-73a9-4288-bb9c-b2ebfb547377", 
                "created_at": "2015-02-25T03:56:53.081642", 
                "name": "first volume transfer", 
                "volume_id": "894623a6-e901-4312-aa06-4275e6321cce", 
                "links": [
                    {
                        "href": "https://localhost/v2/firstproject/os-volume-transfer/1", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://localhost/firstproject/os-volume-transfer/1", 
                        "rel": "bookmark"
                    }
                ]
            }, 
            {
                "id": "f26c0dee-d20d-4e80-8dee-a8d91b9742a1", 
                "created_at": "2015-03-25T03:56:53.081642", 
                "name": "second volume transfer", 
                "volume_id": "673db275-379f-41af-8371-e1652132b4c1", 
                "links": [
                    {
                        "href": "https://localhost/v2/firstproject/os-volume-transfer/2", 
                        "rel": "self"
                    }, 
                    {
                        "href": "https://localhost/firstproject/os-volume-transfer/2", 
                        "rel": "bookmark"
                    }
                ]
            }
        ]
    }
    ```


## 状态码<a name="zh-cn_topic_0092902037_section10353980172239"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码](错误码.md)。

