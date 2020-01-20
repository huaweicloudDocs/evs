# 通过标签查询云硬盘资源实例详情<a name="zh-cn_topic_0102797323"></a>

## 功能介绍<a name="section5299350116935"></a>

通过标签查询云硬盘资源实例详情。

## 接口约束<a name="section4466609116935"></a>

无

## URI<a name="section1378135716935"></a>

-   URI格式

    POST /v2/\{project\_id\}/cloudvolumes/resource\_instances/action

-   参数说明

    <a name="table28484833104128"></a>
    <table><thead align="left"><tr id="row60547305104128"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p5384679104128"><a name="p5384679104128"></a><a name="p5384679104128"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p33505894104128"><a name="p33505894104128"></a><a name="p33505894104128"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p29622926104128"><a name="p29622926104128"></a><a name="p29622926104128"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row50646790104128"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p8749302104128"><a name="p8749302104128"></a><a name="p8749302104128"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p37604871104128"><a name="p37604871104128"></a><a name="p37604871104128"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p26095712104128"><a name="p26095712104128"></a><a name="p26095712104128"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section33444519162337"></a>

-   请求参数

    <a name="table50618906162337"></a>
    <table><thead align="left"><tr id="row13155682162337"><th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.1"><p id="p58977321162337"><a name="p58977321162337"></a><a name="p58977321162337"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.5.1.2"><p id="p12433688162337"><a name="p12433688162337"></a><a name="p12433688162337"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.5.1.3"><p id="p495832162337"><a name="p495832162337"></a><a name="p495832162337"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="41.41414141414141%" id="mcps1.1.5.1.4"><p id="p40162449162337"><a name="p40162449162337"></a><a name="p40162449162337"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row31932906162337"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p36428555162337"><a name="p36428555162337"></a><a name="p36428555162337"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p65031837162337"><a name="p65031837162337"></a><a name="p65031837162337"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p33087431162337"><a name="p33087431162337"></a><a name="p33087431162337"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.41414141414141%" headers="mcps1.1.5.1.4 "><p id="p62836274162337"><a name="p62836274162337"></a><a name="p62836274162337"></a>标签的键值对，请参见<a href="#li8528152083214">•resource_tag参数数据结构说明</a>。</p>
    <p id="p1858507716"><a name="p1858507716"></a><a name="p1858507716"></a>标签列表中最多包含10个key 。</p>
    <p id="p175842500716"><a name="p175842500716"></a><a name="p175842500716"></a>标签列表中的标签key值不允许重复。</p>
    <p id="p14391151142511"><a name="p14391151142511"></a><a name="p14391151142511"></a>标签列表中多个key之间是“与”的关系，云硬盘必须满足请求中所有key才会匹配出来。</p>
    <div class="note" id="note1461127173813"><a name="note1461127173813"></a><a name="note1461127173813"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0102788725_p1970754173519"><a name="zh-cn_topic_0102788725_p1970754173519"></a><a name="zh-cn_topic_0102788725_p1970754173519"></a>如果存在多个tags结构体，以最后一个tags结构体为准，之前的会被覆盖。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row862173882314"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p1487452192311"><a name="p1487452192311"></a><a name="p1487452192311"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p08795219233"><a name="p08795219233"></a><a name="p08795219233"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p47340819249"><a name="p47340819249"></a><a name="p47340819249"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.41414141414141%" headers="mcps1.1.5.1.4 "><p id="p987115282319"><a name="p987115282319"></a><a name="p987115282319"></a>查询记录数。</p>
    <p id="p118795218237"><a name="p118795218237"></a><a name="p118795218237"></a><span id="text138349551887"><a name="text138349551887"></a><a name="text138349551887"></a>最小值1，最大值1000，默认为1000。返回的结果中记录数不超过limit值。</span></p>
    </td>
    </tr>
    <tr id="row94258428238"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p3871352132317"><a name="p3871352132317"></a><a name="p3871352132317"></a>offset</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p38720529235"><a name="p38720529235"></a><a name="p38720529235"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p17737483247"><a name="p17737483247"></a><a name="p17737483247"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.41414141414141%" headers="mcps1.1.5.1.4 "><p id="p68718528233"><a name="p68718528233"></a><a name="p68718528233"></a>索引位置。</p>
    <p id="p787185218237"><a name="p787185218237"></a><a name="p787185218237"></a>最小值0，默认为0。</p>
    <p id="p387145252319"><a name="p387145252319"></a><a name="p387145252319"></a>返回的结果中第一条记录为符合查询条件的第“offset值+1”条记录。</p>
    </td>
    </tr>
    <tr id="row6793144415239"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p1687152172313"><a name="p1687152172313"></a><a name="p1687152172313"></a>action</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p1187552192314"><a name="p1187552192314"></a><a name="p1187552192314"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p97390817249"><a name="p97390817249"></a><a name="p97390817249"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.41414141414141%" headers="mcps1.1.5.1.4 "><p id="p987652192316"><a name="p987652192316"></a><a name="p987652192316"></a>操作标识。</p>
    <p id="p118795202312"><a name="p118795202312"></a><a name="p118795202312"></a>根据标签查询云硬盘实例详情时使用“filter”。</p>
    </td>
    </tr>
    <tr id="row8888748016"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p159133101403"><a name="p159133101403"></a><a name="p159133101403"></a>matches</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p1623519196018"><a name="p1623519196018"></a><a name="p1623519196018"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p109131110706"><a name="p109131110706"></a><a name="p109131110706"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="41.41414141414141%" headers="mcps1.1.5.1.4 "><p id="p129139109019"><a name="p129139109019"></a><a name="p129139109019"></a>资源本身支持的查询条件，请参见<a href="#li15751146383">•match参数数据结构说明</a>。</p>
    <p id="p1547919526720"><a name="p1547919526720"></a><a name="p1547919526720"></a>标签列表中的标签key值不允许重复。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li8528152083214"></a>resource\_tag参数数据结构说明

    <a name="table205290203323"></a>
    <table><thead align="left"><tr id="row13530142033210"><th class="cellrowborder" valign="top" width="16.161616161616163%" id="mcps1.1.5.1.1"><p id="p19530182011329"><a name="p19530182011329"></a><a name="p19530182011329"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.5.1.2"><p id="p20530120163211"><a name="p20530120163211"></a><a name="p20530120163211"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.222222222222225%" id="mcps1.1.5.1.3"><p id="p8530122014321"><a name="p8530122014321"></a><a name="p8530122014321"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="40.40404040404041%" id="mcps1.1.5.1.4"><p id="p18533172017325"><a name="p18533172017325"></a><a name="p18533172017325"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row253510208321"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p17535320203220"><a name="p17535320203220"></a><a name="p17535320203220"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p175351020123212"><a name="p175351020123212"></a><a name="p175351020123212"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.3 "><p id="p953522010321"><a name="p953522010321"></a><a name="p953522010321"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.40404040404041%" headers="mcps1.1.5.1.4 "><p id="p1520310020114"><a name="p1520310020114"></a><a name="p1520310020114"></a>标签键。</p>
    </td>
    </tr>
    <tr id="row853810204325"><td class="cellrowborder" valign="top" width="16.161616161616163%" headers="mcps1.1.5.1.1 "><p id="p1053816201325"><a name="p1053816201325"></a><a name="p1053816201325"></a>values</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.2 "><p id="p13538520153211"><a name="p13538520153211"></a><a name="p13538520153211"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.222222222222225%" headers="mcps1.1.5.1.3 "><p id="p1538920193219"><a name="p1538920193219"></a><a name="p1538920193219"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="40.40404040404041%" headers="mcps1.1.5.1.4 "><p id="p945418465250"><a name="p945418465250"></a><a name="p945418465250"></a>标签值。</p>
    <a name="ul133722079613"></a><a name="ul133722079613"></a><ul id="ul133722079613"><li>标签列表中最多包含10个value。</li><li>标签列表中的标签value值不允许重复。</li><li>标签列表如果为空列表，表示匹配任意值。标签列表中多个value之间是“或”的关系，在key已经满足要求的前提下，云硬盘满足请求中的某个value就会匹配出来。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li15751146383"></a>match参数数据结构说明

    <a name="table0778462086"></a>
    <table><thead align="left"><tr id="row38414461289"><th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.1"><p id="p1487946584"><a name="p1487946584"></a><a name="p1487946584"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21%" id="mcps1.1.5.1.2"><p id="p119224615820"><a name="p119224615820"></a><a name="p119224615820"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="p194174619818"><a name="p194174619818"></a><a name="p194174619818"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="41%" id="mcps1.1.5.1.4"><p id="p109604613817"><a name="p109604613817"></a><a name="p109604613817"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14989461387"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p810194617814"><a name="p810194617814"></a><a name="p810194617814"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="p17102646681"><a name="p17102646681"></a><a name="p17102646681"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p131037466813"><a name="p131037466813"></a><a name="p131037466813"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="41%" headers="mcps1.1.5.1.4 "><p id="p12710163971119"><a name="p12710163971119"></a><a name="p12710163971119"></a>键。枚举值。</p>
    <p id="p1110654618817"><a name="p1110654618817"></a><a name="p1110654618817"></a>key取值范围为：</p>
    <a name="ul168395111111"></a><a name="ul168395111111"></a><ul id="ul168395111111"><li>resource_name：资源名称。</li><li>service_type：服务类型。</li></ul>
    </td>
    </tr>
    <tr id="row81181246181"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.1 "><p id="p111201646386"><a name="p111201646386"></a><a name="p111201646386"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="21%" headers="mcps1.1.5.1.2 "><p id="p7121346287"><a name="p7121346287"></a><a name="p7121346287"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p1122164618815"><a name="p1122164618815"></a><a name="p1122164618815"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="41%" headers="mcps1.1.5.1.4 "><p id="p91249461180"><a name="p91249461180"></a><a name="p91249461180"></a>值。</p>
    <a name="ul1956812345128"></a><a name="ul1956812345128"></a><ul id="ul1956812345128"><li>最大长度255个字符。</li><li>key为“resource_name”时，value为模糊匹配。</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "offset": "100", 
        "limit": "100", 
        "action": "filter", 
        "tags": [
            {
                "key": "key1", 
                "values": [
                    "value1", 
                    "value2"
                ]
            }
        ], 
        "matches": [
            {
                "key": "resource_name", 
                "value": "resource1"
            }, 
            {
                "key": "service_type", 
                "value": "EVS"
            }
        ]
    }
    ```


## 响应消息<a name="section3215934016935"></a>

-   响应参数

    <a name="table716338716935"></a>
    <table><thead align="left"><tr id="row2937460716935"><th class="cellrowborder" valign="top" width="22.37%" id="mcps1.1.4.1.1"><p id="p3053299616935"><a name="p3053299616935"></a><a name="p3053299616935"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.74%" id="mcps1.1.4.1.2"><p id="p5725363416935"><a name="p5725363416935"></a><a name="p5725363416935"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.89%" id="mcps1.1.4.1.3"><p id="p3278200616935"><a name="p3278200616935"></a><a name="p3278200616935"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row63271571172633"><td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.1.4.1.1 "><p id="p24723652172633"><a name="p24723652172633"></a><a name="p24723652172633"></a>total_count</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.1.4.1.2 "><p id="p56458834172633"><a name="p56458834172633"></a><a name="p56458834172633"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.89%" headers="mcps1.1.4.1.3 "><p id="p52593571172633"><a name="p52593571172633"></a><a name="p52593571172633"></a>符合查询条件的云硬盘资源个数</p>
    </td>
    </tr>
    <tr id="row96879441311"><td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.1.4.1.1 "><p id="p261775003110"><a name="p261775003110"></a><a name="p261775003110"></a>resources</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.1.4.1.2 "><p id="p1361765083118"><a name="p1361765083118"></a><a name="p1361765083118"></a>List&lt;resource&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.89%" headers="mcps1.1.4.1.3 "><p id="p06172508319"><a name="p06172508319"></a><a name="p06172508319"></a>符合查询条件的资源列表，请参见<a href="#li95931326163214">•resource参数数据结构说明</a>。</p>
    </td>
    </tr>
    <tr id="row961262962717"><td class="cellrowborder" valign="top" width="22.37%" headers="mcps1.1.4.1.1 "><p id="p129522216412"><a name="p129522216412"></a><a name="p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.74%" headers="mcps1.1.4.1.2 "><p id="p1595262111415"><a name="p1595262111415"></a><a name="p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.89%" headers="mcps1.1.4.1.3 "><p id="p109527215417"><a name="p109527215417"></a><a name="p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li95931326163214"></a>resource参数数据结构说明

    <a name="table8575132033210"></a>
    <table><thead align="left"><tr id="row156391220173215"><th class="cellrowborder" valign="top" width="23.380000000000003%" id="mcps1.1.4.1.1"><p id="p1963910206321"><a name="p1963910206321"></a><a name="p1963910206321"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="19.48%" id="mcps1.1.4.1.2"><p id="p18639920103214"><a name="p18639920103214"></a><a name="p18639920103214"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p176391320153219"><a name="p176391320153219"></a><a name="p176391320153219"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row106392209321"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p6639920143219"><a name="p6639920143219"></a><a name="p6639920143219"></a>resource_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.48%" headers="mcps1.1.4.1.2 "><p id="p1864042093215"><a name="p1864042093215"></a><a name="p1864042093215"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p17640112015324"><a name="p17640112015324"></a><a name="p17640112015324"></a>资源ID</p>
    </td>
    </tr>
    <tr id="row964062083211"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p2640152023219"><a name="p2640152023219"></a><a name="p2640152023219"></a>resource_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.48%" headers="mcps1.1.4.1.2 "><p id="p3640720123212"><a name="p3640720123212"></a><a name="p3640720123212"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1964019207321"><a name="p1964019207321"></a><a name="p1964019207321"></a>资源名称</p>
    </td>
    </tr>
    <tr id="row116403209327"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p1664015207321"><a name="p1664015207321"></a><a name="p1664015207321"></a>resource_detail</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.48%" headers="mcps1.1.4.1.2 "><p id="p11640192033218"><a name="p11640192033218"></a><a name="p11640192033218"></a>object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1640520123214"><a name="p1640520123214"></a><a name="p1640520123214"></a>资源详情，请参见<a href="查询单个云硬盘详情-API-v2.md">查询单个云硬盘详情</a>响应中的volume参数说明表格。</p>
    </td>
    </tr>
    <tr id="row56401020193215"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p1964012013217"><a name="p1964012013217"></a><a name="p1964012013217"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.48%" headers="mcps1.1.4.1.2 "><p id="p19640142093213"><a name="p19640142093213"></a><a name="p19640142093213"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p1640120143218"><a name="p1640120143218"></a><a name="p1640120143218"></a>标签列表，请参见<a href="#li3876131217349">•resource_tag参数数据结构说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li3876131217349"></a>resource\_tag参数数据结构说明

    <a name="table198791012123412"></a>
    <table><thead align="left"><tr id="row8889141218341"><th class="cellrowborder" valign="top" width="23.380000000000003%" id="mcps1.1.4.1.1"><p id="p68931812203414"><a name="p68931812203414"></a><a name="p68931812203414"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.78%" id="mcps1.1.4.1.2"><p id="p2089701233414"><a name="p2089701233414"></a><a name="p2089701233414"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.84%" id="mcps1.1.4.1.3"><p id="p390341263413"><a name="p390341263413"></a><a name="p390341263413"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14906111253419"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p3909112163416"><a name="p3909112163416"></a><a name="p3909112163416"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.4.1.2 "><p id="p1912161283417"><a name="p1912161283417"></a><a name="p1912161283417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.1.4.1.3 "><p id="p2866151481"><a name="p2866151481"></a><a name="p2866151481"></a>标签键。</p>
    </td>
    </tr>
    <tr id="row39391412103418"><td class="cellrowborder" valign="top" width="23.380000000000003%" headers="mcps1.1.4.1.1 "><p id="p179412125347"><a name="p179412125347"></a><a name="p179412125347"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.78%" headers="mcps1.1.4.1.2 "><p id="p159431312163417"><a name="p159431312163417"></a><a name="p159431312163417"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.1.4.1.3 "><p id="p92449569473"><a name="p92449569473"></a><a name="p92449569473"></a>标签值。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li0419202382514"></a>error参数说明

    <a name="zh-cn_topic_0020235144_table15441099103019"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0020235144_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0020235144_p19541716103019"><a name="zh-cn_topic_0020235144_p19541716103019"></a><a name="zh-cn_topic_0020235144_p19541716103019"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0020235144_p39375186103019"><a name="zh-cn_topic_0020235144_p39375186103019"></a><a name="zh-cn_topic_0020235144_p39375186103019"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0020235144_p38578950103019"><a name="zh-cn_topic_0020235144_p38578950103019"></a><a name="zh-cn_topic_0020235144_p38578950103019"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0020235144_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p46815658103019"><a name="zh-cn_topic_0020235144_p46815658103019"></a><a name="zh-cn_topic_0020235144_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p33971979103019"><a name="zh-cn_topic_0020235144_p33971979103019"></a><a name="zh-cn_topic_0020235144_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p21623243103019"><a name="zh-cn_topic_0020235144_p21623243103019"></a><a name="zh-cn_topic_0020235144_p21623243103019"></a>出现错误时，返回的错误消息。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0020235144_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0020235144_p59870541103019"><a name="zh-cn_topic_0020235144_p59870541103019"></a><a name="zh-cn_topic_0020235144_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0020235144_p17675690103019"><a name="zh-cn_topic_0020235144_p17675690103019"></a><a name="zh-cn_topic_0020235144_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0020235144_p6087468103019"><a name="zh-cn_topic_0020235144_p6087468103019"></a><a name="zh-cn_topic_0020235144_p6087468103019"></a>出现错误时，返回的错误码。</p>
    <p id="zh-cn_topic_0020235144_p54787218103019"><a name="zh-cn_topic_0020235144_p54787218103019"></a><a name="zh-cn_topic_0020235144_p54787218103019"></a>错误码和其对应的含义请参考<a href="错误码说明.md">错误码说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
    	"total_count": 1,
    	"resources": [{
    		"resource_name": "resource1",
    		"resource_detail": {
    			"attachments": [{
    				"server_id": "2080869e-ba46-4ea5-b45e-3191ac0f1d54",
    				"attachment_id": "1335f039-7a42-4d1e-be49-ac584db0ba0b",
    				"attached_at": "2019-08-06T07:00:21.842812",
    				"host_name": null,
    				"volume_id": "7fa6b592-ac75-460d-a28a-bb17429d1eb2",
    				"device": "/dev/vda",
    				"id": "7fa6b592-ac75-460d-a28a-bb17429d1eb2"
    			}],
    			"links": [{
    				"href": "https://volume.Region.dc1.domainname.com/v2/051375756c80d5eb2ff0c014498645fb/volumes/7fa6b592-ac75-460d-a28a-bb17429d1eb2",
    				"rel": "self"
    			},
    			{
    				"href": "https://volume.Region.dc1.domainname.com/051375756c80d5eb2ff0c014498645fb/volumes/7fa6b592-ac75-460d-a28a-bb17429d1eb2",
    				"rel": "bookmark"
    			}],
    			"availability_zone": "kvmxen.dc1",
    			"os-vol-host-attr:host": "az21.dc1#2",
    			"encrypted": false,
    			"dedicated_storage_id": null,
    			"enterprise_project_id": "0",
    			"updated_at": "2019-08-09T06:19:35.874737",
    			"os-volume-replication:extended_status": null,
    			"replication_status": "disabled",
    			"snapshot_id": null,
    			"id": "7fa6b592-ac75-460d-a28a-bb17429d1eb2",
    			"size": 40,
    			"user_id": "75f26e17348643bfb7718578b04635c2",
    			"os-vol-tenant-attr:tenant_id": "051375756c80d5eb2ff0c014498645fb",
    			"service_type": "EVS",
    			"os-vol-mig-status-attr:migstat": null,
    			"metadata": {
    				
    			},
    			"status": "in-use",
    			"volume_image_metadata": {
    				"size": "0",
    				"__quick_start": "False",
    				"container_format": "bare",
    				"min_ram": "0",
    				"image_name": "test-hua-centos7.3-0725",
    				"image_id": "c6c153a6-dde8-4bac-8e40-3d7619436934",
    				"__os_type": "Linux",
    				"min_disk": "20",
    				"__support_kvm": "true",
    				"virtual_env_type": "FusionCompute",
    				"__description": "",
    				"__os_version": "CentOS 7.3 64bit",
    				"__os_bit": "64",
    				"__image_source_type": "uds",
    				"__support_xen": "true",
    				"file_format": "zvhd2",
    				"checksum": "d41d8cd98f00b204e9800998ecf8427e",
    				"__imagetype": "gold",
    				"disk_format": "zvhd2",
    				"__image_cache_type": "Not_Cache",
    				"__isregistered": "true",
    				"__image_location": "192.168.46.200:5443:pcsimsregion:c6c153a6-dde8-4bac-8e40-3d7619436934",
    				"__image_size": "911269888",
    				"__platform": "CentOS"
    			},
    			"description": "",
    			"multiattach": false,
    			"source_volid": null,
    			"consistencygroup_id": null,
    			"os-vol-mig-status-attr:name_id": null,
    			"name": "resource1",
    			"bootable": "true",
    			"created_at": "2019-08-06T06:59:03.056682",
    			"volume_type": "SAS",
    			"shareable": false,
    			"dedicated_storage_name": null
    		},
    		"tags": [{
    			"key": "key1",
    			"value": "value1"
    		},
    		{
    			"key": "key1",
    			"value": "value2"
    		}],
    		"resource_id": "7fa6b592-ac75-460d-a28a-bb17429d1eb2"
    	}]
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
        "computeFault": {
            "message": "The server has either erred or is incapable of performing the requested operation.", 
            "code": 500
        }
    }
    ```


## 状态码<a name="section6050296116935"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

