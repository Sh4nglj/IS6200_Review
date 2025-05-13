# S04-1 DAO

## 一、传统组织中的代理问题 (Agency Problems in Traditional Organizations)

### 1.1 代理理论（Agency Theory）

Agency Theory examines the relationship between asset owners (principals) and those employed to manage these assets (agents). Due to misalignment of interests, agents may act against the principals' interests, leading to agency conflicts.

- **Definition**: Principals (such as shareholders) entrust their assets to agents (such as corporate executives) for management, but agents may pursue personal interests (such as high salaries or power), harming the principals' interests.
- **Example**: In the Luckin Coffee Scandal, executives falsified 2.2 billion RMB in sales data, exaggerated costs and expenses, ultimately resulting in the company paying $180 million in fines (document page 3). This demonstrates how agents can harm shareholder interests through fraudulent behavior.

### 1.2 四种代理成本（Four Types of Agency Costs）

1. **监控代理人（Monitoring Agents）**:
   - **Definition**: Principals need to spend resources to monitor agents to prevent self-serving behaviors. This includes audits, internal controls, etc.
   - **Case**: In the Enron Scandal (document page 7), CEO Jeff Skilling and former CEO Ken Lay deceived shareholders by hiding enormous debts, causing shareholders to lose $74 billion. Whistleblower Sherron Watkins exposed the problem, showing the consequences of insufficient monitoring.
   - **Explanation**: Monitoring costs are expensive because they require hiring auditors, establishing compliance systems, etc., but may still not completely prevent fraud.

2. **监控公司运营（Monitoring Firm Operations）**:
   - **Definition**: Principals need to obtain information about company operations to reduce information asymmetry. Information asymmetry means agents know more about the company than principals.
   - **Case**: Wells Fargo was fined $3 billion for opening millions of accounts without customer authorization (document page 8). Shareholders could not detect the problem in time due to lack of transparent information.
   - **Explanation**: Information asymmetry makes it difficult for shareholders to determine whether executive decisions are reasonable, increasing trust costs.

3. **过度开支（Excessive Expenses）**:
   - **Definition**: Agents may waste resources through high managerial perks or excessive executive compensation.
   - **Case**: Former WeWork CEO Adam Neumann was accused of treating employees improperly and squandering company funds (document page 9). For example, he used company funds to purchase a private jet, harming shareholder interests.
   - **Explanation**: Excessive expenses directly reduce company profits, lowering shareholder returns.

4. **未实现利润（Unrealized Profits）**:
   - **Definition**: The company misses profit opportunities due to suboptimal executive decisions by agents.
   - **Case**: Yahoo!'s multiple wrong decisions (document page 10), such as refusing to acquire Google for $1 million in 1998, rejecting Microsoft's $44.6 billion acquisition offer in 2008, and finally being acquired by Verizon for $5 billion in 2016. These decisions led to enormous value loss.
   - **Explanation**: Executive decision failures may stem from lack of ability or personal interest-driven motives, damaging the company's long-term value.

## 二、DAO的定义与优势

### 2.1 DAO的定义 (Definition of DAO)

A DAO is an organization that operates through blockchain technology, characterized by being decentralized and autonomous. It uses smart contracts to automatically execute rules, reducing dependence on traditional managers.

- **Definition**: A DAO is a blockchain-based organizational form where all rules and transaction records are stored on the blockchain, automatically executed through code, and members participate in decision-making through voting.
- **Example**: Uniswap is a DAO that allows users holding UNI tokens to vote on protocol upgrades and fund allocations (document pages 17-20).
- **Supplementary**: The "decentralization" of DAOs means there is no single controlling entity, with decisions made collectively by the community; "autonomy" means rules are automatically executed by code without human intervention.

### 2.2 DAO如何缓解代理问题 (How DAOs Mitigate Agency Problems)

DAOs reduce the agency costs of traditional organizations in the following ways (document pages 6, 11-12):

1. **减少对代理人的依赖 (Reducing Dependence on Agents)**:
   - DAOs transfer decision rights to investor-owners through smart contracts, reducing dependence on fund managers. For example, investment DAOs allow members to directly vote on fund usage, preventing managers from misappropriating funds.
   - **Example**: In traditional funds, managers might invest in low-return projects to receive kickbacks; in DAOs, investment decisions require community voting approval, increasing transparency.

