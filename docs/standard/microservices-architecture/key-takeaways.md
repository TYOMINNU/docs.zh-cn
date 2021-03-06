---
title: "记住的要点"
description: "为容器化的.NET 应用程序的.NET 微服务体系结构 |记住的要点"
keywords: "Docker, 微服务, ASP.NET, 容器"
author: CESARDELATORRE
ms.author: wiwagn
ms.date: 05/26/2017
ms.prod: .net-core
ms.technology: dotnet-docker
ms.topic: article
ms.openlocfilehash: b557d0b641bfe95c025cadb13f82c3f8927f4bc8
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2017
---
# <a name="key-takeaways"></a>记住的要点

作为摘要，并记住的要点，以下是利用本指南的最重要的结论。

**使用容器的好处。** 容器基于解决方案提供成本节省的重要优势，因为容器是因为缺少生产环境中的依赖关系的部署问题的解决方案。 容器显著提高 DevOps 和生产操作。

**容器将无处不在。** 基于 docker 容器变得在容器行业中，支持的 Windows 和 Linux 生态系统中最重要供应商事实上的标准。 这包括 Microsoft、 Amazon AWS、 Google、 和 IBM。 在不久的将来，Docker 将可能无处不在云中和本地数据中心内。

**作为一个单元部署的容器。** Docker 容器变得越来越部署的任何基于服务器的应用程序或服务的标准单位。

**微服务。** 微服务体系结构已变得分布式和大型或复杂任务关键型应用程序基于自治服务形式的多个独立子系统的首选的方法。 在基于微服务的体系结构，该应用程序生成的服务可以是开发、 测试、 版本控制的部署，并且独立; 扩展的集合为这可能包括任何相关的自治数据库。

**域驱动的设计和 SOA。** 从面向服务的体系结构 (SOA) 和域驱动设计 (DDD) 派生的微服务体系结构模式。 当你在设计和开发不断变化的业务规则调整特定域的环境的微服务时，务必考虑到帐户 DDD 方法和模式。

**微服务挑战。** 微服务提供许多强大的功能，如部署独立于、 强子系统边界和技术多样性。 但是，它们也会引发许多如分片与分布式应用程序开发相关的新挑战和独立的数据模型、 弹性通信微服务、 最终一致性和操作的结果的复杂性之间聚合来自多个微服务的日志记录和监视信息。 这些方面引入比传统的整体应用程序的复杂性更高级别。 因此，仅特定方案都适用于基于微服务构成的应用程序。 其中包括多个不断发展子系统; 大型和复杂的应用程序在这些情况下，值得投资在更复杂的软件体系结构，因为它将提供更好地长期的灵活性和应用程序维护。

**任何应用程序的的容器。** 容器便于微服务，但不是会为它们排他。 此外可以与整体应用程序，包括基于传统的.NET Framework 和 Windows 容器通过得到改进的旧版应用程序使用容器。 使用 Docker，例如解决许多部署到生产问题并提供最先进的开发和测试环境的优点适用于许多不同类型的应用程序。

**与 IDE CLI。** 与 Microsoft 工具，你可以开发使用你首选的方法的容器化的.NET 应用程序。 你可以通过使用 Docker CLI 和 Visual Studio Code 开发使用 CLI 和基于编辑器的环境。 或者你可以使用专注于 IDE 的方法与 Visual Studio 和其独特的功能对 Docker，如能够调试多容器应用程序。

**弹性云应用程序。** 在基于云的系统和分布式的系统一般情况下，都始终部分的失败的风险。 由于客户端和服务都是单独的进程 （容器），服务可能无法及时方式与客户端的请求作出响应。 例如，服务出现部分的失败或进行维护; 可能已关闭该服务可能重载，响应速度极慢于请求;或它可能只是无法访问在短时间由于网络问题。 因此，基于云的应用程序必须接受这些故障，并且具有策略设置，以响应这些故障。 这些策略可以包括重试策略 （重新发送消息或重试请求） 和实现的断路器模式，以避免指数负载的重复请求。 基本上，基于云的应用程序必须具有弹性的机制-自定义违规时，或者是基于云的基础结构，例如从 orchestrators 或服务总线高级框架。

**安全。** 我们现代世界中的容器和微服务可以公开新的漏洞。 基本应用程序安全性取决于身份验证和授权;通过多种方法可实现这些。 但是，容器安全包括导致本质上是更安全的应用程序的其他关键组件。 生成更安全的应用的关键元素有个与其他应用程序和系统通信的安全方式，有些东西，它通常需要凭据、 令牌、 密码和其他类型的机密信息-通常被称为应用程序机密。 任何安全的解决方案必须遵循安全最佳做法，例如加密传输; 的过程中的机密加密对静止; 机密并阻止无意中泄露时使用的最终应用程序机密。 这些机密需要存储并保持安全的某处。 为了安全，可以充分利用你选的 orchestrator 的基础结构，或云基础结构，如 Azure 密钥保管库和它的应用程序代码，若要使用它提供了的方式。

**Orchestrators。** 容器基于 orchestrators 类似 Azure 容器服务 （Kubernetes、 Mesos DC/操作系统和 Docker Swarm） 和 Azure Service Fabric 中提供的是必不可少为任何生产就绪基于微服务构成的应用程序和任何多容器使用大大增加复杂性、 可伸缩性的需要和不断发展的应用程序。 本指南中引入了 orchestrators 和基于微服务和容器基于解决方案中的其角色。 如果您的应用程序需要在迁移你向复杂的容器化应用程序，您将发现非常有用找出用于详细了解 orchestrators 的其他资源

>[!div class="step-by-step"]
[以前](secure-net-microservices-web-applications/azure-key-vault-protects-secrets.md)
