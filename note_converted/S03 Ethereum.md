# S03 Ethereum

---

## 1. 课程背景与目标
文档探讨了以太坊（Ethereum）作为可编程区块链（Programmable Blockchain）的技术原理、商业潜力及其与比特币（Bitcoin）的对比，分析其在去中心化应用（DApps）和智能合约（Smart Contracts）中的作用。课程目标是帮助学生理解以太坊如何通过图灵完备（Turing Complete）的编程能力扩展区块链应用，并探讨其扩展性解决方案（如分片和Layer 2）及挑战。

- **关键词**：Ethereum（以太坊）、Programmable Blockchain（可编程区块链）、Smart Contracts（智能合约）、Turing Complete（图灵完备）
- **解释**：以太坊像一个全球计算机，允许开发者编写程序（智能合约）在区块链上运行，自动执行合同条款。
- **示例**：Alice用以太坊智能合约创建自动支付租金的程序，每月自动从她的账户转账给房东。

---

## 2. 比特币的扩展：彩色币与序数理论

### 2.1 彩色币（Colored Coins）
彩色币（Colored Coins）是比特币的扩展协议，旨在赋予特定比特币额外属性，使其代表资产或权证，称为“Bitcoin 2.0”。

- **概念**：通过标记（“染色”）部分比特币，使其代表特定资产（如房产、股票）。
- **比特币单位**：
  - 1 BTC = 100 centi-BTC (cBTC)
  - 1 BTC = 10^8 satoshi (sat)
  - 闪电网络（Lightning Network）最小单位：1 BTC = 10^11 milli-satoshi (msat)
- **白皮书**：由Yoni Assia、Vitalik Buterin等人撰写，提出比特币2.X（Bitcoin 2.X），即彩色币的初始规范。
- **Mastercoin**：早期尝试将比特币扩展为更复杂区块链平台，称为“第二比特币”（The Second Bitcoin）。
- **关键词**：Colored Coins（彩色币）、Bitcoin 2.0、Mastercoin、Satoshi（聪）、Milli-satoshi（毫聪）
- **解释**：彩色币像给普通钞票贴上标签，标明它代表一辆车的所有权。
- **示例**：Alice用1个彩色比特币代表她的房产所有权，转移这1比特币即转移房产。

### 2.2 序数理论（Ordinal Theory）
序数理论（Ordinal Theory）由Casey Rodarmor提出，通过为每个聪（satoshi）分配唯一编号（Ordinal Number），实现比特币的非同质化（Non-fungible）特性，类似NFT（非同质化代币）。

- **概念**：
  - 每个比特币包含10^8聪，每个聪可编号，编号由两部分组成：
    - **整数部分**：生成聪的区块高度（Block Height）。
    - **小数部分**：该区块内聪的偏移量（Offset）。
  - **编号方式**：
    - **十进制（Decimal Notation）**：如3891094.16797（区块高度.偏移量）。
    - **度数表示（Degree Notation）**：如3°111094′214″16797‴，表示周期、区块、交易等层级。
    - **百分位表示（Percentile Notation）**：如99.999719490602545%，表示聪在比特币总供应中的位置。
  - **稀有性分类**：
    - **Common（普通）**：非首聪的普通聪。
    - **Uncommon（不常见）**：每个区块的首个聪。
    - **Rare（稀有）**：每个难度调整（Difficulty Adjustment）的首个聪。
    - **Epic（史诗）**：每次减半（Halving）的首个聪。
    - **Legendary（传奇）**：每个周期（Cycle）的首个聪。
    - **Mythic（神话）**：创世区块（Genesis Block）的首个聪。
  - **周期（Cycle）**：减半（每210,000区块）和难度调整（每2,016区块）同时发生的时间点，称为“Conjunction”（交汇）。计算：
    - 210,000 ÷ 2,016 = 13125/126 ≈ 104.1667，整数解为H=6（第6次减半，约24年后）。
- **实现**：
  - **SegWit（隔离见证）**：增加区块容量，支持更多数据。
  - **Taproot（Taproot升级）**：支持存储元数据（Meta-data），用于铭文（Inscription）。
  - 铭文（Inscription）：将数据（如图像）嵌入聪，创建类似NFT的资产。
