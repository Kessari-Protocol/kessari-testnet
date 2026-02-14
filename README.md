# kessari-testnet
kessari-testnet — Public test network configuration and tooling for the Kessari protocol. Allows developers to run nodes, deploy applications, and experiment with transactions safely before mainnet release.

# kessari-testnet

Public test network configuration for the Kessari protocol.

The testnet allows developers to run nodes, submit transactions, and integrate applications without risking real value.

This environment exists for experimentation, integration development, and protocol validation prior to mainnet release.

---

## Purpose

The testnet provides:

- a stable development endpoint
- transaction experimentation
- integration testing
- node compatibility verification
- protocol behavior observation

No economic guarantees exist in this network.

---

## Default Endpoint


Local node endpoint:
http://localhost:7070/

---

## Connecting via SDK (JavaScript)

```js
import { KessariClient } from "@kessari/sdk"

const client = new KessariClient("https://testnet.kessari.network")
use kessari_sdk::Client;

let client = Client::new("https://testnet.kessari.network");
```
## Connecting via SDK (Rust)

```rust
use kessari_sdk::Client;

let client = Client::new("https://testnet.kessari.network");
```
## Running a Local Test Node

```bash
git clone https://github.com/kessari-protocol/kessari-node
cd kessari-node
cargo run
```
## The node will expose a local RPC endpoint on port 7070.

## Faucet

A public faucet will be available in future testnet phases.

Until then, transactions operate in a zero-value environment.

---

## Intended Use

Use this network to:

- test integrations
- debug transactions
- validate application logic
- explore protocol behavior

Do not treat testnet behavior as final mainnet guarantees.

---

## Documentation

Protocol specification:  
https://github.com/kessari-protocol/kessari-docs

---

## Status

Active development test network.

Network resets may occur without notice.
