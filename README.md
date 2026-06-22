# Genote — live demo

A live, on-chain demo of **Genote**, a private journal built on the [GenLayer](https://genlayer.com) Asimov testnet.

🔗 **Live:** https://gumilang88.github.io/genote-demo/

This is a single static `index.html` — no backend. It talks to the GenLayer contract directly
from the browser using [`genlayer-js`](https://www.npmjs.com/package/genlayer-js) loaded from a CDN,
and your **MetaMask wallet signs every write**.

## What you can do

- **Connect wallet** — MetaMask is switched to (or added for) the GenLayer Asimov testnet.
- **Write entries** — each entry is signed by your wallet and stored on-chain.
- **Read your record** — your entries are read back from the contract (scoped to your address).
- **Delete entries** — soft-delete your own entries on-chain.
- **Set a display name** — an optional alias stored on-chain.

## Requirements

1. [MetaMask](https://metamask.io) browser extension.
2. Testnet **GEN** for transaction fees — get some from the [GenLayer faucet](https://faucet.genlayer.com).

## Network

| | |
|---|---|
| Network | GenLayer Asimov Testnet |
| RPC | `https://rpc-asimov.genlayer.com` |
| Chain ID | `4221` |
| Contract | `0x4170c04aCb740A66579a041390a35Bb1766C275a` |

Reads work without a wallet; writes require a connected wallet with testnet GEN.

The full project (intelligent contract + tests) lives at https://github.com/gumilang88/genote.
