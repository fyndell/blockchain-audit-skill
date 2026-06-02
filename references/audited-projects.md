# Audited Blockchain Projects — Clean Security Record Reference
*Last updated: June 2026 (auto-updated)*

---

## Table of Contents
1. [Decentralized Exchanges (DEX)](#1-decentralized-exchanges-dex)
2. [Lending & Borrowing Protocols](#2-lending--borrowing-protocols)
3. [Oracle Networks](#3-oracle-networks)
4. [Staking & Liquid Staking](#4-staking--liquid-staking)
5. [Layer 1 Blockchains & Consensus Clients](#5-layer-1-blockchains--consensus-clients)
6. [Layer 2 / Rollups](#6-layer-2--rollups)
7. [Infrastructure & Tooling](#7-infrastructure--tooling)
8. [Asset Management & Yield](#8-asset-management--yield)
9. [Governance & DAOs](#9-governance--daos)
10. [Privacy Protocols](#10-privacy-protocols)
11. [Multisig & Account Infrastructure](#11-multisig--account-infrastructure)

---

## 1. Decentralized Exchanges (DEX)

### Uniswap v2 / v3 / v4
- **Chain**: Ethereum + multi-chain
- **Auditors**: OpenZeppelin (v4 core, periphery, universal router), Trail of Bits, ABDK
- **Audits**: 9+ audits for v4 alone; $2.35M competitive security contest; $15.5M bug bounty
- **Exploit Record**: ✅ Uniswap v2 and v3 facilitated **465M+ swaps with zero hacks or exploits**. No critical bugs found in v4 security competition or bug bounty.
- **Audit Reports**: https://github.com/Uniswap/v4-core/tree/main/audits
- **Score**: ~95/100
- **Notes**: Most battle-tested DEX protocol in DeFi history.

### 1inch
- **Chain**: Multi-chain (Ethereum, BNB, Polygon, etc.)
- **Auditors**: OpenZeppelin (13+ audits), others
- **Exploit Record**: ✅ No critical core protocol exploits. Launched Fusion swaps in 2025 to eliminate front-running.
- **Score**: ~82/100

### SushiSwap (Core Contracts)
- **Chain**: Multi-chain
- **Auditors**: Zellic, PeckShield, others
- **Exploit Record**: ✅ Core AMM contracts have not been exploited. (Note: The 2021 RouteProcessor2 incident was a peripheral contract added post-audit, not the core AMM.)
- **Score**: ~72/100
- **Notes**: Only count the core AMM — peripheral/routing contracts have had issues.

### PancakeSwap (Core)
- **Chain**: BNB Chain, zkSync, Linea
- **Auditors**: CertiK, Hacken, PeckShield
- **Exploit Record**: ✅ Core contracts exploit-free. Top DEX on BNB Chain.
- **Score**: ~70/100

---

## 2. Lending & Borrowing Protocols

### Aave (v1 / v2 / v3 Core)
- **Chain**: Ethereum + multi-chain
- **Auditors**: OpenZeppelin (multiple), Trail of Bits, CertiK, SigmaPrime, others
- **Exploit Record**: ✅ Core smart contracts have not been successfully exploited. One governance-related bad debt event (CRV short position, 2023) was an economic design issue, not a smart contract hack.
- **Audit Reports**: https://github.com/aave/aave-v3-core/tree/master/audits
- **Score**: ~90/100
- **Notes**: 94% of top 20 DeFi protocols use OpenZeppelin Contracts, which Aave's foundation relies on.

### Compound (v2 Core)
- **Chain**: Ethereum
- **Auditors**: OpenZeppelin (multiple), Trail of Bits
- **Exploit Record**: ✅ No smart contract hack. A 2021 COMP distribution bug (over-distributed COMP due to a governance proposal) was a configuration error, not an exploit by an attacker.
- **Audit Reports**: https://compound.finance/docs/security
- **Score**: ~85/100

### MakerDAO / Sky (DAI / Core Contracts)
- **Chain**: Ethereum
- **Auditors**: Trail of Bits, OpenZeppelin, Runtime Verification, others
- **Exploit Record**: ✅ Core contracts never exploited since 2017. One of the longest clean records in DeFi.
- **Score**: ~92/100
- **Notes**: The March 2020 Black Thursday liquidation was a market crisis, not an exploit.

### Morpho (Core)
- **Chain**: Ethereum
- **Auditors**: OpenZeppelin (Morpho Blue audit), Spearbit, Trail of Bits
- **Exploit Record**: ✅ No core protocol exploits.
- **Score**: ~84/100

### Spark (MakerDAO's lending arm)
- **Chain**: Ethereum
- **Auditors**: Inherited from MakerDAO audits + independent audits
- **Exploit Record**: ✅ No exploits.
- **Score**: ~80/100

---

## 3. Oracle Networks

### Chainlink
- **Chain**: Multi-chain (80%+ DeFi oracle market share)
- **Auditors**: Trail of Bits, OpenZeppelin, multiple others; continuously audited
- **Exploit Record**: ✅ Core oracle network has never been successfully exploited. Chainlink itself has been time-tested on mainnet securing billions in DeFi (Aave, Synthetix, Compound, etc.)
- **Score**: ~93/100
- **Notes**: Many DeFi hacks involve *misuse* of Chainlink price feeds (e.g., TWAP issues in integrations) — this is an integration issue, NOT a Chainlink exploit.

### UMA Protocol
- **Chain**: Ethereum + multi-chain
- **Auditors**: OpenZeppelin (10+ audits as primary security partner)
- **Exploit Record**: ✅ No critical exploits of core optimistic verification system.
- **Score**: ~81/100

---

## 4. Staking & Liquid Staking

### Lido (Core Contracts)
- **Chain**: Ethereum
- **Auditors**: Multiple (Sigma Prime, MixBytes, Oxorio, others)
- **Exploit Record**: ✅ Core staking contracts have not been exploited. A May 2025 incident involved 1.46 ETH in gas fees lost due to a compromised oracle key from 2021 — **no user funds were affected**. The 5-of-9 quorum mechanism protected the system.
- **Score**: ~85/100
- **Notes**: Secures 25%+ of all staked ETH. Oracle key rotation was completed after the 2025 incident.

### EigenLayer
- **Chain**: Ethereum
- **Auditors**: Multiple; heavily audited as one of the most scrutinized newer protocols
- **Exploit Record**: ✅ No core protocol exploits as of mid-2026.
- **Score**: ~78/100
- **Notes**: Newer protocol — track record still maturing.

---

## 5. Layer 1 Blockchains & Consensus Clients

### Ethereum 2.0 / Beacon Chain
- **Auditors**: Trail of Bits, Quantstamp, Sigma Prime (Lighthouse client), ConsenSys Diligence, others
- **Exploit Record**: ✅ No successful attacks on the consensus layer since the Merge (2022).
- **Score**: ~96/100

### Algorand
- **Auditors**: Trail of Bits
- **Exploit Record**: ✅ No known core protocol exploits.
- **Score**: ~82/100

### Solana Foundation (Core Protocol)
- **Auditors**: Zellic, Halborn, Neodyme, others
- **Exploit Record**: ✅ Core Solana protocol has not been exploited. (Various Solana-based dApps have been hacked — these are application-layer, not protocol-layer.)
- **Score**: ~80/100

---

## 6. Layer 2 / Rollups

### Arbitrum (Core Bridge & Rollup Contracts)
- **Chain**: Ethereum L2
- **Auditors**: Trail of Bits, OpenZeppelin, others
- **Exploit Record**: ✅ No successful exploit of core bridge or rollup contracts.
- **Score**: ~85/100

### Optimism (Core Contracts)
- **Chain**: Ethereum L2
- **Auditors**: OpenZeppelin, Trail of Bits, Zeppelin
- **Exploit Record**: ✅ No successful exploit of core contracts. (A 2022 bug was found and patched by white-hat researchers before exploitation.)
- **Score**: ~84/100

### ZKsync (Core)
- **Chain**: Ethereum L2
- **Auditors**: Cyfrin, Trail of Bits (Starknet assessed separately), others
- **Exploit Record**: ✅ No exploits of core zkEVM contracts. (A May 2025 airdrop contract administrative error was resolved and not a hack.)
- **Score**: ~80/100

---

## 7. Infrastructure & Tooling

### OpenZeppelin Contracts Library
- **Auditors**: Self-audited + community + used by OpenZeppelin audit team
- **Exploit Record**: ✅ The library itself has not been exploited; it is used to *prevent* exploits. Over $35T in total onchain value transferred using OZ Contracts.
- **Score**: ~97/100
- **Notes**: The industry standard for secure Solidity development.

### Across Protocol
- **Chain**: Multi-chain bridge
- **Auditors**: OpenZeppelin (OFT Integration audit, 2025), others
- **Exploit Record**: ✅ No core protocol exploits.
- **Score**: ~78/100

### LayerZero (Core Messaging)
- **Chain**: Multi-chain
- **Auditors**: Multiple; ongoing audits
- **Exploit Record**: ✅ Core messaging protocol has not been exploited. (Specific integrations using LayerZero have had issues.)
- **Score**: ~78/100

---

## 8. Asset Management & Yield

### Synthetix (Core Contracts)
- **Chain**: Ethereum, Optimism
- **Auditors**: OpenZeppelin (multiple), others
- **Exploit Record**: ✅ Core smart contracts have not been exploited.
- **Score**: ~82/100

### Pendle Finance
- **Chain**: Ethereum + multi-chain
- **Auditors**: Multiple audits
- **Exploit Record**: ✅ No critical core exploits.
- **Score**: ~76/100

---

## 9. Governance & DAOs

### Gnosis Safe (Core)
- **Chain**: Multi-chain
- **Auditors**: Multiple independent audits
- **Exploit Record**: ✅ The Safe multisig smart contract itself has not been exploited. (The Bybit $1.5B hack in 2025 was a frontend/social engineering attack on Safe's UI, NOT the smart contract.)
- **Score**: ~90/100
- **Notes**: The #1 multisig by TVL and usage. Core contract security is exemplary.

---

## 10. Privacy Protocols

### Zcash (Core Protocol)
- **Chain**: Standalone L1
- **Auditors**: Trail of Bits, others
- **Exploit Record**: ✅ No known exploits of the core Zcash protocol or zk-SNARK implementation.
- **Score**: ~85/100

---

## 11. Multisig & Account Infrastructure

### Squads Protocol v4 (Solana)
- **Chain**: Solana
- **Auditors**: Trail of Bits (2023 audit of v4)
- **Exploit Record**: ✅ No exploits of core multisig contracts.
- **Audit Report**: https://squads.xyz/blog/trail-of-bits-security-audit-v4
- **Score**: ~80/100

### Drift Protocol (Solana)
- **Chain**: Solana
- **Auditors**: Trail of Bits (2022 DEX audit, no high-severity findings)
- **Exploit Record**: ✅ No critical smart contract exploits.
- **Score**: ~78/100

---

## ❌ Notable Exclusions (Audited BUT Exploited)

These were audited by reputable firms but still suffered significant exploits.
Do NOT include in clean-record assessments:

| Protocol | Exploit | Loss | Auditor(s) |
|----------|---------|------|-----------|
| Curve Finance (pools) | Vyper compiler bug (2023) | ~$70M | Multiple |
| Ronin Bridge | Compromised validator keys (2022) | $625M | CertiK |
| Wormhole | Smart contract bug (2022) | $320M | Multiple |
| Nomad Bridge | Merkle tree bug (2022) | $190M | Quantstamp |
| Rari Capital | Reentrancy (2022) | $80M | Quantstamp |
| Alpha Finance | Flash loan (2021) | $37M | Quantstamp |
| MonoX | Price manipulation (2021) | $31M | CertiK |
| Beanstalk | Governance attack (2022) | $182M | Halborn |
| Poly Network | Private key/logic (2021) | $611M | Multiple |
| THORChain | Multiple incidents | $8M+ | Halborn |
| Gnosis Pay | Smart contract exploit (2026-06-01) | Unknown | Multiple |
| Yearn Finance | Strategy exploit (2023) | $11M | Multiple |

> 🔑 Key lesson: Even Tier 1 auditors cannot guarantee zero exploits. Scope, timing, and coverage all matter.

---

## Quick Lookup Table

| Protocol | Category | Top Auditor | Audits | Exploit-Free | Score |
|----------|----------|-------------|--------|--------------|-------|
| Uniswap v2/v3/v4 | DEX | OpenZeppelin | 9+ | ✅ Yes | 95 |
| MakerDAO/Sky | Stablecoin/CDP | Trail of Bits | 5+ | ✅ Yes | 92 |
| Chainlink | Oracle | Trail of Bits | 5+ | ✅ Yes | 93 |
| Aave v3 | Lending | OpenZeppelin | 6+ | ✅ Yes | 90 |
| Gnosis Safe | Multisig | Multiple | 4+ | ✅ Yes | 90 |
| Ethereum Beacon | L1 Consensus | Sigma Prime | 4+ | ✅ Yes | 96 |
| Compound v2 | Lending | OpenZeppelin | 4+ | ✅ Yes* | 85 |
| Lido | Liquid Staking | Sigma Prime | 4+ | ✅ Yes** | 85 |
| Zcash | L1 Privacy | Trail of Bits | 2+ | ✅ Yes | 85 |
| Morpho | Lending | OpenZeppelin | 3+ | ✅ Yes | 84 |
| Arbitrum | L2 | Trail of Bits | 3+ | ✅ Yes | 85 |
| Optimism | L2 | OpenZeppelin | 3+ | ✅ Yes | 84 |
| 1inch | DEX Agg | OpenZeppelin | 13+ | ✅ Yes | 82 |
| Synthetix | Derivatives | OpenZeppelin | 3+ | ✅ Yes | 82 |
| Algorand | L1 | Trail of Bits | 2+ | ✅ Yes | 82 |
| Squads v4 | Multisig (SOL) | Trail of Bits | 1+ | ✅ Yes | 80 |

*COMP distribution bug 2021 was not an attacker exploit
**1.46 ETH gas loss in 2025 — no user funds affected
