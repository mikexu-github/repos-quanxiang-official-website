---
title: "创建 API"
description: "API 创建流程介绍"
keywords: "API"
linkTitle: "创建 API"
weight: 7360
---

创建 API 即录入需要可视化编排的 API 的信息。本小节主要介绍如何快速创建 API 。

## 前提条件

- 已创建 API 分组。如果未创建 API 分组，参考 [创建 API 分组](../create_apigroup/) 进行创建。



## 新建 API 

按照以下步骤，创建 API。

1. 选择需要新建 API 的 API 分组，点击 **新建 API**。

   ![create_api1](/images/api/arrange/create_api1.png)

2. 在弹框中填写 API 信息，确认后点击新建并设计 API。

   {{<table >}}

   | 参数     | 描述                                                         |
   | -------- | ------------------------------------------------------------ |
   | API 名称 | 所创建的 API 的名称，API 名称标识需在所属分组内具有唯一性。<br/>**说明**：最多可填写 20 个字符，支持中文或英文字符。 |
   | API 标识 | API 标识需用英文标识，作为 API 唯一标识，不可重复。<br/>**说明**：最多可填写 20 个字符，必须以字母开头，只能包含字母、数字、下划线。 |
   | 描述     | API 的相关描述。                                             |

   {{</table >}}

3. 创建成功后跳转进入 API 设计页面，详细流程及参数说明参见：[编排 API](../arrange_api/)。

    ![create_api2](/images/api/arrange/create_api2.png)

4. 编排完成后，点击调试，调试成功后即可上线。

5. 上线后在 API 列表中可以看到 API 基本信息。详细说明参见下表。



## API 参数说明

{{<table >}}

| 参数     | 描述                                                         |
| -------- | ------------------------------------------------------------ |
| API 名称 | 所创建的 API 的名称，API 名称标识需在所属分组内具有唯一性。<br/>**说明**：最多可填写 20 个字符，支持中文或英文字符。 |
| 请求方法 | 目前仅支持 POST 方法，系统自动生成。                         |
| 访问路径 | 系统自动生成，用户调用 API 的路径。                          |
| 描述     | API 的相关描述。                                             |
| 状态     | 点击切换状态，支持上线、下线。                               |
| 操作     | 支持设计 API、复制、删除。                                   |

{{</table >}}

