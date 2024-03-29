---
title: "什么是 API 编排"
description: "全象云 API 编排功能介绍"
keywords: "API"
linkTitle: "什么是 API 编排"
weight: 7351
---

API 编排是指把已经开发好的 API 接口按照一定的业务逻辑和流程进行可视化编排的过程。通过 API 编排，可以进行业务逻辑的重组与重构，能够提升 API 的复用效率。

全象云 API 编排用于接入和管理后端（包括第三方）API，提供权限控制、隐私管理、聚合编排、组合输出、规范化调用等服务。前端开发者可以根据业务需求及页面所需数据，定制实现页面所需的**聚合 API**。

平台支持通过 API 聚合和 API 编排生成聚合 API，用户仅需调用一次聚合 API 即可获取多个 API 的数据。

{{< alert tip >}}
**说明**

API 的传统调用方式为：需要展示 n 个 API 数据，则调用 n 次 。
{{</ alert >}}

## API 编排应用场景

API 编排即在 API 网关中实现一种机制，用于灵活调用和组装后端原生 API，使前端能够根据业务需求，定制实现页面所需的**聚合 API**。

一个典型的 API 编排应用案例如下：

![intro](/images/api/arrange/intro.png)

**图注**：图中方框大小示意调用时数据量大小。

可以看出，与后端微服务 API 以“高内聚”为目标不同，聚合 API 以业务需求为导向，通过简单组合已有的原生 API，在后端代理调用多个API，并对输出数据进行重新剪裁组装。

## API 编排优势

与前端直接调用多个异构的后端 API 相比，聚合 API 具有很明显的优势：

- 简化前端逻辑，一次 API 调用即可获取所有所需数据；
- 减少传输数据量，仅向前端发送需要展示的数据；
- 灵活的动态组合扩展特性，后端只需要实现“原子 API”，把业务需求交给消费方去**自助配置**，**组合扩展**；
- 同化调用方法，由 API 编排服务兼容异构实现的后端 API 的调用过程；
- 统一的身份认证和权限管理；
- 向前端隐藏第三方 API 的身份认证过程，由 API 编排服务兼容不同平台的 API 认证方法。