- **交易模型**：采用先进先出（First-In, First-Out, FIFO），需谨慎处理交易以保留特定聪。
- **关键词**：Ordinal Theory（序数理论）、Ordinal Number（序数编号）、Inscription（铭文）、Non-fungible（非同质化）、SegWit（隔离见证）、Taproot（Taproot升级）、Difficulty Adjustment（难度调整）、Halving（减半）、Cycle（周期）、Conjunction（交汇）
- **解释**：序数理论像给每个聪贴上身份证号，使其独一无二，可代表艺术品等独特资产。
- **示例**：Bob用编号#110000.000000001的聪存储一幅数字画作，作为NFT出售。

---

## 3. 以太坊概述

### 3.1 以太坊简介
以太坊由Vitalik Buterin于2013年提出，2015年上线，是一个支持智能合约的去中心化平台，基于区块链技术（Blockchain Technology）。

- **特点**：
  - **Programmable Blockchain（可编程区块链）**：支持图灵完备（Turing Complete）的编程语言（如Solidity），允许开发者创建复杂应用。
  - **Smart Contracts（智能合约）**：自动执行的程序，运行在以太坊虚拟机（EVM）上。
  - **Consensus Mechanism（共识机制）**：2022年“合并”（The Merge）前使用工作量证明（Proof-of-Work, PoW），之后转为权益证明（Proof-of-Stake, PoS）。
- **关键词**：Ethereum（以太坊）、Smart Contracts（智能合约）、Turing Complete（图灵完备）、EVM（以太坊虚拟机）、The Merge（合并）、Proof-of-Stake (PoS)（权益证明）
- **解释**：以太坊像一个全球共享的计算机，任何人都可以上传程序并运行。
- **示例**：公司用以太坊智能合约自动支付员工工资，无需人工干预。

### 3.2 与比特币的对比
- **相似性**：
  - 两者均为去中心化区块链（Decentralized Blockchain），使用公钥/私钥对（Public/Private Key Pairs）管理账户。
  - 都基于P2P网络（Peer-to-Peer Network），通过共识算法（Consensus Algorithm）维护账本。
- **差异**：
  - **编程能力**：以太坊支持智能合约，比特币仅限简单脚本（非图灵完备）。
  - **共识机制**：比特币始终使用PoW，以太坊转为PoS。
  - **用途**：比特币主要作为数字货币（Medium of Exchange）和价值储存（Store of Value），以太坊支持DApps和NFT等。
- **关键词**：Decentralized Blockchain（去中心化区块链）、Consensus Algorithm（共识算法）、Medium of Exchange（交换媒介）、Store of Value（价值储存）
- **解释**：比特币像数字黄金，以太坊像数字操作系统。
- **示例**：比特币用于跨境汇款，以太坊用于创建去中心化交易所。

### 3.3 EOAs vs CAs

- **EOAs（Externally Owned Accounts，外部拥有账户）**

  - **定义**：由用户通过私钥控制的账户，代表以太坊网络中的个人或实体。

    **创建**：通过生成一对公钥和私钥，公钥派生出地址（160 位哈希，0x 开头）。

    **控制**：私钥持有者通过签名交易控制账户。

    **功能**：

    - 发送交易（转账 ETH、调用智能合约）。
    - 持有 ETH 和 ERC-20 代币。
    - 支付 Gas 费用（页面65：Gas 限额问题）。

- **CAs（Contract Accounts，合约账户）**

  - **定义**：由智能合约代码控制的账户，存储在以太坊区块链上，执行预定义逻辑。

    **创建**：通过 EOA 部署智能合约（包含字节码），生成合约地址。

    **控制**：由智能合约代码逻辑控制，无私钥，需通过 EOA 或其他 CA 调用。

    **功能**：

    - 执行智能合约逻辑（如 DeFi、NFT、DAO）。
    - 持有 ETH 和代币。
    - 自动响应交易或事件。

  ### 3.4. Merkle Patricia Trie

  <img src="/Users/sh4nglj/Documents/MS DTTI/SEM B/IS6200 Blockchain/Final Review/note_converted/pictures/S03 MPT.png" alt="S03 MPT" style="zoom:40%;" />

---

## 4. 以太坊的共识机制：权益证明（PoS）

### 4.1 PoS简介
以太坊于2022年通过“合并”（The Merge）从PoW转为PoS，验证者（Validator）通过质押ETH（Stake）参与区块创建。

- **机制**：验证者质押至少32 ETH，随机被选中创建区块，获得交易费（Gas Fees）和区块奖励（Block Reward）。
- **优势**：
  - 能耗低：PoW需大量计算，PoS仅需质押。
  - 环保：减少碳足迹。
- **关键词**：Proof-of-Stake (PoS)（权益证明）、The Merge（合并）、Validator（验证者）、Stake（质押）、Gas Fees
- **解释**：PoS像股东投票，持有更多ETH的人有更大机会记账。
- **示例**：Alice质押32 ETH，成为验证者，验证交易后获得0.1 ETH奖励。

