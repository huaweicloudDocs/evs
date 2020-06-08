# 云硬盘Actions<a name="evs_04_0026"></a>

本章节仅列出了云硬盘v2接口的授权信息。对于v3接口，若提供的功能与v2接口一样，则授权信息也一致。

例如：创建云硬盘时，v2接口为POST /v2/\{project\_id\}/cloudvolumes，对应的v3接口为POST /v3/\{project\_id\}/cloudvolumes，两个接口支持的授权信息一致。

<a name="table11136162518266"></a>
<table><thead align="left"><tr id="evs_04_0045_row19140152562617"><th class="cellrowborder" valign="top" width="26.05%" id="mcps1.1.5.1.1"><p id="evs_04_0045_p5664144515597"><a name="evs_04_0045_p5664144515597"></a><a name="evs_04_0045_p5664144515597"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="21.73%" id="mcps1.1.5.1.2"><p id="evs_04_0045_p9664104575914"><a name="evs_04_0045_p9664104575914"></a><a name="evs_04_0045_p9664104575914"></a>授权项</p>
</th>
<th class="cellrowborder" valign="top" width="22.259999999999998%" id="mcps1.1.5.1.3"><p id="evs_04_0045_p266414512595"><a name="evs_04_0045_p266414512595"></a><a name="evs_04_0045_p266414512595"></a>授权范围</p>
</th>
<th class="cellrowborder" valign="top" width="29.959999999999997%" id="mcps1.1.5.1.4"><p id="evs_04_0045_p19664194585915"><a name="evs_04_0045_p19664194585915"></a><a name="evs_04_0045_p19664194585915"></a>对应API接口</p>
</th>
</tr>
</thead>
<tbody><tr id="evs_04_0045_row14183202592618"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p1630995419425"><a name="evs_04_0045_p1630995419425"></a><a name="evs_04_0045_p1630995419425"></a>扩容云硬盘（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p1350513314414"><a name="evs_04_0045_p1350513314414"></a><a name="evs_04_0045_p1350513314414"></a>evs:volumes:extend</p>
<p id="evs_04_0045_p1938111964"><a name="evs_04_0045_p1938111964"></a><a name="evs_04_0045_p1938111964"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul13951688261"></a><a name="evs_04_0045_ul13951688261"></a><ul id="evs_04_0045_ul13951688261"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317"><a name="evs_04_0045_evs_04_0045_p48451412122317"></a><a name="evs_04_0045_evs_04_0045_p48451412122317"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159"><a name="evs_04_0045_evs_04_0045_p69718230159"></a><a name="evs_04_0045_evs_04_0045_p69718230159"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p12701151145818"><a name="evs_04_0045_p12701151145818"></a><a name="evs_04_0045_p12701151145818"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p870141175817"><a name="evs_04_0045_p870141175817"></a><a name="evs_04_0045_p870141175817"></a>action="os-extend"</p>
</td>
</tr>
<tr id="evs_04_0045_row7188202572612"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p14505173334110"><a name="evs_04_0045_p14505173334110"></a><a name="evs_04_0045_p14505173334110"></a>将云硬盘导出为镜像（OpenStack Cinder）</p>
<p id="evs_04_0045_p750573324115"><a name="evs_04_0045_p750573324115"></a><a name="evs_04_0045_p750573324115"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p1350563310410"><a name="evs_04_0045_p1350563310410"></a><a name="evs_04_0045_p1350563310410"></a>evs:volumes:uploadImage</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul2038991513269"></a><a name="evs_04_0045_ul2038991513269"></a><ul id="evs_04_0045_ul2038991513269"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_1"><a name="evs_04_0045_evs_04_0045_p48451412122317_1"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_1"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_1"><a name="evs_04_0045_evs_04_0045_p69718230159_1"></a><a name="evs_04_0045_evs_04_0045_p69718230159_1"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p1870171125811"><a name="evs_04_0045_p1870171125811"></a><a name="evs_04_0045_p1870171125811"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p770151125815"><a name="evs_04_0045_p770151125815"></a><a name="evs_04_0045_p770151125815"></a>action="os-volume_upload_image"</p>
</td>
</tr>
<tr id="evs_04_0045_row919611258261"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p1350513334410"><a name="evs_04_0045_p1350513334410"></a><a name="evs_04_0045_p1350513334410"></a>挂载云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p17505183344119"><a name="evs_04_0045_p17505183344119"></a><a name="evs_04_0045_p17505183344119"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p3505633174113"><a name="evs_04_0045_p3505633174113"></a><a name="evs_04_0045_p3505633174113"></a>evs:volumes:attach</p>
<p id="evs_04_0045_p7683122512614"><a name="evs_04_0045_p7683122512614"></a><a name="evs_04_0045_p7683122512614"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul93581424132615"></a><a name="evs_04_0045_ul93581424132615"></a><ul id="evs_04_0045_ul93581424132615"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_2"><a name="evs_04_0045_evs_04_0045_p48451412122317_2"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_2"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_2"><a name="evs_04_0045_evs_04_0045_p69718230159_2"></a><a name="evs_04_0045_evs_04_0045_p69718230159_2"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p1771715164586"><a name="evs_04_0045_p1771715164586"></a><a name="evs_04_0045_p1771715164586"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p4717516115811"><a name="evs_04_0045_p4717516115811"></a><a name="evs_04_0045_p4717516115811"></a>action="os-attach"</p>
</td>
</tr>
<tr id="evs_04_0045_row520272562611"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p9505233144119"><a name="evs_04_0045_p9505233144119"></a><a name="evs_04_0045_p9505233144119"></a>卸载云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p12505833184111"><a name="evs_04_0045_p12505833184111"></a><a name="evs_04_0045_p12505833184111"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p75050336410"><a name="evs_04_0045_p75050336410"></a><a name="evs_04_0045_p75050336410"></a>evs:volumes:detach</p>
<p id="evs_04_0045_p924813014617"><a name="evs_04_0045_p924813014617"></a><a name="evs_04_0045_p924813014617"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul13297192816267"></a><a name="evs_04_0045_ul13297192816267"></a><ul id="evs_04_0045_ul13297192816267"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_3"><a name="evs_04_0045_evs_04_0045_p48451412122317_3"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_3"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_3"><a name="evs_04_0045_evs_04_0045_p69718230159_3"></a><a name="evs_04_0045_evs_04_0045_p69718230159_3"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p171791612583"><a name="evs_04_0045_p171791612583"></a><a name="evs_04_0045_p171791612583"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p19717171616581"><a name="evs_04_0045_p19717171616581"></a><a name="evs_04_0045_p19717171616581"></a>action="os-detach"</p>
</td>
</tr>
<tr id="evs_04_0045_row72061525202618"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p1550793324114"><a name="evs_04_0045_p1550793324114"></a><a name="evs_04_0045_p1550793324114"></a>保留云硬盘（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p150711337412"><a name="evs_04_0045_p150711337412"></a><a name="evs_04_0045_p150711337412"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul15999123612263"></a><a name="evs_04_0045_ul15999123612263"></a><ul id="evs_04_0045_ul15999123612263"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_4"><a name="evs_04_0045_evs_04_0045_p48451412122317_4"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_4"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_4"><a name="evs_04_0045_evs_04_0045_p69718230159_4"></a><a name="evs_04_0045_evs_04_0045_p69718230159_4"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p9556221585"><a name="evs_04_0045_p9556221585"></a><a name="evs_04_0045_p9556221585"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p20551522115817"><a name="evs_04_0045_p20551522115817"></a><a name="evs_04_0045_p20551522115817"></a>action="os-reserve"</p>
</td>
</tr>
<tr id="evs_04_0045_row202111725132618"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p17507153311414"><a name="evs_04_0045_p17507153311414"></a><a name="evs_04_0045_p17507153311414"></a>取消保留云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p1450715338413"><a name="evs_04_0045_p1450715338413"></a><a name="evs_04_0045_p1450715338413"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p1250710336417"><a name="evs_04_0045_p1250710336417"></a><a name="evs_04_0045_p1250710336417"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul15613852172611"></a><a name="evs_04_0045_ul15613852172611"></a><ul id="evs_04_0045_ul15613852172611"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_5"><a name="evs_04_0045_evs_04_0045_p48451412122317_5"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_5"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_5"><a name="evs_04_0045_evs_04_0045_p69718230159_5"></a><a name="evs_04_0045_evs_04_0045_p69718230159_5"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p4551922135816"><a name="evs_04_0045_p4551922135816"></a><a name="evs_04_0045_p4551922135816"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p105512210589"><a name="evs_04_0045_p105512210589"></a><a name="evs_04_0045_p105512210589"></a>action="os-unreserve"</p>
</td>
</tr>
<tr id="evs_04_0045_row3216132515266"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p650763354113"><a name="evs_04_0045_p650763354113"></a><a name="evs_04_0045_p650763354113"></a>设置云硬盘启动盘标识（OpenStack Cinder）</p>
<p id="evs_04_0045_p1350713313411"><a name="evs_04_0045_p1350713313411"></a><a name="evs_04_0045_p1350713313411"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p2050703394118"><a name="evs_04_0045_p2050703394118"></a><a name="evs_04_0045_p2050703394118"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul88341954192618"></a><a name="evs_04_0045_ul88341954192618"></a><ul id="evs_04_0045_ul88341954192618"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_6"><a name="evs_04_0045_evs_04_0045_p48451412122317_6"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_6"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_6"><a name="evs_04_0045_evs_04_0045_p69718230159_6"></a><a name="evs_04_0045_evs_04_0045_p69718230159_6"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p555822145818"><a name="evs_04_0045_p555822145818"></a><a name="evs_04_0045_p555822145818"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p1956132219580"><a name="evs_04_0045_p1956132219580"></a><a name="evs_04_0045_p1956132219580"></a>action="os-set_bootable"</p>
</td>
</tr>
<tr id="evs_04_0045_row122182572614"><td class="cellrowborder" valign="top" width="26.05%" headers="mcps1.1.5.1.1 "><p id="evs_04_0045_p1750819334410"><a name="evs_04_0045_p1750819334410"></a><a name="evs_04_0045_p1750819334410"></a>设置云硬盘只读标识（OpenStack Cinder）</p>
<p id="evs_04_0045_p250873310414"><a name="evs_04_0045_p250873310414"></a><a name="evs_04_0045_p250873310414"></a></p>
</td>
<td class="cellrowborder" valign="top" width="21.73%" headers="mcps1.1.5.1.2 "><p id="evs_04_0045_p14508153317415"><a name="evs_04_0045_p14508153317415"></a><a name="evs_04_0045_p14508153317415"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="22.259999999999998%" headers="mcps1.1.5.1.3 "><a name="evs_04_0045_ul735765982614"></a><a name="evs_04_0045_ul735765982614"></a><ul id="evs_04_0045_ul735765982614"><li>支持：<p id="evs_04_0045_evs_04_0045_p48451412122317_7"><a name="evs_04_0045_evs_04_0045_p48451412122317_7"></a><a name="evs_04_0045_evs_04_0045_p48451412122317_7"></a>IAM项目(Project)</p>
</li><li>不支持：<p id="evs_04_0045_evs_04_0045_p69718230159_7"><a name="evs_04_0045_evs_04_0045_p69718230159_7"></a><a name="evs_04_0045_evs_04_0045_p69718230159_7"></a>企业项目(Enterprise Project)</p>
</li></ul>
</td>
<td class="cellrowborder" valign="top" width="29.959999999999997%" headers="mcps1.1.5.1.4 "><p id="evs_04_0045_p556162215810"><a name="evs_04_0045_p556162215810"></a><a name="evs_04_0045_p556162215810"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p4561722185810"><a name="evs_04_0045_p4561722185810"></a><a name="evs_04_0045_p4561722185810"></a>action="os-update_readonly_flag"</p>
</td>
</tr>
</tbody>
</table>

