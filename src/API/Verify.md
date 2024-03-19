# Verify

The security of CNS resolving can be greatly upgraded by doing verification, which require access to synchronized full node. 

The quick and dirty way is just resolve without verify, but to resist the malicious resolver, the client are persuade to verify the proof in the client side.

Here is the steps:

1. download coin data from blockchain for the proof coin
2. parse(uncurry) the coin and check the correctness of name and binding address
3. check the next coin of this proof coin is not spent (that the proof coin is the latest changes)

## API to check coin

Different client may have different way to get the coin details, here is one way to demonstrate this function.

**POST** https://walletapi.chiabee.net/Wallet/get-coin-solution

**Request:**

```json
{
  "coinIds": ["0x59cffe9b0d863c74e04bd41aad96f39ca74bf8494d09e74aa387ad2dbc81086d"]
}
```

**Response:**

```json
[
  {
    "coin": {
      "amount": 1,
      "parent_coin_info": "0x804037b1362351a6e9b29f0dc3a821a81143dc499fd953a1b9573ed95fc4836e",
      "puzzle_hash": "0x10d14864451e4c2e6e94d58512b29f7de603e77713ed62e4b23f1b8af44f3b0d"
    },
    "puzzle_reveal": "0xff02ffff01ff02ffff0...",
    "solution": "0xffffa0793d3984ad2321...",
    "confirmed_index": 4946819,
    "spent_index": 4952003,
    "timestamp": 1707986063
  }
]
```
