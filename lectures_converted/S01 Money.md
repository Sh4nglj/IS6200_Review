# S01 Money

## 一、货币的定义与历史演变

### 1.1 货币的本质 (What is Money?)

Money serves as a medium of exchange, store of value, and unit of account, simplifying transactions and facilitating economic activities. The document poses the question: "What comes to mind when you think of money?" to encourage reflection on the multiple functions of money.

- **交换媒介 (Medium of Exchange)**: Money solves the inefficiency problem of barter. For example, in ancient times, one might need to exchange eggs for cloth, but the needs of both parties might not match; money simplifies transactions as a universal medium.
- **价值储存 (Store of Value)**: Money  
  - Example: Gold is often used as a store of value due to its scarcity and durability.
- **记账单位 (Unit of Account)**: Money provides a uniform standard for measuring value.
  - Example: The US dollar as a unit of account in international trade.

**Supplementary**: Economist Milton Friedman mentioned in "Money Mischief" that the form of money has evolved from stones and feathers to paper currency and electronic data, and may exist in the future as "computer bytes".

### 1.2 物物交换的历史 (Bartering History)

Before the emergence of money, barter was the main form of transaction, but it was inefficient due to the problem of the "double coincidence of wants".

- **古代物物交换 (Ancient Barter)**:
  - Example: A farmer exchanging grain for pottery, but the pottery maker might not need grain, leading to transaction failure.
- **现代物物交换 (Modern Barter)**:
  - Example: During the 2022 Xi'an lockdown in China, residents exchanged cigarettes for cabbage or Nintendo Switch gaming consoles for instant noodles through social media.
  - Platforms like **Bunz** (a Toronto-based barter community) facilitate modern barter, where users exchange clothing, furniture, and other items.
  - **B2B物物交换 (Business-to-Business Bartering)**:
    - Example: In 1990, Pepsico signed an agreement with the Soviet Union to exchange soft drink concentrate for vodka and merchant ships, valued at $3 billion.
  - **媒体物物交换 (Media Barter)**:
    - Example: Through **Capital Media Solutions**, businesses can exchange advertising space for other services, avoiding cash transactions.

**Supplementary**: Michael B. Wong's 2024 research ("Money and Barter in the Field") demonstrated through the Bunz community's digital currency experiment that money overcomes the inefficiency of barter, but emphasized that redeemability is essential for currency circulation.

### 1.3 货币的功能与加密货币的表现 (Functions of Money and Performance of Cryptocurrencies)

The document cites Charles Wheelan's "Naked Economics" to evaluate the performance of cryptocurrencies in terms of money functions:

- **记账单位 (Unit of Account)**: Grade F (Fail). Due to severe price fluctuations, Bitcoin is not suitable as a stable measure of value.
  - Example: In 2021, Bitcoin's price soared from $30,000 to $69,000, making it difficult to use for daily pricing.
- **价值储存 (Store of Value)**: Grade D (Poor). Volatility makes it unstable, but in some situations (such as government collapse), it can serve as a hedge.
  - Example: During Venezuela's hyperinflation, residents turned to Bitcoin to preserve wealth.
- **交换媒介 (Medium of Exchange)**:
  - Ordinary people: Grade C (Average). Due to long median transaction confirmation time and high fees, Bitcoin is inefficient for everyday transactions.
  - Unstable countries: Grade B+ (Good). In areas with failing governments, Bitcoin provides an alternative payment method.
  - Illegal transactions: Grade A+ (Excellent). Its anonymity makes it used for illegal activities such as drug trading.

**Supplementary**: The Central African Republic was the first country to adopt Bitcoin as legal tender, but the legal status of Bitcoin globally varies greatly, from completely legal to strictly prohibited.

---

## 二、比特币与区块链的起源 (Origin of Bitcoin and Blockchain)

### 2.1 比特币的提出 (Bitcoin's Proposal)

