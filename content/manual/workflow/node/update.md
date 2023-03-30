---
title: "数据更新节点"
description: "全象云平台工作流：数据更新节点介绍。"
linkTitle: "数据更新节点"
weight: 44221
---

数据更新节点用于业务流程中，更新某条记录中一个或多个字段的值。支持更新本表字段或关联他表字段。

## 应用场景

- 工作表【商品库存】中，商品出库时自动减少库存记录中当前商品的库存值。
- 工作表【退货单详情】中，如果通过申请，则将工作表【商品库存】记录中 更新商品库存值。

## 配置步骤

### 1、添加数据更新节点

工作流中点击 **+** ，在弹出的组件集中拖动 **数据更新组件** 到工作流中。

{{< alert tip >}}

**说明**

数据更新节点支持重命名，点击节点名称 **数据更新** 即可重命名。

{{</ alert >}}

### 2、添加基础配置

#### 选择目标数据表

根据业务需求选择目标数据表。流程设计中支持切换数据表。

{{< alert warning >}}

**注意**

切换数据表后，原有数据更新的配置将被清空，请确认后切换。

 {{</ alert >}}

![update1](/images/manual/workflow/update1.png)

#### 设置表单数据是否触发工作流执行

根据业务需求设置表单数据与触发工作流执行的关系。系统默认选中。

{{< alert tip >}}

**案例**

工作表【请假统计】，在数据生成之后是否需要复核，需根据公司业务来决定。若是比较简单的统计则无需触发工作流；若带有金额的计算，则需要复核。

{{</ alert >}}

#### 设置过滤条件

1. 选择过滤条件关系：满足以下所有、任一。

2. 定义目标字段，支持定义{等于，不等于，包含，不包含}。

   ![update2](/images/manual/workflow/update2.png)

#### 设置更新规则

1. 选择目标表更新字段。
2. 设置字段更新规则：支持设置字段值、自定义、公式计算、流程变量。
   - 字段值：选择当前数据表中对应字段；

   - 自定义：数值自定义；

   - 公式计算：支持编辑公式设定更新规则；

   - 流程变量：需提前在工作流变量中定义，定义好后可直接引用。定义规则参见：[工作流变量](../../../../manual/workflow/variables/)。

     ![update3](/images/manual/workflow/update3.png)


