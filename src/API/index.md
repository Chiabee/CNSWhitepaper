# API

| API        | Path                                                   | Type | Summary                                    |
| ---------- | ------------------------------------------------------ | ---- | ------------------------------------------ |
| [Resolve]  | https://walletapi.chiabee.net/Name/resolve             | POST | resolve address or name                    |
| [Resolve]  | https://walletapi.chiabee.net/Name/all                 | GET  | get all names and corresponding address    |
| [Verify]   | https://walletapi.chiabee.net/Wallet/get-coin-solution | POST | get the information for verification       |
| [Register] | https://cns.api.pawket.app/api/price                   | GET  | get price for the CNS to register or renew |
| [Register] | https://cns.api.pawket.app/api/register                | POST | request to register or renew certain CNS   |

- for testnet, prefix `testnet.`
  - Resolving/Verify: https://testnet.walletapi.chiabee.net/
  - Register: https://testnet.cns.api.pawket.app/

[resolve]: Resolve.md
[verify]: Verify.md
[register]: Register.md