Bitcoin was proposed by the mysterious figure Satoshi Nakamoto in 2008, aiming to create a peer-to-peer electronic cash system that doesn't require a trusted third party. Its core features include:

- **防止双重支付 (Prevention of Double-Spending)**: Verifying transactions through a peer-to-peer network.
- **匿名性 (Anonymity)**: Participants don't need to reveal their real identities.
- **工作量证明 (Proof-of-Work)**: Generating new coins and maintaining network security through hash calculations (Hashcash).

**Example**: Satoshi Nakamoto published the Bitcoin white paper on November 1, 2008 via email.

### 2.2 比特币之前的尝试 (Attempts Before Bitcoin)

Bitcoin was not the first attempt at digital currency; the document mentions the following pioneers:

- **PayPal** (1998): An online payment platform, relying on centralized trust.
- **e-gold** (1996): A digital currency backed by gold, shut down due to regulatory issues.
- **b-money** (1998): Proposed by Wei Dai, emphasizing anonymity and decentralization, influenced by the Crypto-Anarchy ideology.
  - **密码朋克 (Cypherpunk)**: An ideology advocating for anarchism through cryptography, believing that encryption can render violence ineffective because participants cannot be tracked.

**Supplementary**: The domain name bitcoin.org was registered on August 18, 2008, and is hosted on Cloudflare's servers.

### 2.3 区块链1.0 (Blockchain 1.0)

Blockchain is the core technology of Bitcoin, known as "Blockchain 1.0," referring to cryptocurrency blockchains represented by Bitcoin. Its characteristics include distributed ledger and immutable records.

- **定义 (Definition)**: Blockchain is a chain of transactions linked by cryptography, maintained by nodes.
- **Example**: The Bitcoin network records each transaction through timestamps and hashes, forming an unchangeable chain.

**Supplementary**: Blockchain 1.0 mainly focuses on currency functionality; subsequent Blockchain 2.0 (smart contracts) and 3.0 (decentralized applications, DApps) expanded the application scenarios.

---

## 三、密码学基础 (A Taste of Cryptography)

Cryptography is the cornerstone of blockchain technology. The document introduces three core concepts: encryption, hash functions, and digital signatures.

### 3.1 加密 (Encryption)

Encryption converts plaintext into ciphertext to protect information security. It is divided into:

- **对称加密 (Symmetric Encryption)**:
  - Uses the same key for encryption and decryption.
  - Example: VPNs (such as ivpn.cityu.edu.hk at City University of Hong Kong) and HTTPS use symmetric encryption to protect data transmission.
- **公钥加密 (Public Key Encryption)**:
  - Uses a pair of keys: public key for encryption, private key for decryption.
  - Example: Alice encrypts a message with Bob's public key, and only Bob's private key can decrypt it.
  - **RSA加密 (RSA Encryption)**: A public key encryption algorithm based on the factorization of large prime numbers.
    - The document provides an RSA decryption exercise, requiring a private key to decrypt ciphertext.

**Supplementary**: Symmetric encryption is fast but requires a secure channel for key distribution; public key encryption is more secure but computationally complex, often used for key exchange.

### 3.2 哈希函数 (Hash Functions)

Hash functions map data of arbitrary length to values of fixed length (Hash/Digest/Fingerprint), used in blockchain for data integrity verification.

- **特性 (Features)**:
  - **单向性 (One-Way Function)**: It is impossible to derive the original input from the hash value.
  - **抗碰撞性 (Collision Resistance)**: The probability of different inputs producing the same hash is extremely low.
  - **确定性 (Deterministic)**: The same input always produces the same hash.
  - **敏感性 (Sensitivity)**: Small changes in input lead to significant changes in the hash.
