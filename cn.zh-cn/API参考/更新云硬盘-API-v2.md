# 更新云硬盘<a name="zh-cn_topic_0020235147"></a>

## 功能介绍<a name="section41753265"></a>

更新一个云硬盘的名称和描述。支持企业项目授权功能。

## URI<a name="section40235071"></a>

-   URI格式

    PUT /v2/\{project\_id\}/cloudvolumes/\{volume\_id\}

-   参数说明

    <a name="table21989419"></a>
    <table><thead align="left"><tr id="row9690616"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.4.1.1"><p id="p46742451"><a name="p46742451"></a><a name="p46742451"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="27%" id="mcps1.1.4.1.2"><p id="p28042199"><a name="p28042199"></a><a name="p28042199"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.4.1.3"><p id="p56825610"><a name="p56825610"></a><a name="p56825610"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row39471735"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.4.1.1 "><p id="p43093956"><a name="p43093956"></a><a name="p43093956"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.4.1.2 "><p id="p949529"><a name="p949529"></a><a name="p949529"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.4.1.3 "><p id="p9803039"><a name="p9803039"></a><a name="p9803039"></a>项目ID。</p>
    <p id="p55811451337"><a name="p55811451337"></a><a name="p55811451337"></a>获取方法请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
    </td>
    </tr>
    <tr id="row21118492"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.4.1.1 "><p id="p32876269"><a name="p32876269"></a><a name="p32876269"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.4.1.2 "><p id="p45732164"><a name="p45732164"></a><a name="p45732164"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.4.1.3 "><p id="p13317766"><a name="p13317766"></a><a name="p13317766"></a>云硬盘ID。</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求消息<a name="section26571327"></a>

-   请求参数

    <a name="table56177481416"></a>
    <table><thead align="left"><tr id="row19617104815119"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p106178485120"><a name="p106178485120"></a><a name="p106178485120"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p1361817480115"><a name="p1361817480115"></a><a name="p1361817480115"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p161813481016"><a name="p161813481016"></a><a name="p161813481016"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p76189487116"><a name="p76189487116"></a><a name="p76189487116"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row146181485120"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p1261817484111"><a name="p1261817484111"></a><a name="p1261817484111"></a>volume</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p1061818481218"><a name="p1061818481218"></a><a name="p1061818481218"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p176183483115"><a name="p176183483115"></a><a name="p176183483115"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p20618248316"><a name="p20618248316"></a><a name="p20618248316"></a>待修改的云硬盘信息，请参见<a href="#li44975500">•volume参数说明</a>。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   <a name="li44975500"></a>volume参数说明

    <a name="table2126321"></a>
    <table><thead align="left"><tr id="row49924131"><th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.1"><p id="p37408856172245"><a name="p37408856172245"></a><a name="p37408856172245"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="18%" id="mcps1.1.5.1.2"><p id="p11847581"><a name="p11847581"></a><a name="p11847581"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="16%" id="mcps1.1.5.1.3"><p id="p20130041"><a name="p20130041"></a><a name="p20130041"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="48%" id="mcps1.1.5.1.4"><p id="p19920592"><a name="p19920592"></a><a name="p19920592"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row45067606"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p26597492"><a name="p26597492"></a><a name="p26597492"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p6913218"><a name="p6913218"></a><a name="p6913218"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p10871744171339"><a name="p10871744171339"></a><a name="p10871744171339"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p30183810114010"><a name="p30183810114010"></a><a name="p30183810114010"></a>新的云硬盘的名字，name和description不能同时为null。<span id="text13527029102829"><a name="text13527029102829"></a><a name="text13527029102829"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    <tr id="row62503562"><td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.1 "><p id="p29623765"><a name="p29623765"></a><a name="p29623765"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="18%" headers="mcps1.1.5.1.2 "><p id="p50714740"><a name="p50714740"></a><a name="p50714740"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="16%" headers="mcps1.1.5.1.3 "><p id="p14253264"><a name="p14253264"></a><a name="p14253264"></a>否</p>
    </td>
    <td class="cellrowborder" valign="top" width="48%" headers="mcps1.1.5.1.4 "><p id="p66104967114034"><a name="p66104967114034"></a><a name="p66104967114034"></a>新的云硬盘的描述，name和description不能同时为null。<span id="text30454448102841"><a name="text30454448102841"></a><a name="text30454448102841"></a>最大支持255个字节。</span></p>
    </td>
    </tr>
    </tbody>
    </table>


