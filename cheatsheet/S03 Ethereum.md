# S03 Ethereum

## 2. 比特币的扩展：彩色币与序数理论 (Bitcoin Extensions: Colored Coins and Ordinal Theory)

### 2.1 彩色币（Colored Coins）

Colored Coins are an extension protocol for Bitcoin, designed to give specific bitcoins additional properties, allowing them to represent assets or certificates, referred to as "Bitcoin 2.0."

- **Concept**: By marking ("coloring") portions of bitcoin, they can represent specific assets (such as real estate or stocks).
- **Bitcoin units**:
  - 1 BTC = 100 centi-BTC (cBTC)
  - 1 BTC = 10^8 satoshi (sat)
  - Lightning Network's smallest unit: 1 BTC = 10^11 milli-satoshi (msat)
- **White paper**: Written by Yoni Assia, Vitalik Buterin, and others, proposing Bitcoin 2.X, the initial specification for Colored Coins.
- **Mastercoin**: An early attempt to extend Bitcoin into a more complex blockchain platform, called "The Second Bitcoin."
- **Keywords**: Colored Coins, Bitcoin 2.0, Mastercoin, Satoshi, Milli-satoshi
- **Explanation**: Colored Coins are like attaching a label to ordinary banknotes, indicating they represent ownership of a car.
- **Example**: Alice uses 1 colored bitcoin to represent ownership of her property; transferring this 1 bitcoin transfers the property.

### 2.2 序数理论（Ordinal Theory）

Ordinal Theory, proposed by Casey Rodarmor, achieves Bitcoin's non-fungible characteristics by assigning unique numbering (Ordinal Number) to each satoshi, similar to NFTs (Non-Fungible Tokens).

- **Concept**:
  - Each bitcoin contains 10^8 satoshis, and each satoshi can be numbered with two components:
    - **Integer part**: The block height where the satoshi was generated.
    - **Decimal part**: The offset of the satoshi within that block.
  - **Numbering methods**:
    - **Decimal Notation**: Such as 3891094.16797 (block height.offset).
    - **Degree Notation**: Such as 3°111094′214″16797‴, representing cycle, block, transaction, and other hierarchical levels.
    - **Percentile Notation**: Such as 99.999719490602545%, indicating the satoshi's position in the total Bitcoin supply.
  - **Rarity classification**:
    - **Common**: Ordinary satoshis that are not the first in their category.
    - **Uncommon**: The first satoshi of each block.
    - **Rare**: The first satoshi of each difficulty adjustment.
    - **Epic**: The first satoshi of each halving.
    - **Legendary**: The first satoshi of each cycle.
    - **Mythic**: The first satoshi of the genesis block.
  - **Cycle**: When halving (every 210,000 blocks) and difficulty adjustment (every 2,016 blocks) occur simultaneously, called a "Conjunction." Calculation:
    - 210,000 ÷ 2,016 = 13125/126 ≈ 104.1667, integer solution is H=6 (the 6th halving, approximately 24 years later).
- **Implementation**:
  - **SegWit (Segregated Witness)**: Increases block capacity, supporting more data.
  - **Taproot**: Supports storing metadata, used for inscriptions.
  - **Inscription**: Embedding data (such as images) into satoshis, creating NFT-like assets.
- **Transaction model**: Uses First-In, First-Out (FIFO), requiring careful transaction handling to preserve specific satoshis.
- **Keywords**: Ordinal Theory, Ordinal Number, Inscription, Non-fungible, SegWit, Taproot, Difficulty Adjustment, Halving, Cycle, Conjunction
- **Explanation**: Ordinal Theory is like attaching an ID card to each satoshi, making it unique and capable of representing distinct assets like artwork.
- **Example**: Bob stores a digital painting on satoshi #110000.000000001 as an NFT for sale.

---

## 3. 以太坊概述 (Ethereum Overview)

### 3.1 以太坊简介 (Introduction to Ethereum)

Ethereum was proposed by Vitalik Buterin in 2013 and launched in 2015. It is a decentralized platform supporting smart contracts, based on blockchain technology.

