---
title: "多行文本"
description: "单行文本组件定义和字段属性"
linkTitle: "多行文本"
weight: 42212
---

## 组件定义

多行文本常用于录入长内容的信息，如：订单详情、备注、会议记录、反馈等。暂不支持和富文本组件的互相转换。

## 字段属性

![多行文本_属性](/images/manual/component/多行文本_属性.png)

请根据实际需要配置字段的以下属性：

- 标题名称：字段名称，必填；
- 占位提示：如有需要请填写；
- 描述内容：如有需要请填写；
- 格式：支持多种数据格式，详情参见下文格式；
- 字段属性：支持设置成普通、只读、隐藏，默认为普通；
- 是否必填：可选择字段是否必填，默认非必填；
- 数据源：支持自定义；
- 默认值：如有需要请输入。

### 格式

在多行文本组件中，支持预设数据格式，起到字段校验的作用。目前仅支持中国范围的数据校验：

- **无**：汉字或数字；
- **固定电话**：0 开头的区号-座机号-分机号，其中区号和分机号可选填；
- **邮编号码**：6 位数字；
- **手机号码**：1 开头的 11 位数字；
- **身份证号**：采用正则表达式进行校验；
  - 身份证长度 18 位，前 17 位必然为数字；
  - 前两位省份数字在 11 到 82 区间；
  - 从第七位开始的六位生日码符合日期校验；
  - 最后一位可以是数字、大写X；
- **邮箱**：xxx@xxx.xxx。

