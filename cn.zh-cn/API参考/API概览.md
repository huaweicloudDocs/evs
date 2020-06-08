# API概览<a name="zh-cn_topic_0124881427"></a>

云硬盘所提供的接口分为EVS自定义API与OpenStack Cinder API。

通过配合使用EVS自定义API与OpenStack Cinder API，您可以完整的使用云硬盘的所有功能。此外，部分扩展接口提供了基于企业项目的授权功能，具体在该接口的功能介绍中有描述，如果您需要使用企业项目授权功能，建议您调用这部分接口。

**表 1**  接口说明

<a name="zh-cn_topic_0121588224_table5876102613294"></a>
<table><thead align="left"><tr id="zh-cn_topic_0121588224_row3878122616298"><th class="cellrowborder" valign="top" width="17%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0121588224_p487811268290"><a name="zh-cn_topic_0121588224_p487811268290"></a><a name="zh-cn_topic_0121588224_p487811268290"></a><strong id="zh-cn_topic_0121588224_b1251874443714"><a name="zh-cn_topic_0121588224_b1251874443714"></a><a name="zh-cn_topic_0121588224_b1251874443714"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="18.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0121588224_p68781126182914"><a name="zh-cn_topic_0121588224_p68781126182914"></a><a name="zh-cn_topic_0121588224_p68781126182914"></a><strong id="zh-cn_topic_0121588224_b125201844173712"><a name="zh-cn_topic_0121588224_b125201844173712"></a><a name="zh-cn_topic_0121588224_b125201844173712"></a>子类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="64.02%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0121588224_p158781726112914"><a name="zh-cn_topic_0121588224_p158781726112914"></a><a name="zh-cn_topic_0121588224_p158781726112914"></a><strong id="zh-cn_topic_0121588224_b15203449370"><a name="zh-cn_topic_0121588224_b15203449370"></a><a name="zh-cn_topic_0121588224_b15203449370"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row8756133619716"><td class="cellrowborder" rowspan="3" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="p1953888887"><a name="p1953888887"></a><a name="p1953888887"></a>API</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.2 "><p id="p115392818814"><a name="p115392818814"></a><a name="p115392818814"></a>云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="64.02%" headers="mcps1.2.4.1.3 "><p id="p6540881586"><a name="p6540881586"></a><a name="p6540881586"></a>该部分API提供云硬盘的创建、删除、云硬盘详情查询等操作。</p>
</td>
</tr>
<tr id="row1340619396716"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p115407810816"><a name="p115407810816"></a><a name="p115407810816"></a>云硬盘快照</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p2054113817818"><a name="p2054113817818"></a><a name="p2054113817818"></a>云硬盘快照指的是云硬盘数据在某个时刻的完整拷贝或镜像。</p>
<p id="p1054112812817"><a name="p1054112812817"></a><a name="p1054112812817"></a>该部分API提供回滚快照数据至云硬盘的操作。</p>
</td>
</tr>
<tr id="row94071041170"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="p454219817815"><a name="p454219817815"></a><a name="p454219817815"></a>云硬盘标签</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p55421681582"><a name="p55421681582"></a><a name="p55421681582"></a>标签用于标识云资源，可通过标签实现对云资源的分类和搜索。</p>
<p id="p971310714105"><a name="p971310714105"></a><a name="p971310714105"></a>该部分API提供云硬盘标签的添加、删除、查询等操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row148781026122919"><td class="cellrowborder" rowspan="4" valign="top" width="17%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121588224_p16878726162916"><a name="zh-cn_topic_0121588224_p16878726162916"></a><a name="zh-cn_topic_0121588224_p16878726162916"></a>OpenStack Cinder API</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121588224_p128788265295"><a name="zh-cn_topic_0121588224_p128788265295"></a><a name="zh-cn_topic_0121588224_p128788265295"></a>云硬盘</p>
</td>
<td class="cellrowborder" valign="top" width="64.02%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0121588224_p56591328178"><a name="zh-cn_topic_0121588224_p56591328178"></a><a name="zh-cn_topic_0121588224_p56591328178"></a>该部分API提供云硬盘的创建、更新、云硬盘列表查询、镜像列表查询、租户配额查询等操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row1987820263297"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121588224_p8939172693215"><a name="zh-cn_topic_0121588224_p8939172693215"></a><a name="zh-cn_topic_0121588224_p8939172693215"></a>云硬盘Action</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0121588224_p86434284717"><a name="zh-cn_topic_0121588224_p86434284717"></a><a name="zh-cn_topic_0121588224_p86434284717"></a>该部分API提供云硬盘的扩容、保留、导出镜像、设置启动盘表示等操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row87746166614"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121588224_p197741716567"><a name="zh-cn_topic_0121588224_p197741716567"></a><a name="zh-cn_topic_0121588224_p197741716567"></a>云硬盘快照</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p574018556012"><a name="p574018556012"></a><a name="p574018556012"></a>云硬盘快照指的是云硬盘数据在某个时刻的完整拷贝或镜像。</p>
<p id="zh-cn_topic_0121588224_p1477491610610"><a name="zh-cn_topic_0121588224_p1477491610610"></a><a name="zh-cn_topic_0121588224_p1477491610610"></a>该部分API提供云硬盘快照的创建、快照列表查询、快照元数据更新、快照元数据查询等操作。</p>
</td>
</tr>
<tr id="zh-cn_topic_0121588224_row816313459617"><td class="cellrowborder" valign="top" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0121588224_p1216317451267"><a name="zh-cn_topic_0121588224_p1216317451267"></a><a name="zh-cn_topic_0121588224_p1216317451267"></a>云硬盘过户</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.2.4.1.2 "><p id="p1876353719210"><a name="p1876353719210"></a><a name="p1876353719210"></a>通过云硬盘过户功能把一个租户的云硬盘过户给另一个租户，过户成功后，该云硬盘就属于接受过户的租户。</p>
<p id="p1948613421824"><a name="p1948613421824"></a><a name="p1948613421824"></a>该部分API提供云硬盘过户的创建、接受、删除、过户记录查询等操作。</p>
</td>
</tr>
</tbody>
</table>