- **Features**:
  - **Programmable Blockchain**: Supports Turing-complete programming languages (such as Solidity), allowing developers to create complex applications.
  - **Smart Contracts**: Automatically executed programs running on the Ethereum Virtual Machine (EVM).
  - **Consensus Mechanism**: Used Proof-of-Work (PoW) before "The Merge" in 2022, then transitioned to Proof-of-Stake (PoS).
- **Keywords**: Ethereum, Smart Contracts, Turing Complete, EVM, The Merge, Proof-of-Stake (PoS)
- **Explanation**: Ethereum is like a globally shared computer where anyone can upload and run programs.
- **Example**: A company uses Ethereum smart contracts to automatically pay employee salaries without manual intervention.

### 3.2 与比特币的对比 (Comparison with Bitcoin)

- **Similarities**:
  - Both are decentralized blockchains using public/private key pairs to manage accounts.
  - Both are based on P2P networks and maintain ledgers through consensus algorithms.
- **Differences**:
  - **Programming capability**: Ethereum supports smart contracts, while Bitcoin is limited to simple scripts (not Turing-complete).
  - **Consensus mechanism**: Bitcoin always uses PoW, while Ethereum has transitioned to PoS.
  - **Usage**: Bitcoin primarily serves as a digital currency (medium of exchange) and store of value, while Ethereum supports DApps, NFTs, and more.
- **Keywords**: Decentralized Blockchain, Consensus Algorithm, Medium of Exchange, Store of Value
- **Explanation**: Bitcoin is like digital gold, while Ethereum is like a digital operating system.
- **Example**: Bitcoin is used for cross-border remittances, while Ethereum is used to create decentralized exchanges.

### 3.3 EOAs vs CAs (Externally Owned Accounts vs Contract Accounts)

- **EOAs (Externally Owned Accounts)**

  - **Definition**: Accounts controlled by users through private keys, representing individuals or entities in the Ethereum network.

    **Creation**: Generated by creating a pair of public and private keys, with the public key deriving the address (160-bit hash, starting with 0x).

    **Control**: The private key holder controls the account by signing transactions.

    **Functions**:

    - Send transactions (transfer ETH, call smart contracts).
    - Hold ETH and ERC-20 tokens.
    - Pay Gas fees (page 65: Gas limit issue).

- **CAs (Contract Accounts)**

  - **Definition**: Accounts controlled by smart contract code, stored on the Ethereum blockchain, executing predefined logic.

    **Creation**: Created by deploying smart contracts (including bytecode) through EOAs, generating contract addresses.

    **Control**: Controlled by smart contract code logic, no private keys, requiring calls from EOAs or other CAs.

    **Functions**:

    - Execute smart contract logic (such as DeFi, NFTs, DAOs).
    - Hold ETH and tokens.
    - Automatically respond to transactions or events.

  ### 3.4. Merkle Patricia Trie

  <img src="/Users/sh4nglj/Documents/MS DTTI/SEM B/IS6200 Blockchain/Final Review/note_converted/pictures/S03 MPT.png" alt="S03 MPT" style="zoom:40%;" />

---

## 4. 以太坊的共识机制：权益证明（PoS） (Ethereum's Consensus Mechanism: Proof-of-Stake)

### 4.1 PoS简介 (Introduction to PoS)

Ethereum transitioned from PoW to PoS in 2022 through "The Merge," with validators participating in block creation by staking ETH.

- **Mechanism**: Validators stake at least 32 ETH, are randomly selected to create blocks, and receive transaction fees (Gas Fees) and block rewards.
- **Advantages**:
  - Low energy consumption: PoW requires extensive computation, PoS only requires staking.
  - Environmentally friendly: Reduces carbon footprint.
- **Keywords**: Proof-of-Stake (PoS), The Merge, Validator, Stake, Gas Fees
- **Explanation**: PoS is like shareholder voting, where those holding more ETH have a greater chance of recording transactions.
- **Example**: Alice stakes 32 ETH, becomes a validator, and receives a 0.1 ETH reward after validating transactions.

### 4.2 PoS的问题：无利害关系（Nothing at Stake） (PoS Problem: Nothing at Stake)

PoS faces the "Nothing at Stake" problem: validators might simultaneously validate blocks on multiple branches (forks), increasing the risk of double-spending.

