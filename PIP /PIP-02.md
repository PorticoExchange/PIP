# PIP-02: Sidechains (Liquid)

`optional`  `draft` `author:22388oo`

# Why use Elements?

Elements is an open source, sidechain-capable blockchain platform, providing access to powerful features developed by members of the community, such as Confidential Transactions and Issued Assets.

# Using cross-assets between Lightning and Sidechains

Having L-BTC support on Portico allow HTLCs more robust and private due confidential transaction and high reputation around Liquid Network

# Example

In the example below we'll show how works this input and output when make 'swap' with pegin or pegout 

```json
{
  "txid": "5fa4ef7898eb704dbaea16634ab68302826c42198c9a5f9ff3e60622f83aac90",
  "hash": "6d5f1b8965db82ef37a6ec7381de4a09f0369a3ec3ac236d17384738974232b2",
  "wtxid": "6d5f1b8965db82ef37a6ec7381de4a09f0369a3ec3ac236d17384738974232b2",
  "withash": "95151cf350baf2c99c0ff36e1f4110989b1f33e0d32d8c302c95ad5ecd79e8a2",
  "version": 2,
  "size": 7525,
  "vsize": 2155,
  "weight": 8620,
  "locktime": 303,
  "vin": [
    {
      "txid": "956e34fb9ace5709183e8bed4555c5d701781735633cfa17e9c1c68fb2462ee1",
      "vout": 0,
      "scriptSig": {
      "asm": "00144e4f612e206ec2a27cd0818630bb3304526cc56a",
      "hex": "1600144e4f612e206ec2a27cd0818630bb3304526cc56a"
    },