- **示例 (Examples)**:
  - Password storage: Websites store hash values of user passwords (e.g., SHA256("123")).
  - **加盐密码 (Salted Passwords)**: Adding a random string (Salt) after the password to enhance security.
    - Example: SHA256("123"+"FDAF\#!2") produces a different hash.
  - **比特币核心 (Bitcoin Core)**: Uses SHA256 to verify transaction and file integrity.
  - **BitTorrent**: Uses hashes to verify the integrity of downloaded files.

**Exercise**: The document asks whether "MyHash" is a valid hash function; due to its lack of one-way functionality and collision resistance, it does not meet cryptographic requirements.

### 3.3 数字签名 (Digital Signature)

Digital signatures are used to verify the authenticity and integrity of messages, superior to wet-ink signatures and electronic signatures.

- **机制 (Mechanism)**:
  - The sender signs the hash value of the message with their private key, and the recipient verifies it with the public key.
  - Example: Alice signs the message hash, and Bob verifies it using Alice's public key, ensuring the message has not been tampered with.
- **优势 (Advantages)**:
  - **不可伪造 (Unforgeable)**: Because only the sender holds the private key.
  - **可验证 (Verifiable)**: Recipients can confirm the validity of the signature.
- **应用 (Applications)**: Bitcoin transactions verify ownership through digital signatures.

**Supplementary**: Digital signatures are based on asymmetric encryption (such as RSA or ECDSA) and are widely used in software distribution and blockchain transactions.

### 3.4 加密与哈希函数的区别 (Differences Between Encryption and Hash Functions)

- **加密 (Encryption)**: A reversible process aimed at protecting data privacy, where ciphertext can be decrypted back into plaintext using a key.
- **哈希函数 (Hash Functions)**: An irreversible process that generates a fixed-length digest, used to verify data integrity, with no concept of decryption.

**Example**: Encryption protects bank account information, while hashing verifies whether a file has been tampered with.

---

## 四、区块链的重要性 (Why Blockchain Matters?)

Blockchain addresses the dependence on centralized institutions in traditional financial systems through decentralization, transparency, and immutability.

- **去中心化 (Decentralization)**: No single point of control, reducing trust costs.
- **透明性 (Transparency)**: Transaction records visible to all nodes.
- **安全性 (Security)**: Cryptography ensures data cannot be tampered with.

**Example**: The Bitcoin network can complete global transfers without banks, reducing fees and improving efficiency.

**Supplementary**: The applications of blockchain have expanded to supply chain management, medical records, voting systems, and other areas.

---

## 五、重点词汇表 (Key Terms)

Below are key English terms from the document and their Chinese explanations:

- **Blockchain (区块链)**: Distributed ledger technology recording an immutable chain of transactions.
- **Bitcoin (比特币)**: A decentralized digital currency based on blockchain.
- **Cryptocurrency (加密货币)**: Digital currency protected by cryptography, such as Bitcoin.
- **Medium of Exchange (交换媒介)**: A universal tool used for transactions.
- **Store of Value (价值储存)**: Assets that can preserve wealth over the long term.
- **Unit of Account (记账单位)**: Standard for measuring value.
- **Barter (物物交换)**: A transaction method of directly exchanging goods or services.
- **Peer-to-Peer (点对点)**: Direct interaction mode without intermediaries.
- **Double-Spending (双重支付)**: Fraudulent behavior where the same digital currency is used multiple times.
- **Proof-of-Work (工作量证明)**: A mechanism for verifying transactions by solving computational puzzles.
- **Cryptography (密码学)**: Mathematical techniques for protecting information security.
- **Encryption (加密)**: A protection method that converts data into an unreadable form.
- **Hash Functions (哈希函数)**: Functions that generate fixed-length data digests.
- **Digital Signature (数字签名)**: Encryption technology for verifying message authenticity.
- **Public Key (公钥)**: A public key used for encryption or signature verification.
- **Private Key (私钥)**: A confidential key used for decryption or signing.
- **Anonymity (匿名性)**: The characteristic of hiding the identity of transactors.
- **Decentralization (去中心化)**: System architecture without central control.

