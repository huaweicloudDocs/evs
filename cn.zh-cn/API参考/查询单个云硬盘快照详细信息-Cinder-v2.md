# 查询单个云硬盘快照详细信息<a name="ZH-CN_TOPIC_0051408628"></a>

## 功能介绍<a name="section30030484111731"></a>

查询单个云硬盘快照信息。

## URI<a name="section14733765111731"></a>

-   URI格式

    GET /v2/\{project\_id\}/snapshots/\{snapshot\_id\}

-   参数说明

    <a name="table66271751111731"></a>
    <table><thead align="left"><tr id="row56106054111731"><th class="cellrowborder" valign="top" width="28.57%" id="mcps1.1.4.1.1"><p id="p48296540111731"><a name="p48296540111731"></a><a name="p48296540111731"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.1.4.1.2"><p id="p19705674111731"><a name="p19705674111731"></a><a name="p19705674111731"></a>是否必选</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.9%" id="mcps1.1.4.1.3"><p id="p52655801111731"><a name="p52655801111731"></a><a name="p52655801111731"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row37261521111731"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p65393209111731"><a name="p65393209111731"></a><a name="p65393209111731"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p62358553111731"><a name="p62358553111731"></a><a name="p62358553111731"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p17878042111731"><a name="p17878042111731"></a><a name="p17878042111731"></a>项目ID。</p>
    </td>
    </tr>
    <tr id="row26684654111731"><td class="cellrowborder" valign="top" width="28.57%" headers="mcps1.1.4.1.1 "><p id="p13973379111731"><a name="p13973379111731"></a><a name="p13973379111731"></a>snapshot_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.1.4.1.2 "><p id="p58101900111731"><a name="p58101900111731"></a><a name="p58101900111731"></a>是</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.9%" headers="mcps1.1.4.1.3 "><p id="p8633458111731"><a name="p8633458111731"></a><a name="p8633458111731"></a>快照ID</p>
    </td>
    </tr>
    </tbody>
    </table>


## 请求<a name="section28221468111731"></a>

无

## 响应<a name="section63055193111836"></a>

-   响应参数

    <a name="table46086870111836"></a>
    <table><thead align="left"><tr id="row56202297111836"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="p56092213111836"><a name="p56092213111836"></a><a name="p56092213111836"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="p47175401111836"><a name="p47175401111836"></a><a name="p47175401111836"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="p11730844111836"><a name="p11730844111836"></a><a name="p11730844111836"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row10674282111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p59310480111836"><a name="p59310480111836"></a><a name="p59310480111836"></a>snapshot</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p39419575111836"><a name="p39419575111836"></a><a name="p39419575111836"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p61381158111836"><a name="p61381158111836"></a><a name="p61381158111836"></a>快照信息。</p>
    </td>
    </tr>
    <tr id="row15559516111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p52361272111836"><a name="p52361272111836"></a><a name="p52361272111836"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p13404600111836"><a name="p13404600111836"></a><a name="p13404600111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p34969797111836"><a name="p34969797111836"></a><a name="p34969797111836"></a>云硬盘快照ID。</p>
    </td>
    </tr>
    <tr id="row46292725111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p58723264111836"><a name="p58723264111836"></a><a name="p58723264111836"></a>status</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p58963956111836"><a name="p58963956111836"></a><a name="p58963956111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p47023540111836"><a name="p47023540111836"></a><a name="p47023540111836"></a>云硬盘快照的状态，具体请参见<a href="云硬盘快照状态.md">云硬盘快照状态</a>。</p>
    </td>
    </tr>
    <tr id="row20558679111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p54640283111836"><a name="p54640283111836"></a><a name="p54640283111836"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p63786796111836"><a name="p63786796111836"></a><a name="p63786796111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p14293074111836"><a name="p14293074111836"></a><a name="p14293074111836"></a>云硬盘快照名称。</p>
    </td>
    </tr>
    <tr id="row61528809111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p17777665111836"><a name="p17777665111836"></a><a name="p17777665111836"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p30704745111836"><a name="p30704745111836"></a><a name="p30704745111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p60132426111836"><a name="p60132426111836"></a><a name="p60132426111836"></a>云硬盘快照描述信息。</p>
    </td>
    </tr>
    <tr id="row4320926111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p14450739111836"><a name="p14450739111836"></a><a name="p14450739111836"></a>created_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p29659196111836"><a name="p29659196111836"></a><a name="p29659196111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p45391308111836"><a name="p45391308111836"></a><a name="p45391308111836"></a>云硬盘快照创建时间。</p>
    </td>
    </tr>
    <tr id="row3737236411149"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p80695711149"><a name="p80695711149"></a><a name="p80695711149"></a>update_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p6536351711149"><a name="p6536351711149"></a><a name="p6536351711149"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p2439511411149"><a name="p2439511411149"></a><a name="p2439511411149"></a>云硬盘快照更新时间。</p>
    </td>
    </tr>
    <tr id="row5868590111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p5593786111836"><a name="p5593786111836"></a><a name="p5593786111836"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p50443518111836"><a name="p50443518111836"></a><a name="p50443518111836"></a>map</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p46118865111836"><a name="p46118865111836"></a><a name="p46118865111836"></a>云硬盘快照的元数据信息。</p>
    <p id="p771812911458"><a name="p771812911458"></a><a name="p771812911458"></a>如果元数据中包含__system__enableActive字段，则表示该快照为云服务器创建备份时自动生成的快照。</p>
    </td>
    </tr>
    <tr id="row12416602111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p66220711111836"><a name="p66220711111836"></a><a name="p66220711111836"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p62277393111836"><a name="p62277393111836"></a><a name="p62277393111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p43213914111836"><a name="p43213914111836"></a><a name="p43213914111836"></a>快照所属的云硬盘。</p>
    </td>
    </tr>
    <tr id="row53380907111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p28886228111836"><a name="p28886228111836"></a><a name="p28886228111836"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p58083101111836"><a name="p58083101111836"></a><a name="p58083101111836"></a>int</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p39095984111836"><a name="p39095984111836"></a><a name="p39095984111836"></a>云硬盘快照大小。</p>
    </td>
    </tr>
    <tr id="row16319538111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p46814240111836"><a name="p46814240111836"></a><a name="p46814240111836"></a>os-extended-snapshot-attributes:project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p33857106111836"><a name="p33857106111836"></a><a name="p33857106111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p6137764111836"><a name="p6137764111836"></a><a name="p6137764111836"></a>租户ID。</p>
    </td>
    </tr>
    <tr id="row55239881111836"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="p45245366111836"><a name="p45245366111836"></a><a name="p45245366111836"></a>os-extended-snapshot-attributes:progress</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="p40996011111836"><a name="p40996011111836"></a><a name="p40996011111836"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="p18028606145913"><a name="p18028606145913"></a><a name="p18028606145913"></a>创建快照进度。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "snapshot": {
            "status": "available",
            "os-extended-snapshot-attributes:progress": "100%",
            "description": "daily backup",
            "created_at": "2013-02-25t04:13:17.000000",
            "metadata": {},
            "volume_id": "5aa119a8-d25b-45a7-8d1b-88e127885635",
            "os-extended-snapshot-attributes:project_id": "0c2eba2c5af04d3f9e9d0d410b371fde",
            "size": 1,
            "id": "2bb856e1-b3d8-4432-a858-09e4ce939389",
            "name": "snap-001",
            "updated_at": null
    
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
        "itemNotFound": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## 返回值<a name="section38811440112026"></a>

-   正常

    200


## 错误码<a name="section431317151242"></a>

请参考[错误码说明](错误码说明.md)。

