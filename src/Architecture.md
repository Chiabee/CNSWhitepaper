# Technical Architecture

![](architecture.drawio.svg)

- Full Node: This pertains to a full node that is used to obtain data from the Chia blockchain in real-time. 
- Syncer: The Syncer is a device used for real-time analysis of the data on the full node, and to store this data into a database for future reference.
- Resolver: This is a component that receives requests to resolve domain names from users, and then provides the results of these domain resolutions.
- Registrar: The Registrar is in charge of receiving registration requests from users and provides NFT Offer for domain name registration. The core private key that verifies the legality of the domain name resides here and requires high-level security protection.
- Pawket (Wallet): Serving as a user's terminal for the blockchain, the Pawket can perform decentralized registration, resolution, verification, updates, and transactions.
- xch.cool website: The personalized pages on this website allow one to view their account's NFTs, CATs, XCHs, and other asset information.

## Wallet Functions

- Registration: Submit a registration request to the registrar. If the domain name is available, it can obtain an NFT Offer for the domain name. After signature in the wallet, it sends the transaction directly to the full node for registration.
- Resolution: Initiate a resolution request to the resolver, providing domain names to get corresponding basic information and NFT coin information.
- Verification: Based on the NFT coin information obtained during the resolution, verification is carried out via the full node to check 1) whether the coin is a valid and legal domain name NFT, and 2) whether it matches the resolution information.
- Update: Construct transaction information to update the NFT and submit it to the full node for chaining.
- Transaction: Domain name NFT is fully compatible with regular NFTs and can be traded on any market capable of handling NFT transactions.