- **Solutions**:
  - **Slashing**: When malicious behavior (such as double voting) is detected, a portion of the validator's ETH is destroyed, and they may be banned from further staking.
  - **Finality**:
    - **Probabilistic Finality**: In PoW, the more block confirmations, the harder it is to tamper with the blockchain.
    - **Cryptoeconomic Finality**: PoS ensures blocks are irreversible through economic incentives.
- **Keywords**: Nothing at Stake, Slashing, Finality, Double-spending
- **Explanation**: Nothing at Stake is like a cheater supporting two teams simultaneously; slashing is like confiscating their bet.
- **Example**: Bob attempts to validate blocks on two branches, is detected by the system, and loses 10 ETH.

### 4.3 PoS攻击场景 (PoS Attack Scenarios)

- **Attack 1: 33% attack**:
  - If attackers control 33% of staked ETH, they can potentially disrupt consensus through inactivity or double voting.
  - **Solution**: Increase the proportion of active validators, set stricter penalties.
- **Attack 2: 51% attack**:
  - Controlling 51% of staked ETH allows complete control of the network, but the cost is extremely high (requiring purchase of large amounts of ETH).
- **Attack 3: Sybil Attack**
  - Attackers generate multiple fake nodes or accounts, posing as legitimate participants in the network.
  - They participate in network voting, consensus, or data propagation, attempting to influence outcomes.
  - Decentralized systems rely on the honest behavior of most nodes; Sybil attacks undermine this trust through "strength in numbers."
  
- **Explanation**: A 33% attack is like minority shareholders causing disruption, while a 51% attack is like controlling shareholders manipulating a company.
- **Example**: An attacker controlling 33% of ETH refuses to validate new blocks, pausing the network until the slashing mechanism takes effect.

---

## 5. 以太坊的扩展性解决方案 (Ethereum's Scalability Solutions)

### 5.1 扩展性问题与区块链三难困境 (Scalability Issues and the Blockchain Trilemma)

Ethereum faces scalability challenges: balancing decentralization, security, and scalability, known as the **Blockchain Trilemma**.

- **Problem**: High transaction volumes lead to network congestion, causing gas fees to skyrocket.
- **Keywords**: Blockchain Trilemma, Decentralization, Security, Scalability
- **Explanation**: The trilemma is like cooking where you can only choose two out of fast, good, and cheap; you cannot have all three.
- **Example**: During the 2021 NFT boom, single transaction fees on Ethereum reached $100.

### 5.2 Layer 1扩展：链上解决方案 (Layer 1 Scaling: On-Chain Solutions)

- **The Merge**: Transition from PoW to PoS, reducing energy consumption and laying the foundation for future scaling.
- **Sharding**:
  - Dividing the blockchain database into multiple shards, each processing a portion of transactions, improving throughput.
  - **Proto-Danksharding**: Preliminary sharding plan, optimizing data storage, reducing Layer 2 costs.
- **Keywords**: Sharding, Proto-Danksharding, Throughput
- **Explanation**: Sharding is like dividing a large library into smaller libraries, allowing readers to borrow different books simultaneously.
- **Example**: After Ethereum sharding, Alice's NFT transaction and Bob's payment transaction are processed on different shards without interference.

### 5.3 Layer 2扩展：链下解决方案 (Layer 2 Scaling: Off-Chain Solutions)

Layer 2 processes transactions outside the main chain (Layer 1), reducing the burden on the main chain, and is divided into the following types:

#### 5.3.1 Rollups

Rollups execute transactions off-chain, submitting compressed data to the main chain.

- **Types**:
  - **Optimistic Rollups**: Assume off-chain transactions are valid, setting a challenge period for disputes. Examples include Arbitrum.
  - **ZK-Rollups**: Use zero-knowledge proofs to verify transactions, more efficient but computationally complex.
- **Advantages**:
  - Lower transaction fees (Gas Fees).
  - Faster transaction speed.
  - Retain main chain security.
- **Disadvantages**:
  - Challenge periods may delay fund withdrawals.
  - Increased complexity makes development more difficult.
- **Comparison with Lightning Network**:
  - **Similarities**: Both are Layer 2 solutions, reducing main chain burden.
  - **Differences**: Lightning Network is based on payment channels, suitable for small payments; Rollups support complex smart contracts.
