---
title: "CloudEvents 规范概述"
linkTitle: "规范概述"
weight: 1
description: >
  事件随处可见。 然而，事件生产者往往以不同的方式描述事件。
type: "docs"
---

![CloudEvents logo](https://github.com/cncf/artwork/blob/master/projects/cloudevents/horizontal/color/cloudevents-horizontal-color.png)

缺乏描述事件意味着开发者必须不断地重新学习如何消费事件的一种常见方式。
这也限制了库，工具和基础设施的电势到助手事件数据的传送在不同环境，像的 SDK，事件路由器或跟踪系统。
我们可以从事件数据实现了便携性和生产力总体阻碍。

CloudEvents 是用于描述常见格式的事件数据跨服务，平台和系统提供互操作性的规范。

CloudEvents 已经收到了大量的产业利益，从主要云供应商流行的 SaaS 公司。
CloudEvents 由[云本地计算基金](https://cncf.io) (CNCF)主持，被批准为在云本地沙箱级项目[2018 5 月 15 日](https://docs.google.com/presentation/d/1KNSv70fyTfSqUerCnccV7eEC_ynhLsm9A_kjnlmU_t0/edit#slide=id.g37acf52904_1_41).

## CloudEvents 文档

下列文档可用:

|                        |                                    最新发布                                     |                                      工作草案                                       |
| :--------------------- | :-----------------------------------------------------------------------------: | :---------------------------------------------------------------------------------: |
| **核心规范:**          |
| CloudEvents            |          [v1.0](https://github.com/cloudevents/spec/blob/v1.0/spec.md)          |          [master](https://github.com/cloudevents/spec/blob/master/spec.md)          |
|                        |
| **可选规范:**          |
| AMQP Protocol Binding  | [v1.0](https://github.com/cloudevents/spec/blob/v1.0/amqp-protocol-binding.md)  | [master](https://github.com/cloudevents/spec/blob/master/amqp-protocol-binding.md)  |
| AVRO Event Format      |      [v1.0](https://github.com/cloudevents/spec/blob/v1.0/avro-format.md)       |      [master](https://github.com/cloudevents/spec/blob/master/avro-format.md)       |
| HTTP Protocol Binding  | [v1.0](https://github.com/cloudevents/spec/blob/v1.0/http-protocol-binding.md)  | [master](https://github.com/cloudevents/spec/blob/master/http-protocol-binding.md)  |
| JSON Event Format      |      [v1.0](https://github.com/cloudevents/spec/blob/v1.0/json-format.md)       |      [master](https://github.com/cloudevents/spec/blob/master/json-format.md)       |
| Kafka Protocol Binding | [v1.0](https://github.com/cloudevents/spec/blob/v1.0/kafka-protocol-binding.md) | [master](https://github.com/cloudevents/spec/blob/master/kafka-protocol-binding.md) |
| MQTT Protocol Binding  | [v1.0](https://github.com/cloudevents/spec/blob/v1.0/mqtt-protocol-binding.md)  | [master](https://github.com/cloudevents/spec/blob/master/mqtt-protocol-binding.md)  |
| NATS Protocol Binding  | [v1.0](https://github.com/cloudevents/spec/blob/v1.0/nats-protocol-binding.md)  | [master](https://github.com/cloudevents/spec/blob/master/nats-protocol-binding.md)  |
| Web hook               |      [v1.0](https://github.com/cloudevents/spec/blob/v1.0/http-webhook.md)      |      [master](https://github.com/cloudevents/spec/blob/master/http-webhook.md)      |
|                        |
| **其他文档:**          |
| CloudEvents 适配器     |                                        -                                        |        [master](https://github.com/cloudevents/spec/blob/master/adapters.md)        |
| CloudEvents SDK 要求   |                                        -                                        |          [master](https://github.com/cloudevents/spec/blob/master/SDK.md)           |
| 文件扩展               |                                        -                                        | [master](https://github.com/cloudevents/spec/blob/master/documented-extensions.md)  |
| 入门                   |         [v1.0](https://github.com/cloudevents/spec/blob/v1.0/primer.md)         |         [master](https://github.com/cloudevents/spec/blob/master/primer.md)         |
| 专有技术指标           |                                        -                                        |   [master](https://github.com/cloudevents/spec/blob/master/proprietary-specs.md)    |

如果你是新来 CloudEvents，建议您通过阅读[入门](primer.md)为规范的目标和设计决策的概述开始，然后移动到[核心规格](spec.md).

由于并非所有事件生产者默认生成 CloudEvents，有是描述为适应一些热门事件到 CloudEvents 推荐的过程文档，请参阅[CloudEvents 适配器](https://github.com/cloudevents/spec/blob/master/adapters.md).

## SDKs

除了如上所述文档， 也有一个[SDK 建议](SDK.md)和一套软件开发工具包的开发:

- [CSharp](https://github.com/cloudevents/sdk-csharp)
- [Go](https://github.com/cloudevents/sdk-go)
- [Java](https://github.com/cloudevents/sdk-java)
- [Javascript](https://github.com/cloudevents/sdk-javascript)
- [Python](https://github.com/cloudevents/sdk-python)
- [Ruby](https://github.com/cloudevents/sdk-ruby)

## 社区

Learn more about the people and organizations who are creating a dynamic cloud
native ecosystem by making our systems interoperable with CloudEvents.

- [Contributors](community/contributors.md): people and organizations who helped
  us get started or are actively working on the CloudEvents specification.
- Coming soon: [demos & open source](community/README.md) -- if you have
  something to share about your use of CloudEvents, please submit a PR!

## 处理

The CloudEvents project is working to formalize the [specification](spec.md)
based on [design goals](primer.md#design-goals) which focus on interoperability
between systems which generate and respond to events.

In order to achieve these goals, the project must describe:

- Common attributes of an _event_ that facilitate interoperability
- One or more common architectures that are in active use today or planned to be
  built by its members
- How events are transported from producer to consumer via at least one protocol
- Identify and resolve whatever else is needed for interoperability

## 通讯

The main mailing list for e-mail communications:

- Send emails to: [cncf-cloudevents](mailto:cncf-cloudevents@lists.cncf.io)
- To subscribe see: https://lists.cncf.io/g/cncf-cloudevents
- Archives are at: https://lists.cncf.io/g/cncf-cloudevents/topics

And a #cloudevents Slack channel under
[CNCF's Slack workspace](https://slack.cncf.io/).

For SDK related comments and questions:

- Email to: [cncf-cloudevents-sdk](mailto:cncf-cloudevents-sdk@lists.cncf.io)
- To subscribe see: https://lists.cncf.io/g/cncf-cloudevents-sdk
- Archives are at: https://lists.cncf.io/g/cncf-cloudevents-sdk/topics
- Slack: #cloudeventssdk on [CNCF's Slack workspace](https://slack.cncf.io/)

## 会议时间

See the [CNCF public events calendar](https://www.cncf.io/community/calendar/).
This specification is being developed by the
[CNCF Serverless Working Group](https://github.com/cncf/wg-serverless). This
working group meets every Thursday at 9AM PT (USA Pacific):

Join from PC, Mac, Linux, iOS or Android: https://zoom.us/my/cncfserverlesswg

Or iPhone one-tap :

    US: +16465588656,,3361029682#  or +16699006833,,3361029682#

Or Telephone:

    Dial:
        US: +1 646 558 8656 (US Toll) or +1 669 900 6833 (US Toll)
        or +1 855 880 1246 (Toll Free) or +1 877 369 0926 (Toll Free)

Meeting ID: 336 102 9682

International numbers available:
https://zoom.us/zoomconference?m=QpOqQYfTzY_Gbj9_8jPtsplp1pnVUKDr

NOTE: Please use \*6 to mute/un-mute your phone during the call.

World Time Zone Converter:
http://www.thetimezoneconverter.com/?t=9:00%20am&tz=San%20Francisco&

## 会议记录

The minutes from our calls are available [here](https://docs.google.com/document/d/1OVF68rpuPK5shIHILK9JOqlZBbfe91RNzQ7u_P7YCDE/edit#).

Recording from our calls are available [here](https://www.youtube.com/playlist?list=PLj6h78yzYM2Ph7YoBIgsZNW_RGJvNlFOt).

Periodically, the group may have in-person meetings that coincide with a major
conference. Please see the [meeting minutes](https://docs.google.com/document/d/1OVF68rpuPK5shIHILK9JOqlZBbfe91RNzQ7u_P7YCDE/edit#)
for any future plans.
