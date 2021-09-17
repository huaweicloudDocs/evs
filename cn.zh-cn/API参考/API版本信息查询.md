# API版本信息查询<a name="evs_04_0024"></a>

本章节仅列出了云硬盘v2接口的授权信息。对于v3接口，若提供的功能与v2接口一样，则授权信息也一致。

例如：创建云硬盘时，v2接口为POST /v2/\{project\_id\}/cloudvolumes，对应的v3接口为POST /v3/\{project\_id\}/cloudvolumes，两个接口支持的授权信息一致。

授权项列表中，“√”表示支持，“×”表示暂不支持。

<a name="table1331719418287"></a>
<table><thead align="left"><tr id="evs_04_0045_row103171646287"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.1"><p id="evs_04_0045_p153189416282"><a name="evs_04_0045_p153189416282"></a><a name="evs_04_0045_p153189416282"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.2"><p id="evs_04_0045_p10121923790"><a name="evs_04_0045_p10121923790"></a><a name="evs_04_0045_p10121923790"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.3"><p id="evs_04_0045_p931834172816"><a name="evs_04_0045_p931834172816"></a><a name="evs_04_0045_p931834172816"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.4"><p id="evs_04_0045_p10825627161212"><a name="evs_04_0045_p10825627161212"></a><a name="evs_04_0045_p10825627161212"></a>IAM项目</p>
<p id="evs_04_0045_p731814452814"><a name="evs_04_0045_p731814452814"></a><a name="evs_04_0045_p731814452814"></a>(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.5"><p id="evs_04_0045_p121341846171217"><a name="evs_04_0045_p121341846171217"></a><a name="evs_04_0045_p121341846171217"></a>企业项目</p>
<p id="evs_04_0045_p713974411215"><a name="evs_04_0045_p713974411215"></a><a name="evs_04_0045_p713974411215"></a>(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="evs_04_0045_row133414414280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p1934254112819"><a name="evs_04_0045_p1934254112819"></a><a name="evs_04_0045_p1934254112819"></a>查询接口版本信息列表（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p012115231598"><a name="evs_04_0045_p012115231598"></a><a name="evs_04_0045_p012115231598"></a>GET /</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p1634274142812"><a name="evs_04_0045_p1634274142812"></a><a name="evs_04_0045_p1634274142812"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p98032297487"><a name="evs_04_0045_p98032297487"></a><a name="evs_04_0045_p98032297487"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p13804112910485"><a name="evs_04_0045_p13804112910485"></a><a name="evs_04_0045_p13804112910485"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row734315442811"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p234314411288"><a name="evs_04_0045_p234314411288"></a><a name="evs_04_0045_p234314411288"></a>查询接口的版本信息（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p10121123398"><a name="evs_04_0045_p10121123398"></a><a name="evs_04_0045_p10121123398"></a>GET /{api_version}</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p134311482810"><a name="evs_04_0045_p134311482810"></a><a name="evs_04_0045_p134311482810"></a>无</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p134712580137"><a name="evs_04_0045_p134712580137"></a><a name="evs_04_0045_p134712580137"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p14727201551412"><a name="evs_04_0045_p14727201551412"></a><a name="evs_04_0045_p14727201551412"></a>×</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>授权项（Action）为无，表示无需授权。

