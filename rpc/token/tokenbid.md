## Token Bid

### Post a public bid order
This order will be made of the parent chain coin to be filled with the token made on that chain.

Usage: `tokenbid numtokens tokenid price`

Example command:
```shell
./komodo-cli -ac_name=ATEST tokenbid 1000 c5bbc34e6517c483afc910a3b0585c40da5c09b7c5d2d9757c5c5075e2d41b59 1```
output:
```JSON
0100000001484256677a6417030dd99716a47b8c9cb06fba6e57ff4617e9932a6cde2972830100000049483045022100fc1926401b27ba044bbf17c36f36030adae52a188594efc75fe42861ab0b997802205e729d6f5587e5a5296b5649a154ce1fe3c581078fac7ae4e2b4577978c05c8901ffffffff0300e8764817000000302ea22c80201ab400e039122028345520ba041ac3e6ec81ad28d8415e78d760d55f41097dd58103120c008203000401cc10d262684a0300002321028bb4ae66aa4f1960a4aa822907e800eb688d9ab2605c8067a34b421748c67e27ac00000000000000004f6a4c4ce362c5bbc34e6517c483afc910a3b0585c40da5c09b7c5d2d9757c5c5075e2d41b59e80300000000000021028bb4ae66aa4f1960a4aa822907e800eb688d9ab2605c8067a34b421748c67e2700000000
```

### User `sendrawtransaction` to publish order


Example command:
```shell
./komodo-cli -ac_name=ATEST sendrawtransaction 0100000001484256677a6417030dd99716a47b8c9cb06fba6e57ff4617e9932a6cde2972830100000049483045022100fc1926401b27ba044bbf17c36f36030adae52a188594efc75fe42861ab0b997802205e729d6f5587e5a5296b5649a154ce1fe3c581078fac7ae4e2b4577978c05c8901ffffffff0300e8764817000000302ea22c80201ab400e039122028345520ba041ac3e6ec81ad28d8415e78d760d55f41097dd58103120c008203000401cc10d262684a0300002321028bb4ae66aa4f1960a4aa822907e800eb688d9ab2605c8067a34b421748c67e27ac00000000000000004f6a4c4ce362c5bbc34e6517c483afc910a3b0585c40da5c09b7c5d2d9757c5c5075e2d41b59e80300000000000021028bb4ae66aa4f1960a4aa822907e800eb688d9ab2605c8067a34b421748c67e2700000000
```
output (bid order txid):
```shell
5fc8c472bc0e5f994b5a9a3fda23af1a3e1cfd746b902d7216352732e6adba05
```