2. **提高信息透明度 (Improving Information Availability)**:
   - The blockchain's public ledger records all transactions and decisions, reducing information asymmetry. Members can view fund flows and operational status in real-time.
   - **Example**: Uniswap's governance proposals (such as the "Uniswap Delegate Reward") are publicly available on-chain, and all UNI token holders can view and vote (document page 18).
   - **Explanation**: Transparency reduces agents' ability to hide information, making it easier for principals to monitor.

3. **新型治理结构 (Novel Governance Structure)**:
   - DAOs define governance rules through smart contracts, giving principals more choices and reducing dependence on agents. For example, members can directly propose and vote without going through executives.
   - **Supplementary**: Governance structures include the allocation of decision rights, incentive mechanisms, and accountability systems; DAOs ensure fair execution of these mechanisms through code.

## 三、DAO的治理机制 (Governance Mechanisms of DAOs)

### 3.1 治理的定义 (Definition of Governance)

- **Definition**: Governance is the means by which organizations coordinate decision rights, incentives, and accountability (document page 11). In DAOs, governance is achieved through blockchain and smart contracts, ensuring decisions are transparent and automated.
- **Example**: Uniswap's governance process includes proposal discussion (Governance Forum), preliminary voting (Snapshot), and formal on-chain voting (Governance Portal), ensuring community participation (document page 17).

### 3.2 治理的三个核心要素 (Three Core Elements of Governance)

1. **决策权 (Decision Rights)**:
   - **Definition**: Decision rights determine who has the authority to make key decisions. In DAOs, decision rights are typically decentralized, determined collectively by token holders.
   - **Example**: In Uniswap, users holding UNI tokens can vote on protocol upgrades, replacing the traditional model where CEOs make decisions.
   - **Supplementary**: The degree of decentralization of decision rights varies by DAO; some DAOs may still have core teams retaining partial control.

2. **问责制 (Accountability)**:
   - **Definition**: Accountability requires decision-makers to be responsible for the consequences of their actions. Blockchain transparency makes all actions traceable, enhancing accountability.
   - **Example**: Bitcoin's SegWit upgrade (document page 14) was implemented through community consensus, with all proposals and discussions public, making developers accountable to the community.
   - **Explanation**: Accountability ensures decision-makers cannot arbitrarily change rules or hide errors.

3. **激励 (Incentives)**:
   - **Definition**: Incentive mechanisms align the interests of principals and agents through rewards. DAOs incentivize members to participate in governance through token rewards.
   - **Example**: Uniswap's "Delegate Reward" proposal suggests rewarding delegates who actively participate in governance, encouraging more users to vote (document page 18).
   - **Supplementary**: Incentive alignment is key to resolving agency conflicts; DAOs achieve this goal through token economics.

## 四、链上与链下治理 (On-Chain and Off-Chain Governance)

### 4.1 链上治理 (On-Chain Governance)

On-chain governance refers to all governance activities (such as proposals and voting) being executed directly on the blockchain, with immutable records.

- **Definition**: On-chain governance automatically executes voting and decision-making through smart contracts, with results directly recorded on-chain.
- **Example**: Uniswap's final voting stage occurs on the blockchain, requiring a quorum of 40M UNI (document page 20).
- **Advantages**: Transparent, immutable, automated.
- **Disadvantages**: On-chain transactions require Gas fees, potentially limiting participation; high transparency may leak sensitive information.

### 4.2 链下治理 (Off-Chain Governance)

Off-chain governance refers to governance activities taking place outside the blockchain, such as forum discussions or Snapshot voting, with results potentially executed on-chain.

- **Definition**: Off-chain governance collects opinions through external platforms (such as forums or voting tools), reducing costs and complexity.
- **Examples**:
  - **Bitcoin's BIP Process** (document pages 14-15): Bitcoin Improvement Proposals (BIPs) are submitted and discussed via GitHub, with final implementation decided by miner and node consensus. For example, SegWit (Segregated Witness) was proposed through BIP 141, discussed in 2015, and activated in 2017.
  - **Snapshot** (document page 16): Snapshot is an off-chain voting interface where users connect their wallets to verify votes without on-chain transactions. Gnosis DAO uses Snapshot to configure voting rules, such as voting rights based on token holdings.
