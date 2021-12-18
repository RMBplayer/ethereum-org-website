---
title: dapp 介绍
description:
lang: zh
sidebar: true
---

去中心化应用（dapp）是构建在去中心化网络上的应用程序，它结合了[智能合约](/developers/docs/smart-contracts/)和前端用户界面。 请注意，以太坊智能合约具有可访问性和透明性——就像开放 API 一样 ——所以你的 dapp 里甚至可以包含其他人写过的智能合约。

## 基本要求 {#prerequisites}

在学习 dapp 之前，您应该了解[区块链基础知识](/developers/docs/intro-to-ethereum/)，并了解以太坊网络及其去中心化方式。

## dapp 的定义 {#definition-of-a-dapp}

一个 dapp 的后端代码在一个去中心化 P2P 网络上运行。 这与后端代码运行在集中式服务器上的传统应用程序形成鲜明对比。。

dapp 可以用任何语言编写（就像是一个 app）。它有前端代码和用户界面，能调用其后端。 此外，它的前端可以托管在去中心化存储上，例如 [IPFS](https://ipfs.io/)。

- **去中心化** ，dapps在以太坊上运行，这是一个开放的公共去中心化平台，没有任何一个人或团体可以控制。
- **确定性** ，无论在什么环境下执行，dapps都执行相同的功能。
- **图灵完备**，在所需资源满足的情况下，dapp可以执行任何行动
- **隔离性**，dapps在被称为Ethereum虚拟机的虚拟环境中执行，因此，如果智能合约有一个bug，也不会妨碍区块链网络的正常运行。
关于智能合约

### 智能合约 {#on-smart-contracts}

为了介绍dapp，我们需要介绍智能合约--一个dapp的后台，因为缺乏一个更好的术语。要了解详细的概述，请前往我们的智能合约部分。[智能合约](/developers/docs/smart-contracts/)部分。

智能合约是部署在以太坊区块链上的代码，完全按照程序运行。一旦智能合约被部署在网络上，你就不能改变它们。Dapps可以是去中心化的，正因为它们是由写入的智能合约基础逻辑控制的，而不是由个人或公司控制。这也意味着你需要非常仔细地设计你的智能合约，并对它们进行彻底的测试。

<!--Benefits and implications provided by Brian Gu)-->

## Dapp 开发的好处 {#benefits-of-dapp-development}

- **零关机** – 一旦将某 dapp 的智能合约部署在区块链上后，整个网络都能为那些希望与合约交互的用户提供服务。 因此，恶意行为者无法针对单个 dapp 发起 DoS 攻击。
- **隐私** – 您不需要提供真实身份部署或与 dapp 进行交互。
- **抵制审查** – 网络上没有任何一个实体可以阻止用户提交交易、部署 dapp 或读取区块链上的数据。
- **数据完整性** – 由于密码学原理，存储在区块链上的数据是不可改变和无可争议的。恶意行为者无法伪造交易或其他已经公开的数据。
- **无需信任关系的计算/可验证的行为** – 智能合约可以被分析，并保证以可预测的方式执行，而不需要信任一个中央机构。这在传统模式中是不存在的；例如，当我们使用网上银行系统时，我们必须相信金融机构不会滥用我们的财务数据，篡改记录，或被黑客攻击。

dapp开发的弊端

## Dapp 开发的弊端（这也是目前以太坊面临的问题） {#implications-of-dapp-development}

<!-- - Transparency – transactions that trigger dapp functionality are public
- Open source
- Cost of storage – contracts are often only small percentages of the dapp. They are stored on-chain and this storage needs to be paid for, so it can be expensive.
 -->

- **维护** – Dapps可能更难维护，因为发布到区块链上的代码和数据更难修改。开发者很难在他们的dapp（或dapp存储的底层数据）部署后进行更新--即使在旧版本中发现了bug或安全风险。
- **性能开销** – 有巨大的性能开销，而且扩展起来真的很困难。为了达到以太坊所追求的安全性、完整性、透明度和可靠性水平，每个节点都要运行和存储每笔交易。在此基础上，工作证明也需要时间。通过计算，开销是目前标准计算的一百万倍。
- **网络拥堵** – 当一个应用程序使用了太多的计算资源时，整个网络就会受到影响。目前，网络每秒只能处理大约10-15个交易；如果交易的发送速度超过这个速度，未确认的交易池会迅速膨胀。
- **用户体验** – 可能更难设计出用户友好的体验，因为普通的最终用户可能会发现，要建立一个必要的工具栈，以真正安全的方式与区块链交互，这太困难了。（当你发现以太坊用户体验变好的时候，意味着他将走入到大众的视野当中，所以现在也是机会）
- **中心化** – 建立在以太坊基础之上的用户友好型和开发者友好型解决方案最终可能看起来像互联网的应用。例如，这种服务可能在服务器端存储密钥或其他敏感信息，使用集中式服务器为前端服务，或在写入区块链之前在集中式服务器上运行重要的业务逻辑。集中化消除了区块链相对于传统模式的许多（如果不是全部）优势。（比如opensea）

---
 -->

## More of a visual learner? {#visual-learner}

<figure>
  <iframe width="100%" height="315" src="https://www.youtube.com/embed/F50OrwV6Uk8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</figure>

-->## Dapp 工具 {#dapp-tools}

**Scaffold-ETH - 使用一个适应你的智能合约的前端，快速试验Solidity。**

- [GitHub](https://github.com/austintgriffith/scaffold-eth)
- [Example dapp](https://punkwallet.io/)

**创建Eth应用程序 - 用一个命令创建由Ethereum驱动的应用程序。**

- [GitHub](https://github.com/paulrberg/create-eth-app)

**一键式Dapp - 用于从ABI生成Dapp前端的FOSS工具。(/glossary/#abi)._**

- [oneclickdapp.com](https://oneclickdapp.com)
- [GitHub](https://github.com/One-Click-Dapp/one-click-dApp)

**Etherflow** **_- FOSS 工具，供以太坊开发者测试他们的节点，并编写以及从浏览器调试 RPC 调用。_**

- [etherflow.quiknode.io](https://etherflow.quiknode.io/)
- [GitHub](https://github.com/abunsen/etherflow)

## 延伸阅读 {#further-reading}

- [The Architecture of a Web 3.0 application/Web 3.0应用程序的架构](https://www.preethikasireddy.com/post/the-architecture-of-a-web-3-0-application) - _Preethi Kasireddy_
- [A 2021 guide to decentralized applications/2021年去中心化应用的指南](https://limechain.tech/blog/what-are-dapps-the-2021-guide/) - _LimeChain_
- [What Are Decentralized Apps?/什么是去中心化的应用程序？](https://www.gemini.com/cryptopedia/decentralized-applications-defi-dapps) - _Gemini_

__知道有什么社区资源对你有帮助吗？编辑这个页面并添加它！_

_你知道有什么社区资源帮助过你吗？ 编辑并添加本页面！_

## 相关主题 {#related-topics}

- [以太坊技术栈简介](/developers/docs/ethereum-stack/)
- [开发框架](/developers/docs/frameworks/)
