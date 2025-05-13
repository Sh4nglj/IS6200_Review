# S05-1 Industry

## 1. Overview of Tokens and Cryptocurrencies

### 1.1 代币与货币的区别 (Differences Between Tokens and Coins)
- **Coins**: Serve as a medium of exchange, used for payments or transactions. For example, Bitcoin is a typical cryptocurrency designed to serve as currency in a decentralized network.
- **Tokens**: Typically function as assets, representing specific uses or interests. Tokens operate on blockchains with diverse functions, such as accessing services or representing ownership.

**Example**: Bitcoin is a coin that can be directly used to purchase goods; ERC-20 tokens on Ethereum (such as Chainlink) are tokens used to pay for smart contract services.

**Keywords**: Tokens, Coins, Medium of Exchange, Assets, Volatile

### 1.2 代币分类 (Token Classification)
#### 1.2.1 支付代币 (Payment Tokens)
- **Definition**: Cryptocurrencies used for payments, emphasizing privacy and decentralization. Bitcoin is the pioneer of payment tokens.
- **Characteristics**:
  - Serve as a medium of exchange, but with low recognition from governments and banks.
  - High price volatility, but gradually improving over time.
- **Example**: Using Bitcoin to purchase coffee at supporting merchants, but the price may change due to market fluctuations.

#### 1.2.2 法定加密货币与稳定币 (Fiat Cryptocurrencies and Stablecoins)
- **Definition**: Stablecoins are cryptocurrencies pegged to fiat currencies, designed to reduce volatility. Fiat cryptocurrencies refer to digital currencies backed by governments (not detailed in the document, supplementary information follows).
- **Supplementary Information**: Stablecoins like USDT (Tether) are pegged 1:1 with the US dollar, widely used in trading to avoid price fluctuations. Fiat cryptocurrencies like China's digital yuan (e-CNY) are issued by central banks.
- **Characteristics**: Stablecoins have low volatility, suitable for daily transactions; fiat cryptocurrencies are regulated by governments with clear legal status.
- **Example**: Using USDT to purchase other tokens on cryptocurrency exchanges, with stable prices; using digital yuan for online payments.

#### 1.2.3 证券代币 (Security Tokens)
- **Definition**: Tokens representing traditional financial assets (such as stocks, bonds), regulated by securities laws (mentioned but not explained in the document).
- **Supplementary Information**: Security tokens record ownership through blockchain, increasing transaction transparency and efficiency, but must comply with strict regulatory requirements.
- **Characteristics**: Can represent company shares, real estate, and other assets, with high liquidity but strict regulation.
- **Example**: A company issues security tokens, allowing investors to purchase company shares through blockchain, similar to stocks but stored in digital form.

#### 1.2.4 实用代币 (Utility Tokens)
- **Definition**: Tokens used to access specific platforms or services (mentioned but not detailed in the document).
- **Supplementary Information**: Utility tokens grant holders the right to use products or services, typically not intended as investment tools.
- **Characteristics**: Strong functionality, usually do not represent asset ownership.
- **Example**: Golem tokens (GNT) on Ethereum used to pay for decentralized computing services.

