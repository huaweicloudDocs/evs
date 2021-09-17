# 云硬盘Actions<a name="evs_04_0026"></a>

本章节仅列出了云硬盘v2接口的授权信息。对于v3接口，若提供的功能与v2接口一样，则授权信息也一致。

例如：创建云硬盘时，v2接口为POST /v2/\{project\_id\}/cloudvolumes，对应的v3接口为POST /v3/\{project\_id\}/cloudvolumes，两个接口支持的授权信息一致。

授权项列表中，“√”表示支持，“×”表示暂不支持。

<a name="table11136162518266"></a>
<table><thead align="left"><tr id="evs_04_0045_row19140152562617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.1"><p id="evs_04_0045_p5664144515597"><a name="evs_04_0045_p5664144515597"></a><a name="evs_04_0045_p5664144515597"></a>权限</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.2"><p id="evs_04_0045_p19664194585915"><a name="evs_04_0045_p19664194585915"></a><a name="evs_04_0045_p19664194585915"></a>对应API接口</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.3"><p id="evs_04_0045_p18298165452719"><a name="evs_04_0045_p18298165452719"></a><a name="evs_04_0045_p18298165452719"></a>授权项（Action）</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.4"><p id="evs_04_0045_p829825417274"><a name="evs_04_0045_p829825417274"></a><a name="evs_04_0045_p829825417274"></a>IAM项目</p>
<p id="evs_04_0045_p72981254122712"><a name="evs_04_0045_p72981254122712"></a><a name="evs_04_0045_p72981254122712"></a>(Project)</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.1.6.1.5"><p id="evs_04_0045_p162981554202712"><a name="evs_04_0045_p162981554202712"></a><a name="evs_04_0045_p162981554202712"></a>企业项目</p>
<p id="evs_04_0045_p72981354162710"><a name="evs_04_0045_p72981354162710"></a><a name="evs_04_0045_p72981354162710"></a>(Enterprise Project)</p>
</th>
</tr>
</thead>
<tbody><tr id="evs_04_0045_row14183202592618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p1630995419425"><a name="evs_04_0045_p1630995419425"></a><a name="evs_04_0045_p1630995419425"></a>扩容云硬盘（OpenStack Cinder）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p12701151145818"><a name="evs_04_0045_p12701151145818"></a><a name="evs_04_0045_p12701151145818"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p870141175817"><a name="evs_04_0045_p870141175817"></a><a name="evs_04_0045_p870141175817"></a>action="os-extend"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p1350513314414"><a name="evs_04_0045_p1350513314414"></a><a name="evs_04_0045_p1350513314414"></a>evs:volumes:extend</p>
<p id="evs_04_0045_p1938111964"><a name="evs_04_0045_p1938111964"></a><a name="evs_04_0045_p1938111964"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p1260972312332"><a name="evs_04_0045_p1260972312332"></a><a name="evs_04_0045_p1260972312332"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p160992310333"><a name="evs_04_0045_p160992310333"></a><a name="evs_04_0045_p160992310333"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row7188202572612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p14505173334110"><a name="evs_04_0045_p14505173334110"></a><a name="evs_04_0045_p14505173334110"></a>将云硬盘导出为镜像（OpenStack Cinder）</p>
<p id="evs_04_0045_p750573324115"><a name="evs_04_0045_p750573324115"></a><a name="evs_04_0045_p750573324115"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p1870171125811"><a name="evs_04_0045_p1870171125811"></a><a name="evs_04_0045_p1870171125811"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p770151125815"><a name="evs_04_0045_p770151125815"></a><a name="evs_04_0045_p770151125815"></a>action="os-volume_upload_image"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p1350563310410"><a name="evs_04_0045_p1350563310410"></a><a name="evs_04_0045_p1350563310410"></a>evs:volumes:uploadImage</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p612615251337"><a name="evs_04_0045_p612615251337"></a><a name="evs_04_0045_p612615251337"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p1612692563318"><a name="evs_04_0045_p1612692563318"></a><a name="evs_04_0045_p1612692563318"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row919611258261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p1350513334410"><a name="evs_04_0045_p1350513334410"></a><a name="evs_04_0045_p1350513334410"></a>挂载云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p17505183344119"><a name="evs_04_0045_p17505183344119"></a><a name="evs_04_0045_p17505183344119"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p1771715164586"><a name="evs_04_0045_p1771715164586"></a><a name="evs_04_0045_p1771715164586"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p4717516115811"><a name="evs_04_0045_p4717516115811"></a><a name="evs_04_0045_p4717516115811"></a>action="os-attach"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p3505633174113"><a name="evs_04_0045_p3505633174113"></a><a name="evs_04_0045_p3505633174113"></a>evs:volumes:attach</p>
<p id="evs_04_0045_p7683122512614"><a name="evs_04_0045_p7683122512614"></a><a name="evs_04_0045_p7683122512614"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p6674112813319"><a name="evs_04_0045_p6674112813319"></a><a name="evs_04_0045_p6674112813319"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p767452815333"><a name="evs_04_0045_p767452815333"></a><a name="evs_04_0045_p767452815333"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row520272562611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p9505233144119"><a name="evs_04_0045_p9505233144119"></a><a name="evs_04_0045_p9505233144119"></a>卸载云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p12505833184111"><a name="evs_04_0045_p12505833184111"></a><a name="evs_04_0045_p12505833184111"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p171791612583"><a name="evs_04_0045_p171791612583"></a><a name="evs_04_0045_p171791612583"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p19717171616581"><a name="evs_04_0045_p19717171616581"></a><a name="evs_04_0045_p19717171616581"></a>action="os-detach"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p75050336410"><a name="evs_04_0045_p75050336410"></a><a name="evs_04_0045_p75050336410"></a>evs:volumes:detach</p>
<p id="evs_04_0045_p924813014617"><a name="evs_04_0045_p924813014617"></a><a name="evs_04_0045_p924813014617"></a>evs:volumes:get</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p5190432113316"><a name="evs_04_0045_p5190432113316"></a><a name="evs_04_0045_p5190432113316"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p71901732153318"><a name="evs_04_0045_p71901732153318"></a><a name="evs_04_0045_p71901732153318"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row72061525202618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p1550793324114"><a name="evs_04_0045_p1550793324114"></a><a name="evs_04_0045_p1550793324114"></a>保留云硬盘（OpenStack Cinder ）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p9556221585"><a name="evs_04_0045_p9556221585"></a><a name="evs_04_0045_p9556221585"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p20551522115817"><a name="evs_04_0045_p20551522115817"></a><a name="evs_04_0045_p20551522115817"></a>action="os-reserve"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p150711337412"><a name="evs_04_0045_p150711337412"></a><a name="evs_04_0045_p150711337412"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p110813513318"><a name="evs_04_0045_p110813513318"></a><a name="evs_04_0045_p110813513318"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p10108103553311"><a name="evs_04_0045_p10108103553311"></a><a name="evs_04_0045_p10108103553311"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row202111725132618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p17507153311414"><a name="evs_04_0045_p17507153311414"></a><a name="evs_04_0045_p17507153311414"></a>取消保留云硬盘（OpenStack Cinder）</p>
<p id="evs_04_0045_p1450715338413"><a name="evs_04_0045_p1450715338413"></a><a name="evs_04_0045_p1450715338413"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p4551922135816"><a name="evs_04_0045_p4551922135816"></a><a name="evs_04_0045_p4551922135816"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p105512210589"><a name="evs_04_0045_p105512210589"></a><a name="evs_04_0045_p105512210589"></a>action="os-unreserve"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p1250710336417"><a name="evs_04_0045_p1250710336417"></a><a name="evs_04_0045_p1250710336417"></a>evs:volumes:attach</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p11507338163316"><a name="evs_04_0045_p11507338163316"></a><a name="evs_04_0045_p11507338163316"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p1150763819331"><a name="evs_04_0045_p1150763819331"></a><a name="evs_04_0045_p1150763819331"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row3216132515266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p650763354113"><a name="evs_04_0045_p650763354113"></a><a name="evs_04_0045_p650763354113"></a>设置云硬盘启动盘标识（OpenStack Cinder）</p>
<p id="evs_04_0045_p1350713313411"><a name="evs_04_0045_p1350713313411"></a><a name="evs_04_0045_p1350713313411"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p555822145818"><a name="evs_04_0045_p555822145818"></a><a name="evs_04_0045_p555822145818"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p1956132219580"><a name="evs_04_0045_p1956132219580"></a><a name="evs_04_0045_p1956132219580"></a>action="os-set_bootable"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p2050703394118"><a name="evs_04_0045_p2050703394118"></a><a name="evs_04_0045_p2050703394118"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p18572040143318"><a name="evs_04_0045_p18572040143318"></a><a name="evs_04_0045_p18572040143318"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p15857154018334"><a name="evs_04_0045_p15857154018334"></a><a name="evs_04_0045_p15857154018334"></a>×</p>
</td>
</tr>
<tr id="evs_04_0045_row122182572614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.1 "><p id="evs_04_0045_p1750819334410"><a name="evs_04_0045_p1750819334410"></a><a name="evs_04_0045_p1750819334410"></a>设置云硬盘只读标识（OpenStack Cinder）</p>
<p id="evs_04_0045_p250873310414"><a name="evs_04_0045_p250873310414"></a><a name="evs_04_0045_p250873310414"></a></p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.2 "><p id="evs_04_0045_p556162215810"><a name="evs_04_0045_p556162215810"></a><a name="evs_04_0045_p556162215810"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="evs_04_0045_p4561722185810"><a name="evs_04_0045_p4561722185810"></a><a name="evs_04_0045_p4561722185810"></a>action="os-update_readonly_flag"</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.3 "><p id="evs_04_0045_p14508153317415"><a name="evs_04_0045_p14508153317415"></a><a name="evs_04_0045_p14508153317415"></a>evs:volumes:update</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.4 "><p id="evs_04_0045_p1247843103311"><a name="evs_04_0045_p1247843103311"></a><a name="evs_04_0045_p1247843103311"></a>√</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.1.6.1.5 "><p id="evs_04_0045_p54794323313"><a name="evs_04_0045_p54794323313"></a><a name="evs_04_0045_p54794323313"></a>×</p>
</td>
</tr>
</tbody>
</table>

