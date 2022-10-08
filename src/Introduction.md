# Introduction

## About

Chia Name Service (CNS) is a decentralized ecosystem built on Chia Blockchain with its UTXO model and Chialisp Smart Contracts. CNS not only aims to provide name service to users on Chia Blockchain, but also provides cross-chain service with verifiable proof from the most secured blockchain - Chia.

CNS generates the name with the `.xch` suffix, the name is able to resolve various types of data both on-chain or off-chain, including addresses, content, websites, social accounts, etc. Owners have full ownership and management permission. Owner can trade the name like a normal NFT.

**Our Vision**

CNS is a universal name service that seamlessly connects people, information, assets, and applications in the digital world. Although it is secured by Chia Blockchain, it is chain-agnostic. The CNS is a decentralized, censorship-resistant, and open-sourced digital gateway to Web 3.0.

**Our Goals**

- Realize a secure, transparent, and open-name service.
- Serve as a digital gateway for a person or an organization to Web 3.0.
- Interoperate between Web 3.0 and the Web 2.0.
- Build a universal name service for all digital worlds.

## Features

- **Domain Name**.
    Allow users to register a single unique domain name for easy memory and access.
    Domain names can be registered, modified, queried, and transacted on-chain.
- **NFT**.
    CNS is recorded on the chain in the form of NFT, which can be easily queried and interacted with by any application or user.
    CNS is unique and indivisible and can be transacted and circulated as the NFT in the marketplace.
    The attribute of the domain can always be modified by the owner, others have no chance to manipulate it.
    The attribute can be modified by any compatible wallet/client.
- **Digital Gateway**.
    The CNS can store a collection of personal identity data, and represent the unique identity of Web3.
    Different digital assets can be linked to the CNS, allowing it to become a unique gateway to multi-chain networks.
    Subdomains can be created for members of the company, community, or organization as validate credentials.
    By integrating multi-chain data and even the legacy network data in a single place, the Digital Gateway of Web 3.0 to all your assets is formed.


## 挑战
### 安全的去中心化域名系统
### 子域名的支持
### ...

## 现有方案

### Ethereum Name Service

On the Ethereum blockchain, Ethereum Name Service is the most notable name service. The main smart contract is called the Registry, which contains a mapping from domain names to their Resolvers. Each Resolver is another smart contract, which maps domain names to their actual records (for example Ethereum addresses or content hashes). Therefore, to resolve a domain, one first has to look up the correct Resolver in the Registry and then perform the actual resolution. Since Ethereum often has periods of very high transaction traffic, which leads to extreme transaction fees, Ethereum-based projects inevitably inherit these drawbacks.

### FIO protocol

The FIO Protocol is a decentralized service layer that bridges the gap between crypto endpoints such as wallets, exchanges, crypto payment processors, and any other application in which crypto assets are held and/or transferred. The FIO Protocol reimagines and enables a better way of sending and receiving blockchain-based value, regardless of the wallet, exchange, token, or coin used. It is worth mentioning that FIO has its blockchain but only acts as a service layer independent of other public chains, which ensures the security of address data on the one hand and ensures that the domain name service is not disrupted by the public chain on the other.

### 其他，如TNS/ANS