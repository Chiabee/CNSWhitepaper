# FAQ

## Before Registration

### What is CNS?
- CNS (Chia Name Service) is a decentralized domain name service built on the Chia blockchain. Use CNS to receive on-chain assets such as XCH, CATs, NFTs, etc. without copying and pasting lengthy and illegible addresses. Name format example: pawket.xch

### Which wallets currently support CNS?
- Currently only [Pawket](https://info.pawket.app/download) wallet supports using CNS instead of an address to send assets.

### Is CNS only for storing Chia addresses?
- In addition to Chia addresses, CNS can also bind other information such as public key, DID, and text. In the future, social accounts such as Email and Twitter may be supported as well.

### Can I use a CNS name to point to my website?
- Pointing to other websites is not supported for now.
- However, CNS has its own profile homepage (name.xch.cool, eg [pawket.xch.cool](https://pawket.xch.cool/)), which displays your NFT assets, transaction history, etc. In the future, it will support custom decoration of your profile homepage.

### What is the length range for registering a CNS name?
- Currently it supports registration of names within the range of 6 ~ 63 characters.
- 6 characters or less are temporarily unavailable.
- More than 63 characters are unavailable either.

### How much does it cost to register a CNS name? 
- The fee includes registration fee (needed to pay for the first registration) and service fee (charged annually).
  - CNS is priced in USD and paid in XCH.
  - 7 characters and above: 0 registration fee + about $6 service fee/year;
  - 6 characters: about $6 registration fee + $10 service fee/year.
  - Disclaimer:The above fees are for reference only. Due to the real-time fluctuations in the price of XCH, there may be some differences in the dollar valuation of the domain. We will make adjustments regularly to keep its dollar price around this level.

### Can I register a name other than .xch?
- For now, only .xch names are supported for registration.

## When Registering

### What are the rules to register a CNS name?
- Letters, numbers, and hyphen "-" are supported, and the hyphen "-" cannot be used for the first 4 digits.
- Special symbols and emoji are not supported.

### Can I choose the registration period when registering?
- Currently you can only choose the registration period for one year.

### Do I have to bind a Chia address when registering?
- If you do not fill in the binding address when registering, the CNS owner's address will be bound by default, which means, the assets received under this name will enter the owner's address. After forwarding or trading to others, the binding address will be automatically updated to the address of the new owner.
- If you fill in the binding address (which can be different from the holding address), the address will not change after forwarding or trading. The owner can modify the binding address.

### Do I have to add fees?
- It's up to you. The transaction will speed up after adding fees, and the transaction can be completed without adding fees. Adding fees is recommended during sandstorms.

### After payment, how to confirm whether the registration is successful?
- You can check it in wallet NFT or blockchain explorer.

## After Registration

### How to add/modify my binding information?
- In the Pawket wallet, find the corresponding NFT, and click it to add/modify in the Binding Information.

### How do I transfer my CNS to someone else?
- In the Pawket wallet, find the corresponding NFT, click it and select transfer, and you can also perform other transactions, such as selling, moving to DID, etc.

### How to send a transaction using CNS? 
- In the Pawket wallet, when sending a transaction, you just need to enter the CNS name in the address bar.

### How to renew my CNS?
- Under development, stay tuned.

### How to unregister my CNS?
- Currently not supported.
- Tips:
   1. If the binding address is cancelled in the binding information, it will be bound to the holder address of the CNS NFT by default.
   1. If the NFT of CNS is burned (the NFT is sent to a verifiably unspendable address: xch1qqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqqm6ks6e8mvy), the CNS cannot be deregistered.