-   请求样例

    ```
    {
        "volume": {
            "name": "test_volume", 
            "description": "test"
        }
    }
    ```


## 响应消息<a name="section37815352"></a>

-   响应参数

    <a name="table27929698142532"></a>
    <table><thead align="left"><tr id="row42153167142532"><th class="cellrowborder" valign="top" width="21.18%" id="mcps1.1.4.1.1"><p id="p58963386142532"><a name="p58963386142532"></a><a name="p58963386142532"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.35%" id="mcps1.1.4.1.2"><p id="p11304974142532"><a name="p11304974142532"></a><a name="p11304974142532"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.47%" id="mcps1.1.4.1.3"><p id="p16640014142532"><a name="p16640014142532"></a><a name="p16640014142532"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row5663883142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p56121360142532"><a name="p56121360142532"></a><a name="p56121360142532"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p49536326142532"><a name="p49536326142532"></a><a name="p49536326142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p66719203142532"><a name="p66719203142532"></a><a name="p66719203142532"></a><span id="text193761052172315"><a name="text193761052172315"></a><a name="text193761052172315"></a>云硬盘的ID。</span></p>
    </td>
    </tr>
    <tr id="row63601923142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p51482101142532"><a name="p51482101142532"></a><a name="p51482101142532"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p9300668142532"><a name="p9300668142532"></a><a name="p9300668142532"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p19730920142532"><a name="p19730920142532"></a><a name="p19730920142532"></a>云硬盘uri自描述信息，请参见<a href="#li949885516582">•links参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row43360557142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p22544263142532"><a name="p22544263142532"></a><a name="p22544263142532"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p14146042142532"><a name="p14146042142532"></a><a name="p14146042142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p624200142532"><a name="p624200142532"></a><a name="p624200142532"></a>云硬盘名称。</p>
    </td>
    </tr>
    <tr id="row5617804142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p52389016142532"><a name="p52389016142532"></a><a name="p52389016142532"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p15651871142532"><a name="p15651871142532"></a><a name="p15651871142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p15368644142532"><a name="p15368644142532"></a><a name="p15368644142532"></a>云硬盘状态，具体请参见<a href="云硬盘状态.md">云硬盘状态</a>。</p>
    </td>
    </tr>
    <tr id="row4100073142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p63670463142532"><a name="p63670463142532"></a><a name="p63670463142532"></a>attachments</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p57033878142532"><a name="p57033878142532"></a><a name="p57033878142532"></a>Array of objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p250469142532"><a name="p250469142532"></a><a name="p250469142532"></a>云硬盘的挂载信息，请参见<a href="#li2847936164017">•attachments参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row2254227142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p48374687142532"><a name="p48374687142532"></a><a name="p48374687142532"></a>availability_zone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p26035535142532"><a name="p26035535142532"></a><a name="p26035535142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p27087292142532"><a name="p27087292142532"></a><a name="p27087292142532"></a>云硬盘所属的AZ信息。</p>
    </td>
    </tr>
    <tr id="row42459044142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p16630559142532"><a name="p16630559142532"></a><a name="p16630559142532"></a>source_volid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p4898051142532"><a name="p4898051142532"></a><a name="p4898051142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p58075939142532"><a name="p58075939142532"></a><a name="p58075939142532"></a>源云硬盘ID，如果是从源云硬盘创建，则有值。</p>
    <p id="p48931232104211"><a name="p48931232104211"></a><a name="p48931232104211"></a><span id="text88578719717"><a name="text88578719717"></a><a name="text88578719717"></a>当前云硬盘服务不支持该字段。</span></p>
    </td>
    </tr>
    <tr id="row52921406142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p58775474142532"><a name="p58775474142532"></a><a name="p58775474142532"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p63192947142532"><a name="p63192947142532"></a><a name="p63192947142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p10363897142532"><a name="p10363897142532"></a><a name="p10363897142532"></a>快照ID，如果是从快照创建，则有值。</p>
    </td>
    </tr>
    <tr id="row26166216142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p39088784142532"><a name="p39088784142532"></a><a name="p39088784142532"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p12074920142532"><a name="p12074920142532"></a><a name="p12074920142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p35091945142532"><a name="p35091945142532"></a><a name="p35091945142532"></a>云硬盘描述。</p>
    </td>
    </tr>
    <tr id="row47392053142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p13551098142532"><a name="p13551098142532"></a><a name="p13551098142532"></a>os-vol-tenant-attr:tenant_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p23897139142532"><a name="p23897139142532"></a><a name="p23897139142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p22825763142532"><a name="p22825763142532"></a><a name="p22825763142532"></a>云硬盘所属的租户ID，当前该参数返回值无效。<span id="text19941457165313"><a name="text19941457165313"></a><a name="text19941457165313"></a>租户ID就是项目ID。</span></p>
    </td>
    </tr>
    <tr id="row4105277142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p64092025142532"><a name="p64092025142532"></a><a name="p64092025142532"></a>volume_image_metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p24071533142532"><a name="p24071533142532"></a><a name="p24071533142532"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p26176672142532"><a name="p26176672142532"></a><a name="p26176672142532"></a>云硬盘镜像的元数据，当前该参数返回值无效。</p>
    <div class="note" id="note1151018162014"><a name="note1151018162014"></a><a name="note1151018162014"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p16054517146"><a name="p16054517146"></a><a name="p16054517146"></a>关于“volume_image_metadata”字段的详细说明，具体请参见<a href="https://support.huaweicloud.com/api-ims/zh-cn_topic_0020091566.html" target="_blank" rel="noopener noreferrer">查询镜像详情（OpenStack原生）</a>。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row34263457142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p23876638142532"><a name="p23876638142532"></a><a name="p23876638142532"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p54959544142532"><a name="p54959544142532"></a><a name="p54959544142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p13644385142532"><a name="p13644385142532"></a><a name="p13644385142532"></a>云硬盘创建时间。</p>
    <p id="p4374122920318"><a name="p4374122920318"></a><a name="p4374122920318"></a><span id="text15641134183120"><a name="text15641134183120"></a><a name="text15641134183120"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row55690602142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p14644931142532"><a name="p14644931142532"></a><a name="p14644931142532"></a>volume_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p45388732142532"><a name="p45388732142532"></a><a name="p45388732142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p47786148539"><a name="zh-cn_topic_0098680634_p47786148539"></a><a name="zh-cn_topic_0098680634_p47786148539"></a>云硬盘类型。</p>
    <div class="p" id="zh-cn_topic_0044524833_p112762317377"><a name="zh-cn_topic_0044524833_p112762317377"></a><a name="zh-cn_topic_0044524833_p112762317377"></a>目前支持“SSD”，“SAS”和“SATA”三种。<a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><a name="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"></a><ul id="zh-cn_topic_0044524833_zh-cn_topic_0044524833_zh-cn_topic_0058762427_ul4378238815463"><li>“SSD”为超高IO云硬盘</li><li>“SAS”为高IO云硬盘</li><li>“SATA”为普通IO云硬盘</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row32535337142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p18116679142532"><a name="p18116679142532"></a><a name="p18116679142532"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p58164905142532"><a name="p58164905142532"></a><a name="p58164905142532"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p38946139142532"><a name="p38946139142532"></a><a name="p38946139142532"></a>云硬盘大小，单位为GB。</p>
    </td>
    </tr>
    <tr id="row14970936142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p4686293142532"><a name="p4686293142532"></a><a name="p4686293142532"></a>bootable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p44045434142532"><a name="p44045434142532"></a><a name="p44045434142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_p8780414125315"><a name="zh-cn_topic_0098680634_p8780414125315"></a><a name="zh-cn_topic_0098680634_p8780414125315"></a>是否为启动云硬盘。<a name="ul185931714111"></a><a name="ul185931714111"></a><ul id="ul185931714111"><li>true：表示为启动云硬盘。</li><li>false：表示为非启动云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row34847734142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p4094237142532"><a name="p4094237142532"></a><a name="p4094237142532"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p63197743142532"><a name="p63197743142532"></a><a name="p63197743142532"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p41834554142532"><a name="p41834554142532"></a><a name="p41834554142532"></a>云硬盘的元数据，请参见<a href="#li6221175494947">•metadata参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row40966670142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p29965975142532"><a name="p29965975142532"></a><a name="p29965975142532"></a>os-vol-host-attr:host</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p11324945142532"><a name="p11324945142532"></a><a name="p11324945142532"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p13457143142532"><a name="p13457143142532"></a><a name="p13457143142532"></a><span id="text203605127103"><a name="text203605127103"></a><a name="text203605127103"></a>预留属性。</span></p>
    </td>
    </tr>
    <tr id="row2027692114591"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p48928701145954"><a name="p48928701145954"></a><a name="p48928701145954"></a>shareable</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p3801857145954"><a name="p3801857145954"></a><a name="p3801857145954"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="p46595553145954"><a name="p46595553145954"></a><a name="p46595553145954"></a>是否为共享云硬盘。</p>
    <div class="note" id="note3800959821323"><a name="note3800959821323"></a><a name="note3800959821323"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p45212589213213"><a name="p45212589213213"></a><a name="p45212589213213"></a>该字段已经废弃，请使用multiattach。</p>
    </div></div>
    </td>
    </tr>
    <tr id="row54005424142532"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0044524833_p129522216412"><a name="zh-cn_topic_0044524833_p129522216412"></a><a name="zh-cn_topic_0044524833_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0044524833_p1595262111415"><a name="zh-cn_topic_0044524833_p1595262111415"></a><a name="zh-cn_topic_0044524833_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0044524833_p109527215417"><a name="zh-cn_topic_0044524833_p109527215417"></a><a name="zh-cn_topic_0044524833_p109527215417"></a>出现错误时，返回的错误信息，具体请参见<a href="#li0419202382514">•error参数说明</a>。</p>
    </td>
    </tr>
    <tr id="row36470043213458"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="p3792196213528"><a name="p3792196213528"></a><a name="p3792196213528"></a>multiattach</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="p38732436213528"><a name="p38732436213528"></a><a name="p38732436213528"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0098680634_p4781191416535"><a name="zh-cn_topic_0098680634_p4781191416535"></a><a name="zh-cn_topic_0098680634_p4781191416535"></a>是否为共享云硬盘。<a name="ul161621719119"></a><a name="ul161621719119"></a><ul id="ul161621719119"><li>true：表示为共享云硬盘。</li><li>false：表示为非共享云硬盘。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row9244758141817"><td class="cellrowborder" valign="top" width="21.18%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0098680634_p978017142534"><a name="zh-cn_topic_0098680634_p978017142534"></a><a name="zh-cn_topic_0098680634_p978017142534"></a>os-volume-replication:extended_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.35%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0098680634_p12780191455320"><a name="zh-cn_topic_0098680634_p12780191455320"></a><a name="zh-cn_topic_0098680634_p12780191455320"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.47%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0098680634_p278051495317"><a name="zh-cn_topic_0098680634_p278051495317"></a><a name="zh-cn_topic_0098680634_p278051495317"></a><span id="text379518478151"><a name="text379518478151"></a><a name="text379518478151"></a>预留属性。</span></p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li949885516582"></a>links参数说明

    <a name="table44453603165834"></a>
    <table><thead align="left"><tr id="row67020808165834"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="p59976390165834"><a name="p59976390165834"></a><a name="p59976390165834"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="p43343669105259"><a name="p43343669105259"></a><a name="p43343669105259"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="p45826298165834"><a name="p45826298165834"></a><a name="p45826298165834"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row20942657165834"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p18633648165834"><a name="p18633648165834"></a><a name="p18633648165834"></a>href</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p21176318105259"><a name="p21176318105259"></a><a name="p21176318105259"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p50128425165834"><a name="p50128425165834"></a><a name="p50128425165834"></a>对应的快捷链接。</p>
    </td>
    </tr>
    <tr id="row48502642165834"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="p36399890165834"><a name="p36399890165834"></a><a name="p36399890165834"></a>rel</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="p37560167105259"><a name="p37560167105259"></a><a name="p37560167105259"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="p46341215165834"><a name="p46341215165834"></a><a name="p46341215165834"></a>快捷链接标记名称。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li2847936164017"></a>attachments参数说明

    <a name="table3307491164033"></a>
    <table><thead align="left"><tr id="row21424691164033"><th class="cellrowborder" valign="top" width="21.687831216878315%" id="mcps1.1.4.1.1"><p id="p57678439164033"><a name="p57678439164033"></a><a name="p57678439164033"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.687831216878315%" id="mcps1.1.4.1.2"><p id="p66852304105349"><a name="p66852304105349"></a><a name="p66852304105349"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.624337566243376%" id="mcps1.1.4.1.3"><p id="p1357476164033"><a name="p1357476164033"></a><a name="p1357476164033"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row42846717164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p48032051164033"><a name="p48032051164033"></a><a name="p48032051164033"></a>server_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p46327539105349"><a name="p46327539105349"></a><a name="p46327539105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p62170963164033"><a name="p62170963164033"></a><a name="p62170963164033"></a>云硬盘挂载到的云服务器的ID。</p>
    </td>
    </tr>
    <tr id="row22667763164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p24149511164033"><a name="p24149511164033"></a><a name="p24149511164033"></a>attachment_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p61543187105349"><a name="p61543187105349"></a><a name="p61543187105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p919418164033"><a name="p919418164033"></a><a name="p919418164033"></a>挂载信息对应的ID。</p>
    </td>
    </tr>
    <tr id="row57853019113651"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p50055523113657"><a name="p50055523113657"></a><a name="p50055523113657"></a>attached_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p27965571113657"><a name="p27965571113657"></a><a name="p27965571113657"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p6478808113657"><a name="p6478808113657"></a><a name="p6478808113657"></a>挂载的时间信息。</p>
    <p id="p692624863119"><a name="p692624863119"></a><a name="p692624863119"></a><span id="text13941449123112"><a name="text13941449123112"></a><a name="text13941449123112"></a>时间格式：UTC YYYY-MM-DDTHH:MM:SS.XXXXXX</span></p>
    </td>
    </tr>
    <tr id="row8274763164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p66276072164033"><a name="p66276072164033"></a><a name="p66276072164033"></a>host_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p18942231105349"><a name="p18942231105349"></a><a name="p18942231105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p38983264164033"><a name="p38983264164033"></a><a name="p38983264164033"></a>云硬盘挂载到的云服务器对应的物理主机的名称。</p>
    </td>
    </tr>
    <tr id="row15305060164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p31750372164033"><a name="p31750372164033"></a><a name="p31750372164033"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p57925736105349"><a name="p57925736105349"></a><a name="p57925736105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p8281462164033"><a name="p8281462164033"></a><a name="p8281462164033"></a>云硬盘ID。</p>
    </td>
    </tr>
    <tr id="row7424294164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p64496914164033"><a name="p64496914164033"></a><a name="p64496914164033"></a>device</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p61473005105349"><a name="p61473005105349"></a><a name="p61473005105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p42870577164033"><a name="p42870577164033"></a><a name="p42870577164033"></a>挂载点。</p>
    </td>
    </tr>
    <tr id="row50290878164033"><td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.1 "><p id="p47029330164033"><a name="p47029330164033"></a><a name="p47029330164033"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.687831216878315%" headers="mcps1.1.4.1.2 "><p id="p13257486105349"><a name="p13257486105349"></a><a name="p13257486105349"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.624337566243376%" headers="mcps1.1.4.1.3 "><p id="p59986642164033"><a name="p59986642164033"></a><a name="p59986642164033"></a>挂载的资源ID。</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="li6221175494947"></a>metadata参数说明

    <a name="zh-cn_topic_0102756196_table3430728295554"></a>
    <table><thead align="left"><tr id="zh-cn_topic_0102756196_row4496975195554"><th class="cellrowborder" valign="top" width="20.24%" id="mcps1.1.4.1.1"><p id="zh-cn_topic_0102756196_p8809200174410"><a name="zh-cn_topic_0102756196_p8809200174410"></a><a name="zh-cn_topic_0102756196_p8809200174410"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.62%" id="mcps1.1.4.1.2"><p id="zh-cn_topic_0102756196_p168135017449"><a name="zh-cn_topic_0102756196_p168135017449"></a><a name="zh-cn_topic_0102756196_p168135017449"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="zh-cn_topic_0102756196_p1282213034412"><a name="zh-cn_topic_0102756196_p1282213034412"></a><a name="zh-cn_topic_0102756196_p1282213034412"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="zh-cn_topic_0102756196_row456195295554"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p1562408795622"><a name="zh-cn_topic_0102756196_p1562408795622"></a><a name="zh-cn_topic_0102756196_p1562408795622"></a>__system__encrypted</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p5759155095622"><a name="zh-cn_topic_0102756196_p5759155095622"></a><a name="zh-cn_topic_0102756196_p5759155095622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p177192813501"><a name="zh-cn_topic_0102756196_p177192813501"></a><a name="zh-cn_topic_0102756196_p177192813501"></a>metadata中的表示加密功能的字段。<a name="zh-cn_topic_0102756196_ul141951225145011"></a><a name="zh-cn_topic_0102756196_ul141951225145011"></a><ul id="zh-cn_topic_0102756196_ul141951225145011"><li>0代表不加密。</li><li>1代表加密。</li><li>该字段不存在时，云硬盘默认为不加密。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row247050109562"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p241272995622"><a name="zh-cn_topic_0102756196_p241272995622"></a><a name="zh-cn_topic_0102756196_p241272995622"></a>__system__cmkid</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p6121338895622"><a name="zh-cn_topic_0102756196_p6121338895622"></a><a name="zh-cn_topic_0102756196_p6121338895622"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0102756196_p4159804295622"><a name="zh-cn_topic_0102756196_p4159804295622"></a><a name="zh-cn_topic_0102756196_p4159804295622"></a>metadata中的加密cmkid字段，与__system__encrypted配合表示需要加密，cmkid长度固定为36个字节。</p>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row60499086104915"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p1478896104915"><a name="zh-cn_topic_0102756196_p1478896104915"></a><a name="zh-cn_topic_0102756196_p1478896104915"></a>hw:passthrough</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p52681767104915"><a name="zh-cn_topic_0102756196_p52681767104915"></a><a name="zh-cn_topic_0102756196_p52681767104915"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><div class="p" id="zh-cn_topic_0102756196_p17177177145116"><a name="zh-cn_topic_0102756196_p17177177145116"></a><a name="zh-cn_topic_0102756196_p17177177145116"></a>metadata中的表示云硬盘设备类型的字段。<a name="zh-cn_topic_0102756196_ul14462208141855"></a><a name="zh-cn_topic_0102756196_ul14462208141855"></a><ul id="zh-cn_topic_0102756196_ul14462208141855"><li>true表示云硬盘的设备类型为SCSI类型，即允许ECS操作系统直接访问底层存储介质。支持SCSI锁命令。</li><li>false表示云硬盘的设备类型为VBD类型，即为默认类型，VBD只能支持简单的SCSI读写命令。</li><li>该字段不存在时，云硬盘默认为VBD类型。</li></ul>
    </div>
    </td>
    </tr>
    <tr id="zh-cn_topic_0102756196_row991210132288"><td class="cellrowborder" valign="top" width="20.24%" headers="mcps1.1.4.1.1 "><p id="zh-cn_topic_0102756196_p3500156018292"><a name="zh-cn_topic_0102756196_p3500156018292"></a><a name="zh-cn_topic_0102756196_p3500156018292"></a>full_clone</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.62%" headers="mcps1.1.4.1.2 "><p id="zh-cn_topic_0102756196_p1655411118292"><a name="zh-cn_topic_0102756196_p1655411118292"></a><a name="zh-cn_topic_0102756196_p1655411118292"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="zh-cn_topic_0102756196_p47931946183150"><a name="zh-cn_topic_0102756196_p47931946183150"></a><a name="zh-cn_topic_0102756196_p47931946183150"></a>从快照创建云硬盘时，字段的值为0表示使用link克隆方式。</p>
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
        "id": "36ba39af-3579-4e6e-adfc-b764349c0f77", 
        "links": [
            {
                "href": "https://volume.region.xxx.xxx-tsi.de/v2/3cfb09080bd944d0b4cdd72ef26857bd/volumes/36ba39af-3579-4e6e-adfc-b764349c0f77", 
                "rel": "self"
            }, 
            {
                "href": "https://volume.region.xxx.xxx-tsi.de/3cfb09080bd944d0b4cdd72ef26857bd/volumes/36ba39af-3579-4e6e-adfc-b764349c0f77", 
                "rel": "bookmark"
            }
        ], 
        "name": "newVolume", 
        "status": "in-use", 
        "attachments": [
            {
                "server_id": "c3d3250c-7ce5-42cc-b620-dd2b63d19ca5", 
                "attachment_id": "011a2bdb-a033-4479-845b-50bd8ed7f4d4", 
                "attached_at": "2017-05-23T11:27:38.604815", 
                "host_name": null, 
                "volume_id": "36ba39af-3579-4e6e-adfc-b764349c0f77", 
                "device": "/dev/sdf", 
                "id": "36ba39af-3579-4e6e-adfc-b764349c0f77"
            }
        ], 
        "description": "new volume", 
        "multiattach": false, 
        "shareable": false, 
        "size": 10, 
        "metadata": {
            "policy": "dc71a9c9-b3fa-429d-a070-037682d82d21", 
            "attached_mode": "rw", 
            "readonly": "False", 
            "hw:passthrough": "false"
        }, 
        "bootable": "false", 
        "availability_zone": "az-dc-1", 
        "os-vol-host-attr:host": null, 
        "source_volid": null, 
        "snapshot_id": null, 
        "created_at": "2017-05-23T09:49:44.481299", 
        "volume_type": "SATA", 
        "os-vol-tenant-attr:tenant_id": null, 
        "os-volume-replication:extended_status": null,
        "volume_image_metadata": null
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


## 状态码<a name="section4793853"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