#### 1.2.5 非同质化代币 (Non-Fungible Tokens, NFTs)
- **Definition**: Tokens representing unique digital assets that cannot be interchanged (such as artwork, virtual real estate).
- **Characteristics**: Each NFT has uniqueness, with ownership recorded on blockchain, commonly used for digital collectibles or game assets.
- **Example**: Purchasing a piece of digital art (such as Beeple's NFT work), with ownership recorded on the Ethereum blockchain.

**Keywords**: Payment Tokens, Fiat Cryptocurrencies, Stablecoins, Security Tokens, Utility Tokens, Non-Fungible Tokens (NFTs), Pioneer

## 2. 货币的三大功能 (Three Functions of Money)
- **Unit of Account**: Money serves as a standard for measuring the value of goods and services. Cryptocurrencies like Bitcoin can be used for pricing, but volatility makes them unstable.
- **Store of Value**: Money needs to maintain long-term purchasing power. Bitcoin does not fully satisfy this function due to price fluctuations, but assets like gold are typical stores of value.
- **Medium of Exchange**: Money is used for trading goods and services. Bitcoin and stablecoins can serve as mediums of exchange, but with limited acceptance.

**Example**: A coffee shop prices 1 cup of coffee = 0.0001 Bitcoin (unit of account), the customer pays with Bitcoin (medium of exchange), but Bitcoin price drops may reduce its value (insufficient store of value).

**Keywords**: Unit of Account, Store of Value, Medium of Exchange

## 3. 全球加密货币监管 (Global Cryptocurrency Regulation)
The document shows the global regulatory status of cryptocurrencies (as of November 2021):
- **Absolute Ban**: Some countries (such as China) prohibit all cryptocurrency transactions.
- **Implicit Ban**: No explicit legislation prohibiting cryptocurrencies, but indirect restrictions through limiting banking services, etc.
- **Regulated**: Many countries (such as the United States) regulate cryptocurrencies through taxation, Anti-Money Laundering, and Anti-Terrorism Financing laws.
- **El Salvador**: The first country in the world to adopt Bitcoin as legal tender.

**Supplementary Information**: As of 2025, the regulatory environment continues to evolve. For example, China maintains a strict ban, while the European Union regulates the market through MiCA (Markets in Crypto-Assets Regulation).

**Example**: In the United States, crypto transactions must be reported to the IRS for taxation; in China, individuals holding cryptocurrencies may face legal risks.

**Keywords**: Absolute Ban, Implicit Ban, Regulated, Legal Tender, Anti-Money Laundering, Anti-Terrorism Financing

## 4. 萨尔瓦多比特币实验 (El Salvador's Bitcoin Experiment)
The document details El Salvador's experiment of adopting Bitcoin as legal tender and its results:

### 4.1 实验背景 (Experiment Background)
- **2021**: President Nayib Bukele announced that Bitcoin would become legal tender starting September 7.
- **Public Reaction**:
  - UCA poll (August 2021): 90% of the population did not understand Bitcoin, 80% had little confidence in its use, 70% believed the law should be repealed.
  - 2023 poll: 92% of people do not use Bitcoin for transactions, slightly worse than in 2021 (88%).

### 4.2 实验结果 (Experiment Results)
- **Reasons for Failure**:
  - Low public acceptance, lack of trust and understanding of cryptocurrencies.
  - The International Monetary Fund (IMF) warned about Bitcoin risks, affecting El Salvador's ability to obtain loans.
- **February 2025**: El Salvador abandoned Bitcoin as legal tender as a condition for receiving a $1.4 billion bail-out from the IMF.
- **Lessons**: The Bitcoin experiment shows that cryptocurrencies as legal tender require broad public support and infrastructure.

**Example**: Merchants in El Salvador were forced to accept Bitcoin, but many customers still used US dollars due to Bitcoin's high price volatility and operational complexity.

**Keywords**: Legal Tender, Bail-Out, Public Acceptance

## 5. Zcash 与零知识证明 (Zcash and Zero-Knowledge Proof)
Zcash is a privacy-focused payment token; the document introduces its features and zero-knowledge proof.

### 5.1 Zcash 特点 (Zcash Features)
- **Based on Bitcoin**: Zcash inherits Bitcoin's block reward and fixed total supply.
- **Privacy**: Implements selective disclosure through encryption technology, different from Bitcoin's complete transparency.
- **Address Types**:
  - **Shielded Address (z-)**: Transaction information is not visible, protecting privacy.
  - **Transparent Address (t-)**: Similar to Bitcoin, transactions are public.
- **Transaction Types**: Supports four transaction combinations (shielded to shielded, shielded to transparent, etc.).

**Example**: Alice uses Zcash's shielded address to transfer funds to Bob; the transaction amount and addresses are not visible to the public, but Bob can verify receipt of the funds.

### 5.2 零知识证明 (Zero-Knowledge Proof)
- **Definition**: A cryptographic technique allowing one party (the prover) to prove to another party (the verifier) that certain information is true without revealing the specific information.
- **Simple Explanation**: Like proving you know a password without saying the password itself.
- **Example (provided in the document)**:
  - Alice proves to color-blind Bob that two pens have different colors (one red, one green), without telling the specific colors.
  - Method: Bob randomly swaps the pens, Alice correctly states each time whether they were swapped, proving she can distinguish colors.
- **Application in Zcash**: Zero-knowledge proofs ensure transactions are valid (correct amounts, no double-spending) while hiding transaction details.

**Supplementary Information**: Zcash uses zk-SNARKs (Zero-Knowledge Succinct Non-Interactive Arguments of Knowledge), which are computationally efficient and suitable for blockchain privacy protection.

**Keywords**: Zcash, Zero-Knowledge Proof, Selective Disclosure, Shielded Address, Transparent Address, Block Reward, Fixed Total Supply

## 6. 加密货币相关犯罪 (Cryptocurrency-Related Crimes)
### 6.1 规模与影响 (Scale and Impact)
- **Research Data** (Foley et al., 2019):
  - About 25% of Bitcoin users are involved in illegal activities.
  - Approximately $76 billion in illegal transactions annually (46% of Bitcoin transactions), close to the size of US and European drug markets.
- **Trend**: The proportion of illegal transactions has decreased with increased mainstream interest and the emergence of more opaque cryptocurrencies (such as Monero).

### 6.2 案例 (Cases)
- **2016 Bitcoin Theft**: The US Department of Justice recovered $3.6 billion in stolen Bitcoin, the largest financial seizure in history.
- **2024 Ethereum Attack**: Two brothers stole $25 million in 12 seconds by attacking the Ethereum blockchain, involving wire fraud and money laundering.

**Example**: Hackers exploit cryptocurrency anonymity to purchase illegal goods on the dark web, while law enforcement agencies track fund flows through blockchain analysis.

**Keywords**: Crypto-Enabled Crimes, Illegal Activity, Financial Seizure

## 7. 最大可提取价值 (MEV Exploits)
The document introduces MEV (Maximal Extractable Value), which is the practice of extracting additional profits by reordering blockchain transactions.

### 7.1 基本概念 (Basic Concepts)
- **Definition**: MEV is the additional value that validators (or miners) can obtain by manipulating transaction order, inserting, or excluding transactions.
- **Origin**: Originated from miner behavior in Proof of Work (PoW).
- **Realized Economic Value**: The actual MEV profits obtained.
- **Mechanism**: Validators prioritize transactions based on gas fees to profit.

**Example**: Miners place high gas fee transactions at the beginning of blocks, prioritizing them to earn more fees.

### 7.2 套利 (Arbitrage)
- **Definition**: Profiting from price differences in different markets, considered "benign MEV."
- **Example (Stock Arbitrage)**:
  - Stock price is $100 at exchange A, $99 at exchange B.
  - Buy 1000 shares at B ($99/share), sell at A ($100/share), net profit $980 (after $20 in fees).
- **Blockchain Arbitrage**: Exploiting price differences in Automated Market Makers (AMMs).
  - **Constant Product Market Maker (CPMM)**:
    - Formula: \( R_A \times R_B = K \) (K is constant).
    - Initial: Pool has 1000 A and 1000 B tokens, K = 1,000,000, A:B price is 1:1.
    - Market price: 1.1 A = 1 B.
    - Arbitrageurs deposit B tokens, withdraw A tokens, adjusting the pool price to market level, earning the difference.

**Example**: An arbitrageur discovers that token A's price in a Uniswap pool is lower than the market, buys A and sells it on another exchange for profit.

### 7.3 前置交易 (Front-Running)
- **Definition**: Profiting by inserting one's own transaction before another transaction based on advance knowledge, considered malicious MEV.
- **Example (Stock Market)**:
  - A broker learns that a client will purchase 500,000 shares (price $100).
  - The broker first buys 5,000 shares ($100/share), pushing the price to $101.
  - The client's order pushes the price to $110, the broker sells 5,000 shares, making $50,000.
- **Blockchain Front-Running**:
  - MEV bots (like Jaredfromsubway.eth) use high gas fees to execute transactions first, earning millions of dollars.

**Example**: A user submits a large buy order on Uniswap, MEV bots buy tokens first to drive up the price, then sell for profit.

**Keywords**: Maximal Extractable Value (MEV), Arbitrage, Front-Running, Automated Market Maker (AMM), Constant Product Market Maker (CPMM), Gas Fee, Benign MEV, Realized Economic Value

## 8. DeFi

Decentralized Finance (DeFi) is a financial system based on blockchain technology that provides financial services through smart contracts without requiring traditional intermediaries (such as banks, brokers). DeFi utilizes decentralized blockchain networks (like Ethereum) to achieve transparent, open, and trustless financial operations.

DeFi is like a "bank without people," where all financial services (such as lending, trading, saving) are completed through automatically running code (smart contracts), without requiring banks or companies to intervene. Anyone with a crypto wallet can participate, it's globally accessible, and operations are publicly recorded on the blockchain.

------

### DeFi 的核心特点 (Core Features of DeFi)

1. 去中心化 (Decentralized)
   - No central authority controls it; it runs on a distributed network maintained collectively by all participants.
   - **Example**: In traditional banking, loans require bank approval; on the DeFi platform Aave, users automatically borrow and lend through smart contracts.
2. 开放性 (Permissionless)
   - Anyone can participate without identity verification or credit assessment, just needing a crypto wallet.
   - **Example**: Global users can trade tokens through Uniswap (a decentralized exchange) without registering an account.
3. 透明性 (Transparency)
   - All transaction records are publicly viewable on the blockchain, code is typically open source, and anyone can verify it.
   - **Example**: On the Compound platform, lending rates and fund pool status are visible in real-time.
4. 可组合性 (Composability)
   - DeFi protocols are like "Lego blocks" that can be combined to create new services.
   - **Example**: Users collateralize ETH on MakerDAO to generate DAI stablecoins, then use DAI for trading on Uniswap.
5. 自动化 (Automation)
   - Smart contracts automatically execute financial operations, reducing human intervention and lowering costs.
   - **Example**: On Yearn.Finance, smart contracts automatically optimize fund allocation to achieve the highest yields.

------

### DeFi 的主要服务 (Main DeFi Services)

1. 去中心化交易所 (DEX, Decentralized Exchange)
   - Users directly trade crypto assets without intermediaries.
   - **Example**: Uniswap allows users to swap ETH and ERC-20 tokens, with prices set by an Automated Market Maker (AMM).
   - **Keywords**: Automated Market Maker (AMM)
2. 借贷 (Lending and Borrowing)
   - Users can lend crypto assets to earn interest or borrow against collateral.
   - **Example**: On Aave, users collateralize ETH to borrow USDT, with interest rates determined by supply and demand.
   - **Keywords**: Collateral
3. 流动性挖矿 (Liquidity Farming)
   - Users provide assets (such as token pairs) to liquidity pools, earning transaction fees or rewards.
   - **Example**: On SushiSwap, users deposit ETH/USDT pairs and receive SUSHI token rewards.
   - **Keywords**: Liquidity Farming
4. 质押 (Staking)
   - Users lock assets to support network security or protocol operation, receiving returns.
   - **Example**: On Lido Finance, staking ETH supports the Ethereum 2.0 network, earning staking rewards.
   - **Keywords**: Staking
5. 稳定币 (Stablecoins)
   - Tokens pegged to fiat currencies, reducing price volatility, widely used in DeFi transactions.
   - **Example**: DAI is a decentralized stablecoin issued by MakerDAO, pegged 1:1 to the US dollar.
   - **Keywords**: Stablecoins
6. 收益优化 (Yield Farming)
   - Users maximize investment returns through strategies, often involving multiple DeFi protocols.
   - **Example**: Depositing stablecoins on Curve Finance, then staking reward tokens on Balancer, cycling to optimize yields.
   - **Keywords**: Yield Farming

------

### DeFi 的优势 (Advantages of DeFi)

- **Low Cost**: No intermediaries needed, transaction fees are typically lower than traditional finance.
- **Global Access**: Anyone with internet can use it, breaking geographical restrictions.
- **Efficiency**: Transactions and settlements are almost instantaneous, without waiting for bank processing.
- **Innovation**: New financial products and services rapidly emerge, such as Flash Loans.

------

### DeFi 的风险 (Risks of DeFi)

1. 智能合约漏洞 (Smart Contract Risks)
   - Code errors may lead to stolen funds.
   - **Example**: In 2021, Poly Network lost $600 million due to contract vulnerabilities (later recovered).
2. 市场波动 (Market Volatility)
   - Large price fluctuations in crypto assets may cause insufficient collateral value.
   - **Example**: ETH price crashes could trigger liquidations on Aave.
3. 监管不确定性 (Regulatory Uncertainty)
   - Regulations for DeFi are still unclear in many countries, potentially facing legal risks.
   - **Example**: The US SEC is investigating Uniswap's compliance.
4. 用户错误 (User Errors)
   - Lost private keys or operational mistakes may lead to permanent loss of funds.
   - **Example**: Users incorrectly transferring to invalid addresses, with funds unrecoverable.

------

### DeFi 在元宇宙和 GameFi 中的应用 (DeFi Applications in Metaverse and GameFi)

- 元宇宙 (Metaverse): DeFi supports financial activities in virtual worlds, such as virtual land leasing or NFT trading.
  - **Example**: In Decentraland, users purchase virtual real estate through DeFi lending protocols.
- GameFi: DeFi mechanisms (such as staking, lending) integrated into games, allowing players to earn income through Play-to-Earn (P2E) models.
  - **Example**: In Axie Infinity, players collateralize NFT pets to borrow tokens for game investments.

**Keywords**: Play-to-Earn (P2E), Virtual Land

------

### 实际案例 (Real-world Cases)

- **Uniswap**: A decentralized exchange where users can swap tokens and provide liquidity to earn fees.
- **MakerDAO**: A protocol generating DAI stablecoins, where users collateralize crypto assets to control money supply.
- **Aave**: A decentralized lending platform supporting deposits, loans, and flash loans for various assets.