### 4.2 PoS的问题：无利害关系（Nothing at Stake）
PoS存在“无利害关系”问题：验证者可能在多个分支（Fork）上同时验证区块，增加双重支付（Double-spending）风险。

- **解决方案**：
  - **Slashing（惩罚机制）**：检测到恶意行为（如双重投票）时，销毁验证者的部分ETH，并可能禁止其继续质押。
  - **Finality（终局性）**：
    - **概率终局性（Probabilistic Finality）**：PoW中，区块确认数越多，篡改难度越大。
    - **加密经济终局性（Cryptoeconomic Finality）**：PoS通过经济激励确保区块不可逆。
- **关键词**：Nothing at Stake（无利害关系）、Slashing（惩罚机制）、Finality（终局性）、Double-spending（双重支付）
- **解释**：无利害关系像作弊者同时支持两支队伍，惩罚机制像没收其赌注。
- **示例**：Bob尝试在两个分支上验证区块，被系统检测到，损失10 ETH。

### 4.3 PoS攻击场景
- **攻击1：33%攻击**：
  - 若攻击者控制33%质押ETH，可能通过不活跃（Inactive）或双重投票（Double Voting）干扰共识。
  - **解决方案**：增加活跃验证者比例，设置更严格的惩罚。
- **攻击2：51%攻击**：
  - 控制51%质押ETH可完全控制网络，但成本极高（需购买大量ETH）。
- **关键词**：33% Attack（33%攻击）、51% Attack（51%攻击）、Double Voting（双重投票）
- **解释**：33%攻击像少数股东捣乱，51%攻击像控股股东操纵公司。
- **示例**：攻击者控制33% ETH，拒绝验证新区块，网络暂停，直到惩罚机制生效。

---

## 5. 以太坊的扩展性解决方案

### 5.1 扩展性问题与区块链三难困境
以太坊面临扩展性问题：需在去中心化（Decentralization）、安全性（Security）和可扩展性（Scalability）之间平衡，称为**区块链三难困境（Blockchain Trilemma）**。

- **问题**：高交易量导致网络拥堵，交易费用（Gas Fees）飙升。
- **关键词**：Blockchain Trilemma（区块链三难困境）、Decentralization（去中心化）、Security（安全性）、Scalability（可扩展性）
- **解释**：三难困境像做饭时只能选择快、好、省其二，无法三者兼得。
- **示例**：以太坊在2021年NFT热潮中，单笔交易费用高达100美元。

### 5.2 Layer 1扩展：链上解决方案
- **The Merge（合并）**：从PoW转为PoS，降低能耗，为后续扩展奠定基础。
- **Sharding（分片）**：
  - 将区块链数据库分成多个分片（Shards），每个分片处理部分交易，提高吞吐量（Throughput）。
  - **Proto-Danksharding**：初步分片方案，优化数据存储，降低Layer 2成本。
- **关键词**：Sharding（分片）、Proto-Danksharding（原型分片）、Throughput（吞吐量）
- **解释**：分片像把大图书馆分成多个小书库，读者可同时借阅不同书籍。
- **示例**：以太坊分片后，Alice的NFT交易和Bob的支付交易在不同分片处理，互不干扰。

### 5.3 Layer 2扩展：链下解决方案
Layer 2在主链（Layer 1）外处理交易，减轻主链负担，分为以下类型：

#### 5.3.1 Rollups
Rollups将交易在链下执行，数据压缩后提交到主链。

- **类型**：
  - **Optimistic Rollups（乐观Rollups）**：假设链下交易有效，设置挑战期（Challenge Period）允许争议（Dispute）。如Arbitrum。
  - **ZK-Rollups（零知识Rollups）**：使用零知识证明（Zero-Knowledge Proof）验证交易，效率更高但计算复杂。
- **优势**：
  - 降低交易费用（Gas Fees）。
  - 提高交易速度。
  - 保留主链安全性。
- **缺点**：
  - 挑战期可能延迟资金提取。
  - 复杂性增加开发难度。
- **与闪电网络对比**：
  - **相似性**：两者均为Layer 2，减轻主链负担。
  - **差异**：闪电网络基于支付通道（Payment Channel），适合小额支付；Rollups支持复杂智能合约。
