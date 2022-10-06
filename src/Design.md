# Design

## Principles

### Name Principles

According to Zooko's triangle, the name should follow:

1. Human-meaningful, names can be meaningful and memorable to humans.
2. Secure, as long as the Chia Blockchain Consensus is concrete, the CNS can survive various attacks.
3. Decentralised, every entity can start its resolver service without any central authority.

### Everything On-Chain, Non-custody

1. All critical information is On-Chain, non-custody.
2. Every domain is an NFT, and can be transferred and exchanged.
3. Owner of the domain can change the domain reference address afterward, and these changes are also On-Chain.
4. Protocol is open, you can register, update and exchange in a compatible wallet. 

### Resolver 

4. The Off-Chain resolver will provide a quick domain resolving service.
5. Every resolved result can be verified in every full node(by retrieving and parsing an NFT coin's puzzle and solution), Or theoretically by an SPV protocol and even a ZKP protocol. This can avoid malicious resolver attacks and MITM attacks.
6. Resolver would respond not only to the address itself but also come with some critical information(like how long the reference address is stable, which can be done easily by confirmed_index of the domain NFT).
7. Resolver is decentralized, even if we disappear, another team can take up the role and provide the resolving service by collecting information from the On-Chain information.

