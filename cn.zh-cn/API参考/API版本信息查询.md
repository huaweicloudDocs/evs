# API版本信息查询<a name="evs_04_0024"></a>

本章节仅列出了云硬盘v2接口的授权信息。对于v3接口，若提供的功能与v2接口一样，则授权信息也一致。

例如：创建云硬盘时，v2接口为POST /v2/\{project\_id\}/cloudvolumes，对应的v3接口为POST /v3/\{project\_id\}/cloudvolumes，两个接口支持的授权信息一致。

<a name="table1331719418287"></a>
<table><thead align="left"><tr id="evs_04_0045_row103171646287"><th class="cellrowborder" valign="top" width="25.532553255325535%" id="mcps1.1.5.1.1"><p id="evs_04_0045_p153189416282"><a name="evs_04_0045_p153189416282"></a><a name="evs_04_0045_p153189416282"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="21.31213121312131%" id="mcps1.1.5.1.2"><p id="evs_04_0045_p931834172816"><a name="evs_04_0045_p931834172816"></a><a name="evs_04_0045_p931834172816"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="22.572257225722574%" id="mcps1.1.5.1.3"><p id="evs_04_0045_p731814452814"><a name="evs_04_0045_p731814452814"></a><a name="evs_04_0045_p731814452814"></a>授权范围</p>
</th>
<th class="cellrowborder" valign="top" width="30.583058305830583%" id="mcps1.1.5.1.4"><p id="evs_04_0045_p1317114142817"><a name="evs_04_0045_p1317114142817"></a><a name="evs_04_0045_p1317114142817"></a>对应API接口</p>
</th>
</tr>
</thead>
<tbody><tr id="evs_04_0045_row133414414280"><td class="cellrowborder" valign="top" width="25.532553255325535%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p1934254112819"><a name="evs_04_0045_p1934254112819"></a><a name="evs_04_0045_p1934254112819"></a>查询接口版本信息列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p1634274142812"><a name="evs_04_0045_p1634274142812"></a><a name="evs_04_0045_p1634274142812"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="22.572257225722574%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul15342449284"></a><a name="evs_04_0045_ul15342449284"></a><ul id="evs_04_0045_ul15342449284"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317"><a name="evs_04_0045_evs_04_0045_p48451412122317"></a><a name="evs_04_0045_evs_04_0045_p48451412122317"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159"><a name="evs_04_0045_evs_04_0045_p69718230159"></a><a name="evs_04_0045_evs_04_0045_p69718230159"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p43411146283"><a name="evs_04_0045_p43411146283"></a><a name="evs_04_0045_p43411146283"></a>GET /</p>
</td>
</tr>
<tr id="evs_04_0045_row734315442811"><td class="cellrowborder" valign="top" width="25.532553255325535%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p234314411288"><a name="evs_04_0045_p234314411288"></a><a name="evs_04_0045_p234314411288"></a>查询接口的版本信息（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="21.31213121312131%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p134311482810"><a name="evs_04_0045_p134311482810"></a><a name="evs_04_0045_p134311482810"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="22.572257225722574%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul83430413283"></a><a name="evs_04_0045_ul83430413283"></a><ul id="evs_04_0045_ul83430413283"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_1"><a name="evs_04_0045_evs_04_0045_p48451412122317_1"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_1"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_1"><a name="evs_04_0045_evs_04_0045_p69718230159_1"></a><a name="evs_04_0045_evs_04_0045_p69718230159_1"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="30.583058305830583%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p193431342281"><a name="evs_04_0045_p193431342281"></a><a name="evs_04_0045_p193431342281"></a>GET /{api_version}</p>
</td>
</tr>
</tbody>
</table>

