---
title: "基础操作指引"
description: "组件定义，表单和字段，字段与组件的关系"
linkTitle: "基础操作指引"
weight: 4221
---

## 定义

全象云平台将具有相同数据特征的字段封装为组件、每种组件都有相应的数据格式验证方式和属性特征。

目前提供了基础字段、高级字段、布局字段等 21 种组件，开发者使用这些组件可以快速搭建表单。

![basic_operation](/images/manual/form/basic_operation.png)

## 表与字段、字段与组件关系

**表与字段**：工作表是用来存储业务对象的数据集，一个数据表完成填写后会生成一条记录，每个对象有很多相同的属性，在存储这些对象数据的表中，对象的属性叫做字段。例如：【员工信息表】中包含：姓名、电话号码、邮箱、归属部门等字段。

{{<table >}}
| 姓名 | 联系电话 | 出生日期   | ..   |
| ---- | -------- | ---------- | ---- |
| 张三 | 18...    | 1990.01.01 | ..   |
| 李四 | 13...    | 1998.10.29 | ..   |
{{</table >}}


**字段与组件**：为了字段数据的规范和正确的输入，全象云系统预先设置了一些格式化的字段类型，即组件。例如：时间日期组件、单选框组件、复选框组件等等。 表单中添加字段时，请先根据此字段的数据类型选择合适的组件。

## 字段基础操作

字段包含以下几项基础设置：

- 添加字段
- 删除字段
- 复制字段
- 调整位置
- 属性设置

### 添加字段、属性设置

点击或拖拽组建到表单区域即可完成字段添加，字段添加完成后在 **字段属性栏** 根据需要进行属性配置。

![basic_operation1](/images/manual/form/basic_operation1.png)

{{< alert tip >}}

**说明**

字段属性设置包含：标题名称、占位提示、描述内容等。不同字段属性不同，基础组件属性详情参见：[基础组件](../../component/basic_component/)，增强组件属性参见：[增强组件](../../../../manual/form/component/enhance/)。

{{</ alert >}}

### 删除字段、复制字段、调整位置

- **删除字段**：点击删除按钮即可删除字段；
- **复制字段**：点击复制按钮即可复制字段；
- **调整位置**：支持选中调整字段布局。

<img src="/images/manual/form/basic_operation2.png" alt="basic_operation2" style="zoom:67%;" />

{{< alert tip >}}

**说明**

删除字段请谨慎，如果字段已有数据，字段删除后数据将随之消息且无法恢复。

{{</ alert >}}

