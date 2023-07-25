# PIP-06: Drivechains

`optional`  `draft` `author:22388oo`

## What is Drivechains?

Drivechain allows Bitcoin to create, delete, send BTC to, and receive BTC from “Layer-2”s called “sidechains”. Sidechains are Altcoins that lack a native “coin” – instead, pre-existing coins from a different blockchain must first be sent over.

Once on a sidechain, coins can change hands an unlimited number of times, and in an unlimited number of new ways. Thus, BTC-owners can opt-in to new features or tradeoffs. Meanwhile, the Bitcoiners who don’t opt-in, never need to care what any sidechain is doing.

Transfers from sidechain back to the mainchain (ie, from Layer 2 back to Layer 1) are not done via verifiable proof, but instead via conjecture-and-refutation. A “bundle” of transfers is asserted, and then slowly “ACKed” over time. After 3 months of ACKing, the bundle succeeds. Thus, the SC:BTC market price cannot deviate significantly from a 1:1 ratio

## Implementation

TBD