- **Keywords**: Rollups, Optimistic Rollups, ZK-Rollups, Challenge Period, Arbitrum
- **Explanation**: Rollups are like packaging many transactions into a small package, recording only the package information on the main chain.
- **Example**: Alice trades NFTs through Arbitrum with low fees, requiring only final result verification on the main chain.

#### 5.3.2 Sidechains（侧链）

Sidechains are independent blockchains running parallel to Ethereum, interacting with the main chain through bridges.

- **Features**:
  - Faster block times and larger block sizes, improving throughput.
  - **Polygon PoS**: Ethereum's PoS sidechain, with an average block time of about 2 seconds.
- **Disadvantages**:
  - Reduced security: Not fully reliant on the main chain.
  - Decreased decentralization: Potential emergence of super nodes.
- **Keywords**: Sidechains, Polygon PoS, Block Time, Super Nodes
- **Explanation**: Sidechains are like auxiliary roads to a main road, faster but slightly less secure.
- **Example**: Bob quickly trades game tokens on the Polygon sidechain, with fees only 1/10 of the main chain.

---

## 6. 智能合约与安全问题

### 6.1 智能合约特点 (Smart Contract Characteristics)

- **Immutable**: Code cannot be changed after deployment, unless using a proxy contract.
- **Storage required**: Full nodes need to store all smart contract code.
- **Gas limit**: Execution requires Gas payment; if Gas is insufficient, the transaction fails but Gas is not refunded.
- **Keywords**: Proxy Contract, Full Node, Gas Fees
- **Explanation**: Smart contracts are like vending machines, operating according to preset rules that cannot be changed midway.
- **Example**: Alice's smart contract did not execute due to insufficient Gas, resulting in a loss of 0.01 ETH.

### 6.2 安全漏洞 (Security Vulnerabilities)

- **Reentrancy Attack**: A contract is repeatedly called before payment completion, resulting in stolen funds.
  - **Example**: The 2016 DAO attack, where attackers stole 3.6 million ETH through a reentrancy vulnerability.
- **Storage Collision**:
  - Conflict between proxy contract and implementation contract storage layouts, causing data errors.
  - **Example**: The 2022 Aulius governance attack, where storage collision led to control of the governance mechanism.
- **Infinite loops**: Erroneous code could cause the blockchain to freeze, but Gas limits prevent this problem.
- **Keywords**: Reentrancy Attack, Storage Collision
- **Explanation**: A reentrancy attack is like pressing the withdrawal button multiple times at an ATM before it dispenses cash; storage collision is like two books using the same shelf numbering.
- **Example**: An attacker exploits a reentrancy vulnerability to steal 10 ETH from Alice's contract.

---

## 7. 以太坊与去中心化互联网

### 7.1 互联网的中心化问题 (Centralization Issues of the Internet)

The document quotes Leopold Kohr: "Whenever something is wrong, something is too big." The current internet is highly centralized, controlled by a few tech giants.

- **Example**: Twitter (now X) is operated by a single company, controlling user data and content moderation.
- **Keywords**: Centralized
- **Explanation**: Centralization is like all data being stored on one company's servers, making it easily controlled or leaked.
- **Example**: Twitter's 2022 policy change restricting users from sharing others' real-time locations.

### 7.2 Tor与去中心化 (Tor and Decentralization)

**Tor (The Onion Routing Project)** protects privacy through multi-layer encryption (Onion Routing) but is not completely decentralized, relying on a limited number of relay nodes.

- **Problem**: Relay nodes can become bottlenecks, reducing the degree of decentralization.
- **Keywords**: Tor, Onion Routing, Relay Nodes
- **Explanation**: Tor is like forwarding letters through multiple post offices to hide the sender, but the number of post offices is limited.
- **Example**: Alice uses Tor to access websites, with data encrypted and transmitted through multiple relays, protecting her privacy.

### 7.3 以太坊的去中心化潜力 (Ethereum's Decentralization Potential)

Ethereum provides decentralized alternatives through DApps, such as decentralized social media.

- **Example**: Lens Protocol, a decentralized social platform based on Ethereum, where users control their data.
- **Keywords**: Decentralized Social Media
- **Explanation**: Decentralized social media is like users storing their own posts without relying on platforms.
- **Example**: Bob publishes content on Lens, with data stored on Ethereum that platforms cannot delete.
