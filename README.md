# roadchain.io

> RoadChain — a Layer-1 blockchain built from scratch in Python.

**Live at [https://roadchain.io](https://roadchain.io)**

## What RoadChain Is

RoadChain is a Layer-1 blockchain written entirely in Python. No forks, no frameworks, no Solidity. Every component — consensus, cryptography, wallet, mining — is built from first principles.

## Technical Details

- **Cryptography** — secp256k1 ECDSA signatures (same curve as Bitcoin)
- **Hashing** — SHA-256 Proof of Work
- **Block structure** — Merkle trees for transaction verification
- **Wallet CLI** — generate keys, sign transactions, check balances from the terminal
- **P2P networking** — node discovery and block propagation
- **Chain validation** — full chain integrity checks on every block

## Why From Scratch

Most "blockchain projects" are Ethereum forks with a new token. RoadChain is the opposite — every line of code is written to understand and implement the actual cryptographic primitives. secp256k1 elliptic curve math, SHA-256 mining loops, Merkle root computation, UTXO tracking. If you want to learn how blockchains actually work, read this codebase.

## Architecture

- **Language**: Python (no C extensions, no Rust FFI — pure Python for readability)
- **Consensus**: Proof of Work (SHA-256, adjustable difficulty)
- **Signatures**: ECDSA on secp256k1
- **Storage**: JSON chain files (portable, inspectable)
- **Site**: served from Gematria (Caddy TLS)

## Running a Node

```bash
python3 roadchain.py          # Start a node
python3 wallet.py generate    # Create a new wallet
python3 wallet.py balance     # Check balance
python3 miner.py              # Start mining
```

## Part of BlackRoad OS

BlackRoad OS, Inc. (Delaware C-Corp, est. November 2025)
See [blackroad.io](https://blackroad.io) for the full platform.

## License

**PROPRIETARY** — BlackRoad OS, Inc. All rights reserved.

---

*BlackRoad OS — Remember the Road. Pave Tomorrow.*
