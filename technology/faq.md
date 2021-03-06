# FAQ

This guide addresses as many questions you might have about Enter as possible. Please refer to this FAQ section before asking questions on Discord. If your question is still unanswered, please reach out to us through the chat function on our [website](https://blockchainstation.io) in the bottom right corner or join our Discord.

[General questions](broken-reference)\
[ENTER token](broken-reference)\
[Blockchain Station™ network](broken-reference)

## General questions

### What is a consensus algorithm?

A consensus algorithm is a mechanism to reach agreement among nodes in distributed networks. It removes the need for a central authority and allows the whole network to agree on data and the ordering of events in a trustless way.

Nodes participating in the network maintain an exact copy of the ledger, allowing applications built on top of the consensus protocol to function correctly.

### What is aBFT (asynchronous Byzantine Fault Tolerant) consensus? How is it different from blockchains such as Ethereum and Bitcoin?

aBFT consensus stands for “asynchronous Byzantine Fault Tolerant” consensus. When a network is said to be “Byzantine Fault Tolerant”, it means that nodes can still reach an agreement on an ordering of events even if part of the network acts maliciously.

Asynchronous BFT allows nodes in the network to confirm event blocks containing transactions without depending on any timing assumptions. This makes the confirmation of transactions by the network faster, without compromising security or decentralization.\
When a transaction is confirmed by the network, it achieves complete finality and can’t be changed nor reverted. aBFT consensus reaches agreement on transactions even when some of the messages between nodes are lost, which makes the network more resilient

Blockchains such as Ethereum and Bitcoin are synchronous, meaning that transactions are appended into blocks, one at a time. They follow the longest-chain rule in which the chain with the most number of blocks determines the final ordering of events. Transactions in earlier blocks have a much higher probability of being part of the final ordering of events compared to more recent transactions.\
Therefore, these networks require multiple confirmations to ensure that a transaction is permanently part of the blockchain. This behavior leads to a slower confirmation of the transactions than in aBFT consensus.

### What is finality?

Finality means that a transaction cannot be changed or reversed by any party. aBFT consensus algorithms such as Lachesis have a very low time to finality because they achieve absolute finality. Absolute finality means that a transaction is considered final once it is included in a block.

In the case of Enter, Enter Chain can accomplish finality in 1 to 2 seconds.\
TxFlow can achieve finality in less than a second.

Conversely, Nakamoto consensus protocols rely on probabilistic finality. In this case, the probability that a transaction won’t be reverted increases with time. The more blocks that are created on top of a block, thereby confirming it as correct, the more difficult and costlier it would be to revert a transaction in that block. At some point it becomes theoretically impossible to alter older blocks, increasing the probabilistic finality to near 100%.

Bitcoin has finality of 30 to 60 minutes; when using Bitcoin you have to wait a few block confirmations before considering the transaction final and irreversible. Ethereum has a finality of a few minutes.

### What is TxFlow?

TxFlow is an aBFT middleware protocol designed for responsiveness. It runs together with a traditional consensus algorithm such as Lachesis, which guarantees network security.

TxFlow can achieve sub-second latency, which makes it ideal for any application that requires instant confirmation. Check the [GitHub](https://github.com/Fantom-foundation/go-txflow) and the TxFlow [introduction](https://medium.com/fantomfoundation/introducing-txflow-the-protocol-for-responsiveness-a2e42bd5fc3c)

## PLAY token

### Is PLAY an ERC20 token?

Blockchain Station™ has an ERC20 token, but it can’t be used directly on the Blockchain Station™ mainnet. When you send your ERC-20 to the PLAY Wallet, it will automatically be swapped to PLAY native coin.

Here’s a breakdown of the different Enter tokens in circulation at the moment

1\. Blockchain Station™ PLAY: Used on Blockchain Station™ mainnet\
2\. ERC20: ENTRC Exists on the Ethereum network\
3\. BEP20: ENTER Exists on Binance Chain

Note that Blockchain Station™ addresses share the same structure as Ethereum addresses (0x…), **but they are not Ethereum addresses**.

### Can I send ERC20 ENTRC tokens to my Enter Wallet?

No. You need to swap them first to mainnet Enter using [https://multichain.xyz/](https://multichain.xyz).

### What’s the purpose of the ENTER token?

The Enter token has a number of use cases within the Enter ecosystem.\
It plays an essential role for a well-functioning, healthy network.

**1. Securing the network**

Enter uses a Proof-of-Stake system that requires validators to hold ENTER.\
Anyone with at least 1,000 ENTER can run their own validator node to earn epoch rewards and transaction fees.\
Every ENTER holder has the option to delegate their tokens to a validator (while keeping full custody of their funds) to receive staking rewards.\
Validators then take a small fee for their services.

By locking in their ENTER, validators help the network to be decentralized and secure.

**2. Paying for network fees**\
To compensate validators for their services and prevent transaction spam, every action performed within the Enter network costs a small fee.\
This fee is paid in ENTER.

**3. Voting in on-chain governance**\
Decisions regarding the Enter ecosystem are made using transparent on-chain voting.\
Votes are weighted according to the amount of ENTER held by an entity.\
Basically, 1 ENTER equals 1 vote.

With ENTER as the governance token, validators and delegators can vote on network parameters such as block rewards as well technical committees and so forth.

**4. Additional use cases**\
ENTER is used as a collateral on the Enter DeFi suite with Visa crypto cards.

### How can I stake ENTER?

Check out [this guide](broken-reference).

### Can I stake ENTER on exchanges like Binance?

No, you cannot stake ENTER on exchanges at the moment.

### How to run a validator on Blockchain Station™?

To run a validator node on Blockchain Station™, the followings are required:

1. A minimum stake of 1,000 ENTER;
2. Server with 4 CPU, 16GB RAM, and 1TB diskspace.

### Where can I store ENTER?

You can store ENTER on our official PWA wallet for mobile and desktop.

Please note that the above wallets only support Blockchain Station™ Network ENTER. **They do not support ERC20 or BEP2.**

We are working with other wallet providers to add compatibility for the ENTER token.

## Blockchain Station™ network

### What is Blockchain Station™?

Opera is a fully decentralized blockchain network with smart contracts integration for applications. It is compatible with the Ethereum Virtual Machine and powered by Enter's HBFT consensus. Thus, smart contracts developed on Ethereum can run on Enter, with an increase of scalability and security.

### Is Enter compatible with Ethereum smart contracts?

Yes. Blockchain Station™ Network is fully compatible with the Ethereum Virtual Machine (EVM). It also has Web3JS API and RPC support.\
All smart contracts written in Solidity or Vyper, compiled and deployed on Ethereum, are fully compatible with the Opera Network.

### Is Enter compatible with Cosmos SDK?

Yes. Developers can use Enter's fast and secure HBFT consensus mechanism as a base layer and use the Cosmos SDK on top of it.

### What programming languages does Enter support?

Blockchain Station™ network supports all smart contract languages that Ethereum supports for the EVM, which include both Solidity and Vyper.

### When will Enter mainnet go live?

The Blockchain Station™ is planned to go live in the first quarter of 2022, after completing the testing and development stage.