- **关键词**：Rollups（Rollups）、Optimistic Rollups（乐观Rollups）、ZK-Rollups（零知识Rollups）、Challenge Period（挑战期）、Arbitrum
- **解释**：Rollups像把大量交易打包成一个小包裹，只记录包裹信息到主链。
- **示例**：Alice通过Arbitrum以低费用交易NFT，仅需主链验证最终结果。

#### 5.3.2 Sidechains（侧链）
侧链是与以太坊并行的独立区块链，通过桥（Bridge）与主链交互。

- **特点**：
  - 更快区块时间（Block Time）和更大区块大小（Block Size），提高吞吐量。
  - **Polygon PoS**：以太坊的PoS侧链，平均区块时间约2秒。
- **缺点**：
  - 安全性降低：不完全依赖主链。
  - 去中心化减少：可能出现超级节点（Super Nodes）。
- **关键词**：Sidechains（侧链）、Polygon PoS（Polygon PoS侧链）、Block Time（区块时间）、Super Nodes（超级节点）
- **解释**：侧链像主路的辅路，速度快但安全性稍差。
- **示例**：Bob在Polygon侧链上快速交易游戏代币，费用仅为主链的1/10。

---

## 6. 智能合约与安全问题

### 6.1 智能合约特点
- **不可修改**：部署后代码不可更改，除非使用代理合约（Proxy Contract）。
- **需存储**：全节点（Full Node）需存储所有智能合约代码。
- **Gas限制**：运行需支付Gas，Gas不足交易失败但Gas不退还。
- **关键词**：Proxy Contract（代理合约）、Full Node（全节点）、Gas Fees（ガス费）
- **解释**：智能合约像自动售货机，按预设规则运行，无法中途更改。
- **示例**：Alice的智能合约因Gas不足未执行，损失0.01 ETH。

### 6.2 安全漏洞
- **重入攻击（Reentrancy Attack）**：合约在完成支付前被重复调用，导致资金被盗。
  - **示例**：2016年DAO攻击，攻击者通过重入漏洞窃取360万ETH。
- **存储碰撞（Storage Collision）**：
  - 代理合约与实现合约的存储布局冲突，导致数据错误。
  - **示例**：2022年Aulius治理攻击，因存储碰撞导致治理机制被操控。
- **无限循环**：错误代码可能导致区块链卡死，但Gas限制可防止此问题。
- **关键词**：Reentrancy Attack（重入攻击）、Storage Collision（存储碰撞）
- **解释**：重入攻击像小偷在ATM吐钞前多次按取款键，存储碰撞像两本书用同一书架编号。
- **示例**：攻击者利用重入漏洞从Alice的合约偷走10 ETH。

---

## 7. 以太坊与去中心化互联网

### 7.1 互联网的中心化问题
文档引用Leopold Kohr：“Whenever something is wrong, something is too big.”（当事情出错时，往往是因为某物过于庞大。）当前互联网高度中心化（Centralized），由少数科技巨头控制。

- **示例**：Twitter（现为X）由单一公司运营，控制用户数据和内容审核。
- **关键词**：Centralized（中心化）
- **解释**：中心化像所有数据存在一家公司服务器，容易被控制或泄露。
- **示例**：Twitter 2022年政策变更，限制用户分享他人实时位置。

### 7.2 Tor与去中心化
**Tor（The Onion Routing Project）**通过多层加密（Onion Routing）保护隐私，但并非完全去中心化，依赖有限的中继节点（Relay Nodes）。

- **问题**：中继节点可能成为瓶颈，降低去中心化程度。
- **关键词**：Tor（洋葱路由）、Onion Routing（洋葱路由）、Relay Nodes（中继节点）
- **解释**：Tor像通过多个邮局转发信件隐藏寄件人，但邮局数量有限。
- **示例**：Alice用Tor访问网站，数据经多个中继加密传输，保护隐私。

### 7.3 以太坊的去中心化潜力
以太坊通过DApps提供去中心化替代方案，如去中心化社交媒体（Decentralized Social Media）。

- **示例**：Lens Protocol，基于以太坊的去中心化社交平台，用户控制数据。
- **关键词**：Decentralized Social Media（去中心化社交媒体）
- **解释**：去中心化社交像用户自己存储帖子，无需依赖平台。
- **示例**：Bob在Lens上发布内容，数据存储在以太坊，平台无法删除。

---

## 8. 快速问答（Quick Q&As）
以下为文档中的问题及答案，补充解释：

1. **以太坊可编程，比特币不可？** 是（Yes）
   - 以太坊支持Solidity，比特币仅支持简单脚本。
