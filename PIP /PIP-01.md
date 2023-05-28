# PIP-01: HTLC and Atomic Swap principle

`final` `mandatory` `author: 22388oo`

Portico Exchange works using HTLC (Hashed TimeLock) present on Lightning Network as default, we use this main principle around protocol for provider atomic transactions between layers and sidechains in mode trustless be running our client, using Web UI or simple doing transactions on Portico wallet app

# Why use Lightning Network?

We use Lightning Network, 'cause is the layer-2 more used around world and have more network effect

# Taproot as motivation

In the Exchange we use Taproot application for accelerate transaction between peers

# Glossary

- `tx`: transaction on timechain

# Proof of concept

[Demo and PoC of Portico](https://github.com/PorticoExchange/Portico-Swap)

# How works

In this example below show how works our protocol in JSON

``` json
{
["input": "OP_SWAP OP_PUSHBYTE OP_PUSH"]
["output": "OP_CHECKSIG"] 
["output type": "P2PKH / P2STR / P2SH-P2WPKH / P2WPKH"]
["script": "HASH OP"]
["tx": "xxxx"]
["locktime": "xxxx"]
["block":"xxxx target when open or close channel"]
["hex": "xxxxx"]
},


