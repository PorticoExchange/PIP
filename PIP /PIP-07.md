# PIP-07: Softchains/Statechains/Spacechains

`optional`  `draft` `author:22388oo`

## What are Softchains/Statechains/Spacechains?

### Softchains

In order to have two-way pegged sidechains, you need a succinct method for proving to the mainchain that a peg-out is valid. PoW FP provides exactly that -- a low-bandwidth way of determining if a chain, and thus a peg-out, is valid. The slowness of PoW FP consensus is not an issue, as peg-outs can be made arbitrarily slow (e.g. one year).

### Statechains

Statechains are a layer two protocol, meaning it enables the transfer of value without burdening the Bitcoin blockchain. This can help with scaling and save fees. Unlike Lightning it is not trustless, but it maintains a high degree of censorship resistance (more so than federated sidechains) due to the fact that withdrawing on-chain is permissionless.

### Spacechains

As part of the softchain design, mainchain nodes would have to download and validate the block headers for each softchain, and in the case of any chainsplit download and validate those blocks using the UTXO set commitments. This would form the basis of the pegout mechanism to enable a two-way peg. To migrate coins to the sidechain, the user would create a mainchain transaction assigning them to a specific softchain and then point to that transaction when confirmed to claim coins on the sidechain. Conversely, you would do the opposite when attempting to peg out of the sidechain. This is where the PoW fraud proofs come into play. During a pegout the idea is to create a transaction on the mainchain referencing a withdrawal transaction on the sidechain. Those coins would not become spendable until after a long confirmation window (say a year) and would remain "locked in the softchain" if the withdrawal transaction on the sidechain was reorged out or found to be invalid. The latter would be discovered because in the event of a chainsplit, the mainchain node will download all of the blocks on each side of the split and verify them using UTXO set commitments. 

## Implementation

TBD

