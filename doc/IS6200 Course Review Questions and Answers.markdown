# IS6200 Blockchain Tech and Bus App: Questions and Answers

## 1 Money
**1.1 What are the three functions of money?**  
The three functions of money are medium of exchange, unit of account, and store of value.

**1.2 How do you rate cryptocurrencies (i.e., digital currencies issued in a blockchain network) as money?**  
Cryptocurrencies are volatile and lack widespread acceptance, making them weak as money.

## 2 Cryptographic Techniques
### 2.1 Encryption
**2.1.a What are symmetric and asymmetric encryptions?**  
Symmetric encryption uses one key for encryption and decryption; asymmetric uses a public-private key pair.

**2.1.b How are these two different from each other?**  
Symmetric is faster but less secure for key sharing; asymmetric is slower but secure for public key exchange.

### 2.2 Hash Functions
**2.2.a What is the definition of a hash function?**  
A hash function maps data to a fixed-size output, producing a unique hash.

**2.2.b For a hash function to be a cryptographic hash function, what are the expected properties?**  
Cryptographic hash functions must be collision-resistant, preimage-resistant, and second preimage-resistant.

**2.2.c What are the distinctions between encryption and hash functions? Or, can we use these two interchangeably?**  
Encryption is reversible; hash functions are one-way and not interchangeable.

### 2.3 Digital Signatures
**2.3.a What is its usage/application?**  
Digital signatures verify authenticity and integrity of messages or transactions.

**2.3.b Is it better than wet-ink signatures? Why or why not?**  
They are more secure than wet-ink signatures but lack legal recognition in some jurisdictions.

**2.3.c How is it used in Bitcoin?**  
In Bitcoin, digital signatures authenticate transactions, ensuring only the owner spends funds.

## 3 Bitcoin
**3.1 Using one sentence, define the Bitcoin network. Note that "Bitcoin" is used to refer to the blockchain network, while "bitcoin" refers to the cryptocurrency on the network.**  
Bitcoin is a decentralized blockchain network for secure, peer-to-peer cryptocurrency transactions.

**3.2 Why is Bitcoin so energy intensive?**  
Bitcoin’s proof-of-work mining requires intensive computational power, consuming significant energy.

**3.3 If it costs so much to help maintain the network, why are there still so many miners?**  
Miners are incentivized by block rewards and transaction fees despite high costs.

**3.4 What is 51% attack in Bitcoin?**  
A 51% attack occurs when one entity controls over 50% of mining power, enabling transaction manipulation.

**3.5 The number of miners has been growing exponentially. How can Bitcoin maintain a 10min average block time?**  
Bitcoin adjusts mining difficulty to maintain a 10-minute average block time.

**3.6 Is Bitcoin ready to handle global transactions? Why or why not?**  
Bitcoin’s low transaction throughput limits its ability to handle global transactions.

**3.7 People have come up with scaling solutions. They often use layer 1 and layer 2 to distinguish the different types of such solutions. What are these two types?**  
Layer 1 solutions modify the blockchain protocol; layer 2 solutions process transactions off-chain.

**3.8 There have been heated discussions on SegWit, Taproot, and the lightning network. What are them?**  
SegWit increases block capacity, Taproot enhances privacy, and Lightning Network enables fast off-chain transactions.

**3.9 What is "ordinals"? How does it change the Bitcoin ecosystem?**  
Ordinals inscribe data on satoshis, enabling NFTs and expanding Bitcoin’s use cases.

## 4 Ethereum
**4.1 It is just another public blockchain network. What makes it special, given that we already have Bitcoin?**  
Ethereum supports smart contracts, enabling decentralized applications unlike Bitcoin’s focus on payments.

**4.2 What is Gas in Ethereum? Why is it needed? (What is the halting problem?)**  
Gas is Ethereum’s transaction fee unit, needed to prevent infinite loops (halting problem).

**4.3 What happened in the 2016 DAO hack? What was the bug? What did the developers do to fix the bug?**  
The 2016 DAO hack exploited a reentrancy bug; developers hard-forked Ethereum to recover funds.

**4.4 Ethereum shifted from PoW to PoS. What is PoS (in Ethereum)? Is it better than PoW?**  
PoS in Ethereum uses staked ETH for validation, reducing energy use compared to PoW.

**4.5 What does it mean by "nothing at stake" in a PoS blockchain network like Ethereum?**  
"Nothing at stake" means validators risk no loss for supporting invalid chains in PoS.

**4.6 In addition to 51% attack, it seems like one with 34% stake might launch attacks as well. How may these attacks happen and how could we counteract such attacks?**  
A 34% stake can disrupt consensus; slashing penalties and randomization counteract such attacks.

**4.7 Is the shift from PoW to PoS a layer 1 or layer 2 scaling solution?**  
The PoW to PoS shift is a layer 1 scaling solution, altering the core protocol.

**4.8 What is "optimistic rollup"? How many honest nodes do we need to ensure that the batched transactions are valid?**  
Optimistic rollup batches transactions off-chain, assuming validity unless challenged; one honest node ensures correctness.

## 5 Decentralized Autonomous Organization
**5.1 What is the principal-agent problem? What are the agency costs?**  
The principal-agent problem is when agents prioritize self-interest over principals; agency costs are monitoring expenses.

**5.2 How do DAOs mitigate this agency conflict?**  
DAOs align interests via transparent, automated smart contract governance.

**5.3 Do DAOs introduce new agency costs? If so, what are such costs?**  
DAOs introduce risks like voter apathy and smart contract vulnerabilities, creating new agency costs.

**5.4 Voting is important in DAO governance. What are the common voting approaches?**  
Common DAO voting approaches include token-based, quadratic, and reputation-based voting.

## 6 Hyperledger Fabric
**6.1 How does frameworks like Fabric facilitate the adoption of blockchain into businesses?**  
Hyperledger Fabric provides modular, permissioned blockchain frameworks for secure business adoption.

**6.2 What is a channel in a Fabric network?**  
A channel is a private subnet for confidential transactions among specific Fabric members.

**6.3 In Fabric, certificate authority is needed for identity management. Why is it important? Recall what's man-in-the-middle attack?**  
Certificate authority ensures trusted identities, preventing man-in-the-middle attacks.

**6.4 How does Raft ordering service work? At most how many failed node can it withstand?**  
Raft orders transactions via a leader-based consensus, tolerating up to (N-1)/2 failed nodes.

**6.5 Can Raft solve the Byzantine Generals Problem?**  
Raft cannot solve the Byzantine Generals Problem, as it assumes non-malicious failures.

## 7 Cryptotokens
**7.1 We can categorise the tokens issued through blockchain networks into different types. What are they?**  
Tokens include payment tokens, utility tokens, security tokens, and non-fungible tokens (NFTs).

**7.2 How does Zcash differ from Bitcoin? What's the novel technology that makes it unique?**  
Zcash uses zero-knowledge proofs for privacy, unlike Bitcoin’s transparent transactions.

**7.3 What are stablecoins? What are the different types? What's its benefit (recall the examples?)?**  
Stablecoins are pegged to assets; types include fiat-backed, crypto-backed, and algorithmic; they reduce volatility.

**7.4 What are NFTs? How are they special? A couple of innovations based on ERC-1155 and ERC-4907 were implemented to improve NFTs. Describe these innovations.**  
NFTs are unique digital assets; ERC-1155 supports fungible and non-fungible tokens, ERC-4907 enables NFT rentals.

**7.5 Metaverse: the role of blockchain - data continuity; transaction.**  
Blockchain ensures data continuity and secure transactions in the metaverse.