- **Supplementary**: SegWit is a protocol that optimizes Bitcoin transactions by separating signature data from transaction data, increasing block capacity. Snapshot links voting spaces through the Ethereum Name System (ENS), reducing Gas fees.
- **Advantages**: Low cost, flexible, suitable for preliminary discussions.
- **Disadvantages**: Results may be manipulated, less transparent than on-chain governance.

### 4.3 案例：Uniswap的治理流程

1. **请求评论 (Request for Comment, RFC)**:
   - Initial ideas are proposed in the Governance Forum, with 7 days of community discussion, considered off-chain governance.
   - Example: The "Uniswap Delegate Reward" proposal was initiated by Doo_StableLab, discussing reward mechanisms.

2. **温度检查 (Temperature Check)**:
   - Uses Snapshot for a 5-day off-chain vote, requiring a 10M UNI quorum, testing proposal feasibility.

3. **治理提案 (Governance Proposal)**:
   - After proposal iteration, it enters on-chain voting, requiring 2.5M UNI delegated support, a 40M UNI quorum, with a 7-day voting period.
   - Approved proposals have a 2-day timelock, ensuring review before execution.

- **Explanation**: Uniswap's hybrid governance balances efficiency and transparency, with off-chain discussions reducing costs and on-chain voting ensuring fairness.

## 五、DAO中的投票机制 (Voting Mechanisms in DAOs)

### 5.1 投票的重要性 (Importance of Voting)

Voting is the core of DAO governance, determining whether proposals pass. The document compares DAO voting with real-world voting (such as Hong Kong elections) (document page 21).

- **Real-world Voting**: Hong Kong elections require voters to show ID cards or specified documents (such as passports) to receive ballots, emphasizing identity verification.
- **DAO Voting**: Users verify their identity through crypto wallets, with voting rights typically tied to token holdings, without requiring traditional documentation.

### 5.2 投票类型 (Types of Voting)

The document introduces several types of voting in DAOs (document pages 22-23):

1. **单一投票 (Single Voting)**:
   - Each voter chooses one option, similar to the "one person, one vote" in traditional elections.
   - **Example**: PistachioDAO electing a governance leader, with voters choosing one person from Alice, Bob, Carol, and David.

2. **加权投票 (Weighted Voting)**:
   - Voting power is based on token holdings, with users holding more tokens having greater influence.
   - **Example**: In Uniswap's voting, users holding more UNI tokens have higher voting power.

3. **比例投票 (Proportional Voting)**:
   - Voters can allocate their voting weight across multiple options, similar to ranked-choice voting.
   - **Example**: PistachioDAO choosing a slogan, with voters allocating different weights to options like "In Pistachio we believe" and "In Pistachio Veritas."

4. **批准投票 (Approval Voting)**:
   - Voters can approve multiple options, ultimately selecting the option with the most approvals.
   - **Supplementary**: Approval voting is suitable for multi-candidate scenarios, reducing the "vote splitting" problem. For example, voters can simultaneously approve Alice and Bob as governance leaders.

- **Tools**: Snapshot supports various voting types, such as single, weighted, and proportional voting, commonly used in DAO off-chain governance.

## 七、DAO的挑战（新成本）

1. **技术复杂性 (Technical Complexity)**:
   - DAOs rely on blockchain and smart contracts, with high development and maintenance costs. Ordinary users may be unable to participate due to technical barriers.
   - **Example**: Uniswap's governance requires users to understand Snapshot and on-chain voting processes, potentially excluding members without technical backgrounds.

2. **治理效率低 (Low Governance Efficiency)**:
   - Decentralized decision-making requires multiple voting rounds, takes time, and may miss market opportunities.
   - **Example**: Uniswap proposals need to go through RFC, temperature check, and formal voting, taking several weeks.

3. **代币集中风险 (Token Concentration Risk)**:
   - Weighted voting may lead to a few large holders (Whales) controlling decisions, weakening decentralization.
   - **Example**: If a user holds a large amount of UNI tokens, they can unilaterally influence Uniswap governance.

4. **法律与监管 (Legal and Regulatory Issues)**:
   - The legal status of DAOs is unclear, potentially facing regulatory risks.
   - **Supplementary**: In 2023, the US SEC sued certain DAOs for unregistered securities offerings, highlighting regulatory challenges.