2. **以太坊因PoS而公开销售？** 否（No）
   - 以太坊通过ICO（Initial Coin Offering）筹资，2015年上线时使用PoW。
3. **比特币和以太坊从未被成功攻击？** 否（No）
   - 以太坊曾遭DAO攻击，比特币网络未被直接攻击但交易所常被黑。
4. **以太坊创建地址免费？** 是（Yes）
   - 类似比特币，生成地址无需费用。
5. **全节点需存储所有智能合约代码？** 是（Yes）
   - 全节点需同步整个区块链，包括合约代码。
6. **错误智能合约（如无限循环）会导致网络失败？** 否（No）
   - Gas限制防止无限循环。
7. **智能合约部署后可修改？** 否（No）
   - 除非使用代理合约。
8. **Gas不足交易失败，Gas会退还？** 否（No）
   - Gas用于支付已执行计算，不退还。
9. **Rollups将所有交易细节存储在主链？** 是（Yes）
   - Rollups将压缩数据提交主链，确保透明。
10. **重入攻击违法？** 否（No）
    - 技术漏洞利用不一定违法，但可能违反道德。
11. **以太坊分叉为以太坊经典因PoS？** 否（No）
    - 分叉因2016年DAO攻击，经典版反对回滚。
12. **攻击以太坊需51%质押？** 否（No）
    - 33%质押即可干扰共识。

- **解释**：这些问题测试对以太坊机制的理解，如Gas、PoS和安全漏洞。
- **示例**：Alice因Gas不足交易失败，损失0.01 ETH但网络未受影响。

---

## 9. 总结与关键词
以太坊通过智能合约和图灵完备性扩展了区块链应用，PoS提高能效，Layer 1（分片）和Layer 2（Rollups、侧链）解决扩展性问题。然而，智能合约漏洞和PoS的潜在攻击（如33%攻击）需警惕。彩色币和序数理论展示了比特币的扩展潜力，但以太坊在可编程性和DApps方面更具优势。

**重点英文词汇**：
- Ethereum（以太坊）
- Programmable Blockchain（可编程区块链）
- Smart Contracts（智能合约）
- Turing Complete（图灵完备）
- EVM（以太坊虚拟机）
- The Merge（合并）
- Proof-of-Stake (PoS)（权益证明）
- Colored Coins（彩色币）
- Bitcoin 2.0
- Mastercoin
- Satoshi（聪）
- Milli-satoshi（毫聪）
- Ordinal Theory（序数理论）
- Ordinal Number（序数编号）
- Inscription（铭文）
- Non-fungible（非同质化）
- SegWit（隔离见证）
- Taproot（Taproot升级）
- Difficulty Adjustment（难度调整）
- Halving（减半）
- Cycle（周期）
- Conjunction（交汇）
- Decentralized Blockchain（去中心化区块链）
- Consensus Algorithm（共识算法）
- Medium of Exchange（交换媒介）
- Store of Value（价值储存）
- Validator（验证者）
- Stake（质押）
- Gas Fees（ガス费）
- Nothing at Stake（无利害关系）
- Slashing（惩罚机制）
- Finality（终局性）
- Double-spending（双重支付）
- 33% Attack（33%攻击）
- 51% Attack（51%攻击）
- Double Voting（双重投票）
- Blockchain Trilemma（区块链三难困境）
- Decentralization（去中心化）
- Security（安全性）
- Scalability（可扩展性）
- Sharding（分片）
- Proto-Danksharding（原型分片）
- Throughput（吞吐量）
- Rollups（Rollups）
- Optimistic Rollups（乐观Rollups）
- ZK-Rollups（零知识Rollups）
- Challenge Period（挑战期）
- Arbitrum
- Sidechains（侧链）
- Polygon PoS（Polygon PoS侧链）
- Block Time（区块时间）
- Super Nodes（超级节点）
- Proxy Contract（代理合约）
- Full Node（全节点）
- Reentrancy Attack（重入攻击）
- Storage Collision（存储碰撞）
- Centralized（中心化）
- Tor（洋葱路由）
- Onion Routing（洋葱路由）
- Relay Nodes（中继节点）
- Decentralized Social Media（去中心化社交媒体）

---

## 10. 补充说明
- **课程背景**：香港城市大学的课程以“Professional · Creative · For The World”为理念，鼓励探索区块链技术。
- **进一步学习**：
  - 阅读以太坊白皮书（https://ethereum.org/en/whitepaper/）。
  - 访问https://ethereum.org/en/developers/docs/了解开发资源。
  - 体验Polygon侧链钱包（如MetaMask），尝试低费用交易。