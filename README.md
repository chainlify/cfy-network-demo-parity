CFY Network Demo - Parity
=========================

> a simple parity development ethereum network


Resources:
- https://wiki.parity.io/Docker
- https://wiki.parity.io/Private-development-chain

Ports:
- 8545:8545
- 8546:8546
- 30303:30303
- 30303:30303/udp

Options
- --ui-interface all
- --jsonrpc-interface all

Main Wallet
- 0x00a329c0648769a73afac7f9381e08fb43dbea72
- 0x4d5db4107d237df6a3d58ee5f70ae63d73d7658d4026f2eefd2f204c81682cb7

Example Web3

```
web3.eth.accounts.signTransaction({
  from: '0x00a329c0648769a73afac7f9381e08fb43dbea72',
  to: '0x004c0a4E7dBfB2b7029E526Ac24741231f1AF84d',
  value: web3.utils.toHex(web3.utils.toWei("0.001", "ether")),
  gas: 21000,
}, '0x4d5db4107d237df6a3d58ee5f70ae63d73d7658d4026f2eefd2f204c81682cb7').then(console.log).catch(console.log)
```
