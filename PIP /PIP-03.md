# PIP-03: OP_RETURN layers (Omnibolt and RGB)

`optional`  `draft` `author:22388oo`

## Why use RGB and Omnibolt?

OBD implements the OmniBOLT specification, and it is an open source, off-chain decentralized platform, build upon BTC/OmniLayer network, implements basic multi hop HTLC payment, multi-currency atomic swap, and more off-chain contracts on the network of smart assets lightning channels.

RGB is a scalable & confidential smart contracts system for Bitcoin & lightning network. They embrace concepts of private & mutual ownership, abstraction and separation of concerns and represent "post-blockchain", Turing-complete form of trustless distributed computing which does not require introduction of "tokens".

## Using cross-assets between Lightning and layers

Both the protocol use OP_RETURN and commit transactions for allow mint, send, receive using UTXO also as complementary

Both layers are compatible with Atomic swap and submarine swap

## Example with RGB


```json
"input":"xxx"
"output":"xxxx"
"op":"xxxx"
"state":"xxxx"
"locktime":"xxxx"
```

# Example with Omnibolt

```json
"input":"xxx"
"ouput":"xxx"
"op":"xxx"
"locktime":"xxx"
