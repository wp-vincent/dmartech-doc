---
description: 表单是收集联系人信息的有效工具，可以直接将联系人数据引流到Dmartech平台。
---

# 表单

表单可以直接下发给用户也可以部署在网站等页面收集联系人信息，Dmartech平台有两类表单，一类是使用平台的编辑器直接创建的表单，成为“标准表单“；一类是金数据表单，通过对接金数据账号接入在金数据创建的表单，称为“金数据表单“。

## 表单管理

依次点击进入“营销旅程“—表单，进入素材管理页面。

支持对素材分组管理，左侧是分组栏，右侧是素材列表，系统内置了三个分组：全部素材、我创建的、共享给我的

* 全部表单：当前所有的表单，包括系统表单、金数据表单
* 我创建的：使用账号下创建的素材
* 共享给我的：表单是可以共享的，后续会详细介绍，其他账号共享过来的表单都在该分组中 

![](../.gitbook/assets/image%20%2832%29.png)

除了系统内置的分组之外，用户可以按需自行创建分组，方便表单过多时的管理。右侧表单列表分别按照全部表单、Dmartech表单、金数据表单分类。

## 标准表单

1、为了让用户提交的表单字段值能正确收集到Dmartech，在创建表单\(标准表单和金数据表单都一样\)之前，需要先在元数据（“数据中心“—“元数据“—用户属性）中创建表单将用到的字段，如果是已有的用户属性则无需创建，若是没有的，则需要新增。

![&#x5728;&#x5143;&#x6570;&#x636E;&#x65B0;&#x589E;&#x8868;&#x5355;&#x5B57;&#x6BB5;](../.gitbook/assets/666.gif)

2、点击表单列表页面右上角“创建表单“按钮，可以看到Dmartech提供了两种表单创建方式：标准表单和接入金数据表单。在表单列表的“表单来源列“会显示表单的类型。选择表单分组后，点击“标准表单“则进入表单编辑器。

![](../.gitbook/assets/777%20%281%29.gif)

3、单编辑器为左中右布局，左侧为字段选择区，中间为表单展示区，右侧为字段设置区。

![&#x56FE;2-2&#x8868;&#x5355;&#x7F16;&#x8F91;&#x754C;&#x9762;](../.gitbook/assets/tu-pian-17.png)

1）在表单上方编辑表单名称和HTML名称（指导出的HTML文件的名称）

 2）在左侧字段选择区选择所需的字段或字段类型，点击即可添加至表单；

 3）点击表单中字段，在右侧设置相关字段属性，包括字段名称、HTML名称（指在HTML代码中显示的名称）、默认值、提示以及校验等，不同字段可设置校验内容不同，一般包括设置必填项、不能与已有字段重复、字符限制等。

 4）表单创建完成后，点击保存，页面跳转至“字段匹配”页面，**此时在表单右上角会出现表单链接（可复制）、表单二维码（扫描可预览表单），以及导出HTML按钮，点击可导出当前表单HTML源代码，可用于表单二次加工。**

![&#x8868;&#x5355;&#x94FE;&#x63A5;&#x53CA;&#x5BFC;&#x51FA;HTML](../.gitbook/assets/tu-pian-18.png)

5）保存后页面将跳转至“字段匹配”阶段，将表单中创建的字段与元数据中创建的与之对应的字段进行关联，保证正确的收集信息。

![](../.gitbook/assets/image%20%28415%29.png)

6）点击“完成”则创建成功。

 7）表单创建完成，还可以进行表单相关其他设置。

#### 其他设置

**A：扩展属性**

扩展属性一般用于区分表单数据来源，通过为表达链接添加一个扩展属性字段，由该字段判断表单数据的来源渠道。最多可设置三层扩展属性。

![&#x8868;&#x5355;&#x6269;&#x5C55;&#x5C5E;&#x6027;&#x8BBE;&#x7F6E;](../.gitbook/assets/tu-pian-20.png)

**B：跳转设置**

用于设置用户提交表单后页面的指向。支持三种跳转方式：默认跳转、规则设置、隐藏字段跳转。

 a\)默认跳转是指，所有的用户提交表单后都跳转至默认跳转中设置的内容页面。支持设置默认提交成功、文本、富文本、链接。

![&#x9ED8;&#x8BA4;&#x8DF3;&#x8F6C;](../.gitbook/assets/wei-xin-jie-tu-20190925105121.png)

b）规则设置是指，根据用户表单中填写的某字段值跳转至不同的页面，操作为选择字段、字段值，设置对应的跳转链接。以及字段未匹配时的跳转链接。

![&#x8868;&#x5355;&#x8DF3;&#x8F6C;&#x8BBE;&#x7F6E;&#xFF1A;&#x89C4;&#x5219;&#x8BBE;&#x7F6E;](../.gitbook/assets/wei-xin-jie-tu-20190925105232.png)

c）隐藏字段跳转是指，表单代码中新增了一个隐藏字段【GOTOURL】，由前端开发人员在html代码中写入跳转链接，适用于需二次开发的表单。

![&#x8868;&#x5355;&#x8DF3;&#x8F6C;&#x8BBE;&#x7F6E;&#xFF1A;&#x9690;&#x85CF;&#x5B57;&#x6BB5;&#x8DF3;&#x8F6C;](../.gitbook/assets/wei-xin-jie-tu-20190925104850%20%281%29.png)

8）以上内容都设置完毕后，表单就可以投放使用了。表单投放后，在操作栏点击“表单统计”图标，可以查看表单收集到的全部数据。

![&#x8868;&#x5355;&#x7EDF;&#x8BA1;&#x754C;&#x9762;](../.gitbook/assets/tu-pian-24.png)

点击右上角“报告发送设置”可按照规则将报告发送到指定的邮箱内

![&#x8868;&#x5355;&#x7EDF;&#x8BA1;&#x62A5;&#x544A;&#x53D1;&#x9001;](../.gitbook/assets/tu-pian-25.png)

a\)规则名称：可设置多个报告发送规则，因此每个规则需设置一个名称 

b\)字段筛选：设置字段筛选条件，报告将包含符合筛选条件的字段数据 

c\)添加筛选条件：仅符合筛选条件的数据才会导出到CSV报告内 

d\)发送时间：可设置立即发送、定时发送和周期发送 

e\)接收邮箱：添加接收报告的邮箱

## 表单的下发与使用

标准表单不能通过二维码和模板消息下发，可以直接投放表单二维码。

## 表单其他基本操作

表单操作：编辑、表单统计、暂停、共享

* 编辑：已下发的表单，编辑后，只有保留的原来的字段值会被收集到，其他字段不会被收集；
* 表单统计：查看表单提交详情，统计表单提交人数与提交次数
* 暂停：暂停后提交的表单数据将不会被收集
* 共享：表单可以共享给其他账户或安全组（关于安全组的详细内容请查看“[企业设置](../ge-ren-zhong-xin/qi-ye-she-zhi.md)“），并可限制对共享表单的操作权限。

![](../.gitbook/assets/image%20%28456%29.png)





