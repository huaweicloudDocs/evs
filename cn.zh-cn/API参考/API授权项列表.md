# API授权项列表<a name="ZH-CN_TOPIC_0103526772"></a>

## 云硬盘<a name="section115958429354"></a>

<a name="table277762312153"></a>
<table><thead align="left"><tr id="row1179882321511"><th class="cellrowborder" valign="top" width="27%" id="mcps1.1.5.1.1"><p id="p1280617238151"><a name="p1280617238151"></a><a name="p1280617238151"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.1.5.1.2"><p id="p6813112311152"><a name="p6813112311152"></a><a name="p6813112311152"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.5.1.3"><p id="p108191723121517"><a name="p108191723121517"></a><a name="p108191723121517"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.1.5.1.4"><p id="p18251923181518"><a name="p18251923181518"></a><a name="p18251923181518"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row1383192320152"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p168411123121511"><a name="p168411123121511"></a><a name="p168411123121511"></a>POST /v2/{project_id}/cloudvolumes</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1848122310157"><a name="p1848122310157"></a><a name="p1848122310157"></a>创建云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1985372313157"><a name="p1985372313157"></a><a name="p1985372313157"></a>evs:volumes:create</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul13858323121517"></a><a name="ul13858323121517"></a><ul id="ul13858323121517"><li>支持：<a name="ul188661423121511"></a><a name="ul188661423121511"></a><ul id="ul188661423121511"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1088852331510"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p15893152341511"><a name="p15893152341511"></a><a name="p15893152341511"></a>POST /v2/{project_id}/volumes</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p13898122341512"><a name="p13898122341512"></a><a name="p13898122341512"></a>创建云硬盘（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><a name="ul5903182315153"></a><a name="ul5903182315153"></a><ul id="ul5903182315153"><li>创空白云硬盘<p id="p69104235153"><a name="p69104235153"></a><a name="p69104235153"></a>evs:volumes:create</p>
<p id="p041642984516"><a name="p041642984516"></a><a name="p041642984516"></a>evs:volumes:get</p>
</li><li>通过镜像创建云硬盘<p id="p3918172314157"><a name="p3918172314157"></a><a name="p3918172314157"></a>evs:volumes:create</p>
<p id="p1092172361518"><a name="p1092172361518"></a><a name="p1092172361518"></a>ims:images:get</p>
<p id="p178151131194519"><a name="p178151131194519"></a><a name="p178151131194519"></a>evs:volumes:get</p>
</li><li>通过快照创建云硬盘<p id="p14928142361517"><a name="p14928142361517"></a><a name="p14928142361517"></a>evs:volumes:create</p>
<p id="p159301423161510"><a name="p159301423161510"></a><a name="p159301423161510"></a>evs:snapshots:get</p>
<p id="p16155205374412"><a name="p16155205374412"></a><a name="p16155205374412"></a>evs:volumes:get</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul3936202310150"></a><a name="ul3936202310150"></a><ul id="ul3936202310150"><li>支持：<p id="p48451412122317"><a name="p48451412122317"></a><a name="p48451412122317"></a>项目(Project)</p>
</li><li>不支持：<p id="p69718230159"><a name="p69718230159"></a><a name="p69718230159"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row9281224111513"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p8353244153"><a name="p8353244153"></a><a name="p8353244153"></a>POST /v2/{project_id}/cloudvolumes/{volume_id}/action</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p04013248156"><a name="p04013248156"></a><a name="p04013248156"></a>扩容云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p8441224141517"><a name="p8441224141517"></a><a name="p8441224141517"></a>evs:volumes:extend</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul8129132620194"></a><a name="ul8129132620194"></a><ul id="ul8129132620194"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511"></a><a name="zh-cn_topic_0103526772_ul188661423121511"></a><ul id="zh-cn_topic_0103526772_ul188661423121511"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row71331924131514"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1913802471517"><a name="p1913802471517"></a><a name="p1913802471517"></a>GET /v2/{project_id}/cloudvolumes</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1414315240156"><a name="p1414315240156"></a><a name="p1414315240156"></a>查询云硬盘列表</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p16150122401514"><a name="p16150122401514"></a><a name="p16150122401514"></a>evs:volumes:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul1415312410150"></a><a name="ul1415312410150"></a><ul id="ul1415312410150"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317"><a name="zh-cn_topic_0103526772_p48451412122317"></a><a name="zh-cn_topic_0103526772_p48451412122317"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159"><a name="zh-cn_topic_0103526772_p69718230159"></a><a name="zh-cn_topic_0103526772_p69718230159"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1185102491518"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1819182414151"><a name="p1819182414151"></a><a name="p1819182414151"></a>GET /v2/{project_id}/volumes</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p111946244151"><a name="p111946244151"></a><a name="p111946244151"></a>查询云硬盘列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1220192411155"><a name="p1220192411155"></a><a name="p1220192411155"></a>evs:volumes:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul243702432015"></a><a name="ul243702432015"></a><ul id="ul243702432015"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_1"><a name="zh-cn_topic_0103526772_p48451412122317_1"></a><a name="zh-cn_topic_0103526772_p48451412122317_1"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_1"><a name="zh-cn_topic_0103526772_p69718230159_1"></a><a name="zh-cn_topic_0103526772_p69718230159_1"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row32341324101513"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p16239162414153"><a name="p16239162414153"></a><a name="p16239162414153"></a>GET /v2/{project_id}/cloudvolumes/detail</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1624352481513"><a name="p1624352481513"></a><a name="p1624352481513"></a>查询所有云硬盘详情</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p3251102410151"><a name="p3251102410151"></a><a name="p3251102410151"></a>evs:volumes:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul9745154522018"></a><a name="ul9745154522018"></a><ul id="ul9745154522018"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_1"></a><a name="zh-cn_topic_0103526772_ul188661423121511_1"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_1"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row728032419152"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1028615241155"><a name="p1028615241155"></a><a name="p1028615241155"></a>GET /v2/{project_id}/os-vendor-volumes/detail</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p112913248154"><a name="p112913248154"></a><a name="p112913248154"></a>分类查询所有云硬盘详情</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p9298132441516"><a name="p9298132441516"></a><a name="p9298132441516"></a>evs:volumes:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul373995952017"></a><a name="ul373995952017"></a><ul id="ul373995952017"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_2"><a name="zh-cn_topic_0103526772_p48451412122317_2"></a><a name="zh-cn_topic_0103526772_p48451412122317_2"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_2"><a name="zh-cn_topic_0103526772_p69718230159_2"></a><a name="zh-cn_topic_0103526772_p69718230159_2"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1733662417153"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p18342182420156"><a name="p18342182420156"></a><a name="p18342182420156"></a>GET /v2/{project_id}/volumes/detail</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p4348112441514"><a name="p4348112441514"></a><a name="p4348112441514"></a>查询所有云硬盘详情（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1352324171519"><a name="p1352324171519"></a><a name="p1352324171519"></a>evs:volumes:list</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul71931298219"></a><a name="ul71931298219"></a><ul id="ul71931298219"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_3"><a name="zh-cn_topic_0103526772_p48451412122317_3"></a><a name="zh-cn_topic_0103526772_p48451412122317_3"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_3"><a name="zh-cn_topic_0103526772_p69718230159_3"></a><a name="zh-cn_topic_0103526772_p69718230159_3"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row153861824191512"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p139212471518"><a name="p139212471518"></a><a name="p139212471518"></a>GET /v2/{project_id}/os-vendor-volumes/{volume_id}</p>
<p id="p1439520241153"><a name="p1439520241153"></a><a name="p1439520241153"></a></p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p340013242157"><a name="p340013242157"></a><a name="p340013242157"></a>查询单个云硬盘详情</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1540517243159"><a name="p1540517243159"></a><a name="p1540517243159"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul19593215182118"></a><a name="ul19593215182118"></a><ul id="ul19593215182118"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_4"><a name="zh-cn_topic_0103526772_p48451412122317_4"></a><a name="zh-cn_topic_0103526772_p48451412122317_4"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_4"><a name="zh-cn_topic_0103526772_p69718230159_4"></a><a name="zh-cn_topic_0103526772_p69718230159_4"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row94419241150"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p154474246158"><a name="p154474246158"></a><a name="p154474246158"></a>GET /v2/{project_id}/volumes/{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p16452224141514"><a name="p16452224141514"></a><a name="p16452224141514"></a>查询单个云硬盘详情（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p145772413152"><a name="p145772413152"></a><a name="p145772413152"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul37311226219"></a><a name="ul37311226219"></a><ul id="ul37311226219"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_5"><a name="zh-cn_topic_0103526772_p48451412122317_5"></a><a name="zh-cn_topic_0103526772_p48451412122317_5"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_5"><a name="zh-cn_topic_0103526772_p69718230159_5"></a><a name="zh-cn_topic_0103526772_p69718230159_5"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row134911724131511"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p16497102481518"><a name="p16497102481518"></a><a name="p16497102481518"></a>GET /v2/{project_id}/ cloudvolumes /{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1550213243158"><a name="p1550213243158"></a><a name="p1550213243158"></a>查询单个云硬盘详情</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p150712416152"><a name="p150712416152"></a><a name="p150712416152"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul115924632119"></a><a name="ul115924632119"></a><ul id="ul115924632119"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_2"></a><a name="zh-cn_topic_0103526772_ul188661423121511_2"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_2"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row2556182411158"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p5561924151518"><a name="p5561924151518"></a><a name="p5561924151518"></a>DELETE /v2/{project_id}/cloudvolumes/{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p19565624141519"><a name="p19565624141519"></a><a name="p19565624141519"></a>删除云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1757111240150"><a name="p1757111240150"></a><a name="p1757111240150"></a>evs:volumes:delete</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul179441752102117"></a><a name="ul179441752102117"></a><ul id="ul179441752102117"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_3"></a><a name="zh-cn_topic_0103526772_ul188661423121511_3"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_3"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row18604824121517"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p7609924101512"><a name="p7609924101512"></a><a name="p7609924101512"></a>DELETE /v2/{project_id}/volumes/{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p8614102415156"><a name="p8614102415156"></a><a name="p8614102415156"></a>删除云硬盘（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p4620152410152"><a name="p4620152410152"></a><a name="p4620152410152"></a>evs:volumes:delete</p>
<p id="p1262392451511"><a name="p1262392451511"></a><a name="p1262392451511"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul17666905226"></a><a name="ul17666905226"></a><ul id="ul17666905226"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_6"><a name="zh-cn_topic_0103526772_p48451412122317_6"></a><a name="zh-cn_topic_0103526772_p48451412122317_6"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_6"><a name="zh-cn_topic_0103526772_p69718230159_6"></a><a name="zh-cn_topic_0103526772_p69718230159_6"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row15656122416156"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p196621224151515"><a name="p196621224151515"></a><a name="p196621224151515"></a>PUT /v2/{project_id}/cloudvolumes/{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p9667202416150"><a name="p9667202416150"></a><a name="p9667202416150"></a>更新云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1967452411512"><a name="p1967452411512"></a><a name="p1967452411512"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul1599871032214"></a><a name="ul1599871032214"></a><ul id="ul1599871032214"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_4"></a><a name="zh-cn_topic_0103526772_ul188661423121511_4"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_4"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row670792413150"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p27121624141515"><a name="p27121624141515"></a><a name="p27121624141515"></a>PUT /v2/{project_id}/volumes/{volume_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p8717324111518"><a name="p8717324111518"></a><a name="p8717324111518"></a>更新云硬盘（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p10721202451517"><a name="p10721202451517"></a><a name="p10721202451517"></a>evs:volumes:update</p>
<p id="p1272392416155"><a name="p1272392416155"></a><a name="p1272392416155"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul4331923182210"></a><a name="ul4331923182210"></a><ul id="ul4331923182210"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_7"><a name="zh-cn_topic_0103526772_p48451412122317_7"></a><a name="zh-cn_topic_0103526772_p48451412122317_7"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_7"><a name="zh-cn_topic_0103526772_p69718230159_7"></a><a name="zh-cn_topic_0103526772_p69718230159_7"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row3758142414155"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1576172421515"><a name="p1576172421515"></a><a name="p1576172421515"></a>PUT /v2/{project_id}/volumes/{volume_id}/metadata/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p19768182461513"><a name="p19768182461513"></a><a name="p19768182461513"></a>更新云硬盘的单个元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p7771824101511"><a name="p7771824101511"></a><a name="p7771824101511"></a>evs:volumes:update</p>
<p id="p777492401514"><a name="p777492401514"></a><a name="p777492401514"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul12413123114226"></a><a name="ul12413123114226"></a><ul id="ul12413123114226"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_8"><a name="zh-cn_topic_0103526772_p48451412122317_8"></a><a name="zh-cn_topic_0103526772_p48451412122317_8"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_8"><a name="zh-cn_topic_0103526772_p69718230159_8"></a><a name="zh-cn_topic_0103526772_p69718230159_8"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row28051024111517"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p2081011246150"><a name="p2081011246150"></a><a name="p2081011246150"></a>PUT /v2/{project_id}/volumes/{volume_id}/metadata</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p17816924161515"><a name="p17816924161515"></a><a name="p17816924161515"></a>更新云硬盘的元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p58221324171514"><a name="p58221324171514"></a><a name="p58221324171514"></a>evs:volumes:update</p>
<p id="p1982517249156"><a name="p1982517249156"></a><a name="p1982517249156"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul724115433227"></a><a name="ul724115433227"></a><ul id="ul724115433227"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_9"><a name="zh-cn_topic_0103526772_p48451412122317_9"></a><a name="zh-cn_topic_0103526772_p48451412122317_9"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_9"><a name="zh-cn_topic_0103526772_p69718230159_9"></a><a name="zh-cn_topic_0103526772_p69718230159_9"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row685918245158"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p15863172413151"><a name="p15863172413151"></a><a name="p15863172413151"></a>GET /v2/{project_id}/volumes/{volume_id}/metadata/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p138691247154"><a name="p138691247154"></a><a name="p138691247154"></a>查询云硬盘的单个元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p78721424131514"><a name="p78721424131514"></a><a name="p78721424131514"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul1728534902217"></a><a name="ul1728534902217"></a><ul id="ul1728534902217"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_10"><a name="zh-cn_topic_0103526772_p48451412122317_10"></a><a name="zh-cn_topic_0103526772_p48451412122317_10"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_10"><a name="zh-cn_topic_0103526772_p69718230159_10"></a><a name="zh-cn_topic_0103526772_p69718230159_10"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row0906182431511"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p14914172411159"><a name="p14914172411159"></a><a name="p14914172411159"></a>DELETE /v2/{project_id}/volumes/{volume_id}/metadata/{key}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1917224111519"><a name="p1917224111519"></a><a name="p1917224111519"></a>删除云硬盘的单个元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p18922624201511"><a name="p18922624201511"></a><a name="p18922624201511"></a>evs:volumes:delete</p>
<p id="p159261124181511"><a name="p159261124181511"></a><a name="p159261124181511"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul59532547228"></a><a name="ul59532547228"></a><ul id="ul59532547228"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_11"><a name="zh-cn_topic_0103526772_p48451412122317_11"></a><a name="zh-cn_topic_0103526772_p48451412122317_11"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_11"><a name="zh-cn_topic_0103526772_p69718230159_11"></a><a name="zh-cn_topic_0103526772_p69718230159_11"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row69611824161516"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p196710242152"><a name="p196710242152"></a><a name="p196710242152"></a>GET /v2/{project_id}/volumes/{volume_id}/metadata</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p18972102411511"><a name="p18972102411511"></a><a name="p18972102411511"></a>查询云硬盘的元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p397915248159"><a name="p397915248159"></a><a name="p397915248159"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul13184121182317"></a><a name="ul13184121182317"></a><ul id="ul13184121182317"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_12"><a name="zh-cn_topic_0103526772_p48451412122317_12"></a><a name="zh-cn_topic_0103526772_p48451412122317_12"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_12"><a name="zh-cn_topic_0103526772_p69718230159_12"></a><a name="zh-cn_topic_0103526772_p69718230159_12"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row13967023185011"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p996722315012"><a name="p996722315012"></a><a name="p996722315012"></a>POST /v2/{project_id}/volumes/{volume_id}/metadata</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p6967102312503"><a name="p6967102312503"></a><a name="p6967102312503"></a>添加云硬盘的元数据（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p8107558546"><a name="p8107558546"></a><a name="p8107558546"></a>evs:volumes:update</p>
<p id="p71079583412"><a name="p71079583412"></a><a name="p71079583412"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul17289133452"></a><a name="ul17289133452"></a><ul id="ul17289133452"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_13"><a name="zh-cn_topic_0103526772_p48451412122317_13"></a><a name="zh-cn_topic_0103526772_p48451412122317_13"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_13"><a name="zh-cn_topic_0103526772_p69718230159_13"></a><a name="zh-cn_topic_0103526772_p69718230159_13"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row18121325111515"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p11715256159"><a name="p11715256159"></a><a name="p11715256159"></a>GET /v2/{project_id}/types</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p323192521519"><a name="p323192521519"></a><a name="p323192521519"></a>查询云硬盘类型列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p15281025161512"><a name="p15281025161512"></a><a name="p15281025161512"></a>evs:types:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul125294718235"></a><a name="ul125294718235"></a><ul id="ul125294718235"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_14"><a name="zh-cn_topic_0103526772_p48451412122317_14"></a><a name="zh-cn_topic_0103526772_p48451412122317_14"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_14"><a name="zh-cn_topic_0103526772_p69718230159_14"></a><a name="zh-cn_topic_0103526772_p69718230159_14"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row156318257153"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1669425131519"><a name="p1669425131519"></a><a name="p1669425131519"></a>GET /v2/{project_id}/types/{type_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p272152591513"><a name="p272152591513"></a><a name="p272152591513"></a>查询单个云硬盘类型的详细信息（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p13781125111513"><a name="p13781125111513"></a><a name="p13781125111513"></a>evs:types:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul1313871362318"></a><a name="ul1313871362318"></a><ul id="ul1313871362318"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_15"><a name="zh-cn_topic_0103526772_p48451412122317_15"></a><a name="zh-cn_topic_0103526772_p48451412122317_15"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_15"><a name="zh-cn_topic_0103526772_p69718230159_15"></a><a name="zh-cn_topic_0103526772_p69718230159_15"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row51131725111517"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p3120122511517"><a name="p3120122511517"></a><a name="p3120122511517"></a>GET /v2/{project_id}/os-quota-sets/{project_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1512517253157"><a name="p1512517253157"></a><a name="p1512517253157"></a>查询租户的详细配额（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1613142514155"><a name="p1613142514155"></a><a name="p1613142514155"></a>evs:quotas:get</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul18585121142316"></a><a name="ul18585121142316"></a><ul id="ul18585121142316"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_16"><a name="zh-cn_topic_0103526772_p48451412122317_16"></a><a name="zh-cn_topic_0103526772_p48451412122317_16"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_16"><a name="zh-cn_topic_0103526772_p69718230159_16"></a><a name="zh-cn_topic_0103526772_p69718230159_16"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1416413256152"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p10171112521515"><a name="p10171112521515"></a><a name="p10171112521515"></a>GET /v2/{project_id}/extensions</p>
<p id="p4172125191515"><a name="p4172125191515"></a><a name="p4172125191515"></a></p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p101801725111514"><a name="p101801725111514"></a><a name="p101801725111514"></a>查询扩展接口（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p71841825101510"><a name="p71841825101510"></a><a name="p71841825101510"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul1678228162311"></a><a name="ul1678228162311"></a><ul id="ul1678228162311"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_17"><a name="zh-cn_topic_0103526772_p48451412122317_17"></a><a name="zh-cn_topic_0103526772_p48451412122317_17"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_17"><a name="zh-cn_topic_0103526772_p69718230159_17"></a><a name="zh-cn_topic_0103526772_p69718230159_17"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1121512515155"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1422316257155"><a name="p1422316257155"></a><a name="p1422316257155"></a>GET /v2/{project_id}/os-availability-zone</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1222822551515"><a name="p1222822551515"></a><a name="p1222822551515"></a>查询所有的可用分区信息（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p14234102520155"><a name="p14234102520155"></a><a name="p14234102520155"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul157941934112320"></a><a name="ul157941934112320"></a><ul id="ul157941934112320"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_18"><a name="zh-cn_topic_0103526772_p48451412122317_18"></a><a name="zh-cn_topic_0103526772_p48451412122317_18"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_18"><a name="zh-cn_topic_0103526772_p69718230159_18"></a><a name="zh-cn_topic_0103526772_p69718230159_18"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row10269102551515"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p1127522518157"><a name="p1127522518157"></a><a name="p1127522518157"></a>GET /</p>
<p id="p2277152521513"><a name="p2277152521513"></a><a name="p2277152521513"></a></p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p1828102517150"><a name="p1828102517150"></a><a name="p1828102517150"></a>查询接口版本信息列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p6286172521520"><a name="p6286172521520"></a><a name="p6286172521520"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul10174103792310"></a><a name="ul10174103792310"></a><ul id="ul10174103792310"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_19"><a name="zh-cn_topic_0103526772_p48451412122317_19"></a><a name="zh-cn_topic_0103526772_p48451412122317_19"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_19"><a name="zh-cn_topic_0103526772_p69718230159_19"></a><a name="zh-cn_topic_0103526772_p69718230159_19"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row232282518152"><td class="cellrowborder" valign="top" width="27%" headers="mcps1.1.5.1.1 "><p id="p132718252155"><a name="p132718252155"></a><a name="p132718252155"></a>GET /v2</p>
<p id="p19329152510158"><a name="p19329152510158"></a><a name="p19329152510158"></a>或</p>
<p id="p143311625121519"><a name="p143311625121519"></a><a name="p143311625121519"></a>GET /v2/</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p12337725171519"><a name="p12337725171519"></a><a name="p12337725171519"></a>查询接口的v2版本信息（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.5.1.3 "><p id="p1634252581510"><a name="p1634252581510"></a><a name="p1634252581510"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.4 "><a name="ul22671942172315"></a><a name="ul22671942172315"></a><ul id="ul22671942172315"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_20"><a name="zh-cn_topic_0103526772_p48451412122317_20"></a><a name="zh-cn_topic_0103526772_p48451412122317_20"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_20"><a name="zh-cn_topic_0103526772_p69718230159_20"></a><a name="zh-cn_topic_0103526772_p69718230159_20"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 云硬盘Actions<a name="section193981335267"></a>

<a name="table11136162518266"></a>
<table><thead align="left"><tr id="row19140152562617"><th class="cellrowborder" valign="top" width="29.292929292929294%" id="mcps1.1.5.1.1"><p id="p121421125122619"><a name="p121421125122619"></a><a name="p121421125122619"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="23.232323232323235%" id="mcps1.1.5.1.2"><p id="p31531125102619"><a name="p31531125102619"></a><a name="p31531125102619"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="21.21212121212121%" id="mcps1.1.5.1.3"><p id="p6155142592612"><a name="p6155142592612"></a><a name="p6155142592612"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="26.262626262626267%" id="mcps1.1.5.1.4"><p id="p1521211509247"><a name="p1521211509247"></a><a name="p1521211509247"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row14183202592618"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p12304115454216"><a name="p12304115454216"></a><a name="p12304115454216"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p830620547428"><a name="p830620547428"></a><a name="p830620547428"></a>action="os-extend"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p1630995419425"><a name="p1630995419425"></a><a name="p1630995419425"></a>扩容云硬盘（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p1350513314414"><a name="p1350513314414"></a><a name="p1350513314414"></a>evs:volumes:extend</p>
<p id="p1938111964"><a name="p1938111964"></a><a name="p1938111964"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul13951688261"></a><a name="ul13951688261"></a><ul id="ul13951688261"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_21"><a name="zh-cn_topic_0103526772_p48451412122317_21"></a><a name="zh-cn_topic_0103526772_p48451412122317_21"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_21"><a name="zh-cn_topic_0103526772_p69718230159_21"></a><a name="zh-cn_topic_0103526772_p69718230159_21"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row7188202572612"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p175051733134113"><a name="p175051733134113"></a><a name="p175051733134113"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p150533394112"><a name="p150533394112"></a><a name="p150533394112"></a>action="os-volume_upload_image"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p14505173334110"><a name="p14505173334110"></a><a name="p14505173334110"></a>将云硬盘导出为镜像（OpenStack Cinder）</p>
<p id="p750573324115"><a name="p750573324115"></a><a name="p750573324115"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p1350563310410"><a name="p1350563310410"></a><a name="p1350563310410"></a>evs:volumes:uploadImage</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul2038991513269"></a><a name="ul2038991513269"></a><ul id="ul2038991513269"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_22"><a name="zh-cn_topic_0103526772_p48451412122317_22"></a><a name="zh-cn_topic_0103526772_p48451412122317_22"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_22"><a name="zh-cn_topic_0103526772_p69718230159_22"></a><a name="zh-cn_topic_0103526772_p69718230159_22"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row919611258261"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p15051833184116"><a name="p15051833184116"></a><a name="p15051833184116"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p1850543384110"><a name="p1850543384110"></a><a name="p1850543384110"></a>action="os-attach"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p1350513334410"><a name="p1350513334410"></a><a name="p1350513334410"></a>挂载云硬盘（废弃）</p>
<p id="p17505183344119"><a name="p17505183344119"></a><a name="p17505183344119"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p3505633174113"><a name="p3505633174113"></a><a name="p3505633174113"></a>evs:volumes:attach</p>
<p id="p7683122512614"><a name="p7683122512614"></a><a name="p7683122512614"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul93581424132615"></a><a name="ul93581424132615"></a><ul id="ul93581424132615"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_23"><a name="zh-cn_topic_0103526772_p48451412122317_23"></a><a name="zh-cn_topic_0103526772_p48451412122317_23"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_23"><a name="zh-cn_topic_0103526772_p69718230159_23"></a><a name="zh-cn_topic_0103526772_p69718230159_23"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row520272562611"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p1150519336416"><a name="p1150519336416"></a><a name="p1150519336416"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p1950511331414"><a name="p1950511331414"></a><a name="p1950511331414"></a>action="os-detach"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p9505233144119"><a name="p9505233144119"></a><a name="p9505233144119"></a>卸载云硬盘（废弃）</p>
<p id="p12505833184111"><a name="p12505833184111"></a><a name="p12505833184111"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p75050336410"><a name="p75050336410"></a><a name="p75050336410"></a>evs:volumes:detach</p>
<p id="p924813014617"><a name="p924813014617"></a><a name="p924813014617"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul13297192816267"></a><a name="ul13297192816267"></a><ul id="ul13297192816267"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_24"><a name="zh-cn_topic_0103526772_p48451412122317_24"></a><a name="zh-cn_topic_0103526772_p48451412122317_24"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_24"><a name="zh-cn_topic_0103526772_p69718230159_24"></a><a name="zh-cn_topic_0103526772_p69718230159_24"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row72061525202618"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p105050339412"><a name="p105050339412"></a><a name="p105050339412"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p18507533144114"><a name="p18507533144114"></a><a name="p18507533144114"></a>action="os-reserve"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p1550793324114"><a name="p1550793324114"></a><a name="p1550793324114"></a>保留云硬盘（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p150711337412"><a name="p150711337412"></a><a name="p150711337412"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul15999123612263"></a><a name="ul15999123612263"></a><ul id="ul15999123612263"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_25"><a name="zh-cn_topic_0103526772_p48451412122317_25"></a><a name="zh-cn_topic_0103526772_p48451412122317_25"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_25"><a name="zh-cn_topic_0103526772_p69718230159_25"></a><a name="zh-cn_topic_0103526772_p69718230159_25"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row202111725132618"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p8507193344116"><a name="p8507193344116"></a><a name="p8507193344116"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p10507183319418"><a name="p10507183319418"></a><a name="p10507183319418"></a>action="os-unreserve"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p17507153311414"><a name="p17507153311414"></a><a name="p17507153311414"></a>取消保留云硬盘（OpenStack Cinder）</p>
<p id="p1450715338413"><a name="p1450715338413"></a><a name="p1450715338413"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p1250710336417"><a name="p1250710336417"></a><a name="p1250710336417"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul15613852172611"></a><a name="ul15613852172611"></a><ul id="ul15613852172611"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_26"><a name="zh-cn_topic_0103526772_p48451412122317_26"></a><a name="zh-cn_topic_0103526772_p48451412122317_26"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_26"><a name="zh-cn_topic_0103526772_p69718230159_26"></a><a name="zh-cn_topic_0103526772_p69718230159_26"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row3216132515266"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p1450773317410"><a name="p1450773317410"></a><a name="p1450773317410"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p250717334411"><a name="p250717334411"></a><a name="p250717334411"></a>action="os-set_bootable"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p650763354113"><a name="p650763354113"></a><a name="p650763354113"></a>设置云硬盘启动盘标识（OpenStack Cinder）</p>
<p id="p1350713313411"><a name="p1350713313411"></a><a name="p1350713313411"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p2050703394118"><a name="p2050703394118"></a><a name="p2050703394118"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul88341954192618"></a><a name="ul88341954192618"></a><ul id="ul88341954192618"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_27"><a name="zh-cn_topic_0103526772_p48451412122317_27"></a><a name="zh-cn_topic_0103526772_p48451412122317_27"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_27"><a name="zh-cn_topic_0103526772_p69718230159_27"></a><a name="zh-cn_topic_0103526772_p69718230159_27"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row122182572614"><td class="cellrowborder" valign="top" width="29.292929292929294%" headers="mcps1.1.5.1.1 "><p id="p17507173311412"><a name="p17507173311412"></a><a name="p17507173311412"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p2507123311416"><a name="p2507123311416"></a><a name="p2507123311416"></a>action="os-update_readonly_flag"</p>
</td>
<td class="cellrowborder" valign="top" width="23.232323232323235%" headers="mcps1.1.5.1.2 "><p id="p1750819334410"><a name="p1750819334410"></a><a name="p1750819334410"></a>设置云硬盘只读标识（OpenStack Cinder）</p>
<p id="p250873310414"><a name="p250873310414"></a><a name="p250873310414"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.21212121212121%" headers="mcps1.1.5.1.3 "><p id="p14508153317415"><a name="p14508153317415"></a><a name="p14508153317415"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="26.262626262626267%" headers="mcps1.1.5.1.4 "><a name="ul735765982614"></a><a name="ul735765982614"></a><ul id="ul735765982614"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_28"><a name="zh-cn_topic_0103526772_p48451412122317_28"></a><a name="zh-cn_topic_0103526772_p48451412122317_28"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_28"><a name="zh-cn_topic_0103526772_p69718230159_28"></a><a name="zh-cn_topic_0103526772_p69718230159_28"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 云硬盘快照<a name="section176411659163519"></a>

<a name="table8361746185711"></a>
<table><thead align="left"><tr id="row4369184618577"><th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.1.5.1.1"><p id="p837214615572"><a name="p837214615572"></a><a name="p837214615572"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.1.5.1.2"><p id="p14374246205714"><a name="p14374246205714"></a><a name="p14374246205714"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.3"><p id="p15377546195711"><a name="p15377546195711"></a><a name="p15377546195711"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p2030075519274"><a name="p2030075519274"></a><a name="p2030075519274"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row643864695720"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p173020522617"><a name="p173020522617"></a><a name="p173020522617"></a>POST /v2/{project_id}/snapshots</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p10520201618586"><a name="p10520201618586"></a><a name="p10520201618586"></a>创建云硬盘快照（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p7520191613584"><a name="p7520191613584"></a><a name="p7520191613584"></a>evs:snapshots:create</p>
<p id="p752061675812"><a name="p752061675812"></a><a name="p752061675812"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul11373143012820"></a><a name="ul11373143012820"></a><ul id="ul11373143012820"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_29"><a name="zh-cn_topic_0103526772_p48451412122317_29"></a><a name="zh-cn_topic_0103526772_p48451412122317_29"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_29"><a name="zh-cn_topic_0103526772_p69718230159_29"></a><a name="zh-cn_topic_0103526772_p69718230159_29"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1075585012810"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p13741125732820"><a name="p13741125732820"></a><a name="p13741125732820"></a>POST /v2/{project_id}/cloudsnapshots</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p174195720280"><a name="p174195720280"></a><a name="p174195720280"></a>创建云硬盘快照</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p9741105720285"><a name="p9741105720285"></a><a name="p9741105720285"></a>evs:snapshots:create</p>
<p id="p774185710282"><a name="p774185710282"></a><a name="p774185710282"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul1796315454296"></a><a name="ul1796315454296"></a><ul id="ul1796315454296"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_5"></a><a name="zh-cn_topic_0103526772_ul188661423121511_5"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_5"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row134461346195715"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p837771515718"><a name="p837771515718"></a><a name="p837771515718"></a>GET /v2/{project_id}/snapshots</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p186113213712"><a name="p186113213712"></a><a name="p186113213712"></a>查询云硬盘快照列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p2520191615588"><a name="p2520191615588"></a><a name="p2520191615588"></a>evs:snapshots:list</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul94231453142915"></a><a name="ul94231453142915"></a><ul id="ul94231453142915"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_30"><a name="zh-cn_topic_0103526772_p48451412122317_30"></a><a name="zh-cn_topic_0103526772_p48451412122317_30"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_30"><a name="zh-cn_topic_0103526772_p69718230159_30"></a><a name="zh-cn_topic_0103526772_p69718230159_30"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row54658465572"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p868974613712"><a name="p868974613712"></a><a name="p868974613712"></a>GET /v2/{project_id}/snapshots/detail</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p157141752374"><a name="p157141752374"></a><a name="p157141752374"></a>查询云硬盘快照详细信息列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p19520181617589"><a name="p19520181617589"></a><a name="p19520181617589"></a>evs:snapshots:list</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul15728135492913"></a><a name="ul15728135492913"></a><ul id="ul15728135492913"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_31"><a name="zh-cn_topic_0103526772_p48451412122317_31"></a><a name="zh-cn_topic_0103526772_p48451412122317_31"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_31"><a name="zh-cn_topic_0103526772_p69718230159_31"></a><a name="zh-cn_topic_0103526772_p69718230159_31"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1756178123012"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p9500131483014"><a name="p9500131483014"></a><a name="p9500131483014"></a>GET /v2/{project_id}/cloudsnapshots/detail</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p85004141305"><a name="p85004141305"></a><a name="p85004141305"></a>查询云硬盘快照列表详情</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p7500614183020"><a name="p7500614183020"></a><a name="p7500614183020"></a>evs:snapshots:list</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul12768627113016"></a><a name="ul12768627113016"></a><ul id="ul12768627113016"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_6"></a><a name="zh-cn_topic_0103526772_ul188661423121511_6"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_6"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row10475194695719"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p6634104593"><a name="p6634104593"></a><a name="p6634104593"></a>PUT /v2/{project_id}/snapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p8520916115814"><a name="p8520916115814"></a><a name="p8520916115814"></a>更新云硬盘快照（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p1252071613582"><a name="p1252071613582"></a><a name="p1252071613582"></a>evs:snapshots:update</p>
<p id="p205082024154519"><a name="p205082024154519"></a><a name="p205082024154519"></a>evs:snapshots:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul139333517301"></a><a name="ul139333517301"></a><ul id="ul139333517301"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_32"><a name="zh-cn_topic_0103526772_p48451412122317_32"></a><a name="zh-cn_topic_0103526772_p48451412122317_32"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_32"><a name="zh-cn_topic_0103526772_p69718230159_32"></a><a name="zh-cn_topic_0103526772_p69718230159_32"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row179161013314"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p598817197319"><a name="p598817197319"></a><a name="p598817197319"></a>PUT /v2/{project_id}/cloudsnapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p8988101983119"><a name="p8988101983119"></a><a name="p8988101983119"></a>更新云硬盘快照</p>
<p id="p1698811190312"><a name="p1698811190312"></a><a name="p1698811190312"></a></p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p99887198315"><a name="p99887198315"></a><a name="p99887198315"></a>evs:snapshots:update</p>
<p id="p898814195311"><a name="p898814195311"></a><a name="p898814195311"></a>evs:snapshots:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul0448142513117"></a><a name="ul0448142513117"></a><ul id="ul0448142513117"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_7"></a><a name="zh-cn_topic_0103526772_ul188661423121511_7"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_7"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1217231317314"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p61881743123115"><a name="p61881743123115"></a><a name="p61881743123115"></a>GET</p>
<p id="p201888434316"><a name="p201888434316"></a><a name="p201888434316"></a>/v2/{project_id}/snapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p91887436313"><a name="p91887436313"></a><a name="p91887436313"></a>查询云硬盘快照详情（OpenStack Cinder）</p>
<p id="p41881643193114"><a name="p41881643193114"></a><a name="p41881643193114"></a></p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p15188194319319"><a name="p15188194319319"></a><a name="p15188194319319"></a>evs:snapshots:get</p>
<p id="p151886434311"><a name="p151886434311"></a><a name="p151886434311"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul4298165463114"></a><a name="ul4298165463114"></a><ul id="ul4298165463114"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_33"><a name="zh-cn_topic_0103526772_p48451412122317_33"></a><a name="zh-cn_topic_0103526772_p48451412122317_33"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_33"><a name="zh-cn_topic_0103526772_p69718230159_33"></a><a name="zh-cn_topic_0103526772_p69718230159_33"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row1412410163210"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p9721822133211"><a name="p9721822133211"></a><a name="p9721822133211"></a>GET</p>
<p id="p10721192293212"><a name="p10721192293212"></a><a name="p10721192293212"></a>/v2/{project_id}/cloudsnapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p87211922103217"><a name="p87211922103217"></a><a name="p87211922103217"></a>查询云硬盘快照详情</p>
<p id="p107216223328"><a name="p107216223328"></a><a name="p107216223328"></a></p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p147211522103211"><a name="p147211522103211"></a><a name="p147211522103211"></a>evs:snapshots:get</p>
<p id="p10721722143211"><a name="p10721722143211"></a><a name="p10721722143211"></a></p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul114583449323"></a><a name="ul114583449323"></a><ul id="ul114583449323"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_8"></a><a name="zh-cn_topic_0103526772_ul188661423121511_8"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_8"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
<tr id="row1448414645716"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p732852311913"><a name="p732852311913"></a><a name="p732852311913"></a>DELETE /v2/{project_id}/snapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p568112919919"><a name="p568112919919"></a><a name="p568112919919"></a>删除云硬盘快照（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p15520161665817"><a name="p15520161665817"></a><a name="p15520161665817"></a>evs:snapshots:delete</p>
<p id="p331517388456"><a name="p331517388456"></a><a name="p331517388456"></a>evs:snapshots:get</p>
<p id="p47022010154218"><a name="p47022010154218"></a><a name="p47022010154218"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul3874175513213"></a><a name="ul3874175513213"></a><ul id="ul3874175513213"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_34"><a name="zh-cn_topic_0103526772_p48451412122317_34"></a><a name="zh-cn_topic_0103526772_p48451412122317_34"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_34"><a name="zh-cn_topic_0103526772_p69718230159_34"></a><a name="zh-cn_topic_0103526772_p69718230159_34"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row413170183313"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.1.5.1.1 "><p id="p5277127133311"><a name="p5277127133311"></a><a name="p5277127133311"></a>DELETE /v2/{project_id}/cloudsnapshots/{snapshot_id}</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.1.5.1.2 "><p id="p6277117193320"><a name="p6277117193320"></a><a name="p6277117193320"></a>删除云硬盘快照</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.3 "><p id="p32777710334"><a name="p32777710334"></a><a name="p32777710334"></a>evs:snapshots:delete</p>
<p id="p15277779333"><a name="p15277779333"></a><a name="p15277779333"></a>evs:snapshots:get</p>
<p id="p153941629164318"><a name="p153941629164318"></a><a name="p153941629164318"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul251571614333"></a><a name="ul251571614333"></a><ul id="ul251571614333"><li>支持：<a name="zh-cn_topic_0103526772_ul188661423121511_9"></a><a name="zh-cn_topic_0103526772_ul188661423121511_9"></a><ul id="zh-cn_topic_0103526772_ul188661423121511_9"><li>项目(Project)</li><li>企业项目(Enterprise Project)</li></ul>
</li></ul>
</td>
</tr>
</tbody>
</table>

## 云硬盘过户<a name="section173078159254"></a>

<a name="table33101915182515"></a>
<table><thead align="left"><tr id="row832041542517"><th class="cellrowborder" valign="top" width="28.000000000000004%" id="mcps1.1.5.1.1"><p id="p432481512259"><a name="p432481512259"></a><a name="p432481512259"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="22%" id="mcps1.1.5.1.2"><p id="p732841511255"><a name="p732841511255"></a><a name="p732841511255"></a>API功能</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p11330151542511"><a name="p11330151542511"></a><a name="p11330151542511"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p3822238173919"><a name="p3822238173919"></a><a name="p3822238173919"></a>授权项作用域</p>
</th>
</tr>
</thead>
<tbody><tr id="row1533321516254"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p1853611211283"><a name="p1853611211283"></a><a name="p1853611211283"></a>POST /v2/{project_id}/os-volume-transfer</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p178090277285"><a name="p178090277285"></a><a name="p178090277285"></a>创建云硬盘过户</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p1355812615270"><a name="p1355812615270"></a><a name="p1355812615270"></a>evs:transfers:create</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul498414413399"></a><a name="ul498414413399"></a><ul id="ul498414413399"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_35"><a name="zh-cn_topic_0103526772_p48451412122317_35"></a><a name="zh-cn_topic_0103526772_p48451412122317_35"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_35"><a name="zh-cn_topic_0103526772_p69718230159_35"></a><a name="zh-cn_topic_0103526772_p69718230159_35"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row63451215152514"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p198813107290"><a name="p198813107290"></a><a name="p198813107290"></a>GET /v2/{project_id}/os-volume-transfer</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p3558142672711"><a name="p3558142672711"></a><a name="p3558142672711"></a>查询云硬盘过户记录列表概要</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p265073320219"><a name="p265073320219"></a><a name="p265073320219"></a>evs:transfers:list</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul819753819404"></a><a name="ul819753819404"></a><ul id="ul819753819404"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_36"><a name="zh-cn_topic_0103526772_p48451412122317_36"></a><a name="zh-cn_topic_0103526772_p48451412122317_36"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_36"><a name="zh-cn_topic_0103526772_p69718230159_36"></a><a name="zh-cn_topic_0103526772_p69718230159_36"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row8355101572511"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p0311347122919"><a name="p0311347122919"></a><a name="p0311347122919"></a>GET /v2/{project_id}/os-volume-transfer/detail</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p165581269277"><a name="p165581269277"></a><a name="p165581269277"></a>查询云硬盘过户记录列表详情</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p6652143318216"><a name="p6652143318216"></a><a name="p6652143318216"></a>evs:transfers:list</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul10388539104010"></a><a name="ul10388539104010"></a><ul id="ul10388539104010"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_37"><a name="zh-cn_topic_0103526772_p48451412122317_37"></a><a name="zh-cn_topic_0103526772_p48451412122317_37"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_37"><a name="zh-cn_topic_0103526772_p69718230159_37"></a><a name="zh-cn_topic_0103526772_p69718230159_37"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row5365101582519"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p135558423014"><a name="p135558423014"></a><a name="p135558423014"></a>GET /v2/{project_id}/os-volume-transfer/{transfer_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p65587264271"><a name="p65587264271"></a><a name="p65587264271"></a>查询单个云硬盘过户记录详情</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p1055817260275"><a name="p1055817260275"></a><a name="p1055817260275"></a>evs:transfers:get</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul169486499402"></a><a name="ul169486499402"></a><ul id="ul169486499402"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_38"><a name="zh-cn_topic_0103526772_p48451412122317_38"></a><a name="zh-cn_topic_0103526772_p48451412122317_38"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_38"><a name="zh-cn_topic_0103526772_p69718230159_38"></a><a name="zh-cn_topic_0103526772_p69718230159_38"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row113831315142516"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p1440162033011"><a name="p1440162033011"></a><a name="p1440162033011"></a>POST /v2/{project_id}/os-volume-transfer/{transfer_id}/accept</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p855819261278"><a name="p855819261278"></a><a name="p855819261278"></a>接受云硬盘过户</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p95583265274"><a name="p95583265274"></a><a name="p95583265274"></a>evs:transfers:accept</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul49972050154015"></a><a name="ul49972050154015"></a><ul id="ul49972050154015"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_39"><a name="zh-cn_topic_0103526772_p48451412122317_39"></a><a name="zh-cn_topic_0103526772_p48451412122317_39"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_39"><a name="zh-cn_topic_0103526772_p69718230159_39"></a><a name="zh-cn_topic_0103526772_p69718230159_39"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
<tr id="row997615405218"><td class="cellrowborder" valign="top" width="28.000000000000004%" headers="mcps1.1.5.1.1 "><p id="p2459121182211"><a name="p2459121182211"></a><a name="p2459121182211"></a>DELETE /v2/{project_id}/os-volume-transfer/{transfer_id}</p>
</td>
<td class="cellrowborder" valign="top" width="22%" headers="mcps1.1.5.1.2 "><p id="p1394094642118"><a name="p1394094642118"></a><a name="p1394094642118"></a>删除云硬盘过户</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p179401346122117"><a name="p179401346122117"></a><a name="p179401346122117"></a>evs:transfers:delete</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><a name="ul11216152124012"></a><a name="ul11216152124012"></a><ul id="ul11216152124012"><li>支持：<p id="zh-cn_topic_0103526772_p48451412122317_40"><a name="zh-cn_topic_0103526772_p48451412122317_40"></a><a name="zh-cn_topic_0103526772_p48451412122317_40"></a>项目(Project)</p>
</li><li>不支持：<p id="zh-cn_topic_0103526772_p69718230159_40"><a name="zh-cn_topic_0103526772_p69718230159_40"></a><a name="zh-cn_topic_0103526772_p69718230159_40"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
</tr>
</tbody>
</table>

