# 🔐 Blockchain Audit Skill for Claude

A Claude skill that tracks audited blockchain protocols with clean security records — **no critical smart contract exploits**.

## What It Does
- ✅ References 16+ exploit-free protocols across 11 categories (DEX, Lending, Oracle, L1, L2, etc.)
- 📊 Scores protocol security on a **0–100 rubric** (auditor tier, audit count, years clean, TVL, bug bounty, formal verification)
- ❌ Flags audited projects that were still exploited (Curve, Wormhole, Ronin, Nomad, etc.)
- 📋 Generates standardized security posture reports

## Protocols Covered (highlights)

| Protocol | Score | Category |
|----------|-------|----------|
| Ethereum Beacon Chain | 96/100 | L1 Consensus |
| OpenZeppelin Contracts | 97/100 | Library |
| Uniswap v2/v3/v4 | 95/100 | DEX |
| Chainlink | 93/100 | Oracle |
| MakerDAO/Sky | 92/100 | Stablecoin |
| Aave v3 | 90/100 | Lending |
| Gnosis Safe | 90/100 | Multisig |

## Audit Firms Referenced
- **Tier 1**: Trail of Bits, OpenZeppelin, ConsenSys Diligence, Sigma Prime
- **Tier 2**: Zellic, Spearbit/Cantina, Halborn, Quantstamp, ChainSecurity
- **Tier 3**: CertiK, Hacken, PeckShield, SlowMist, Cyfrin

## Install
Download `blockchain-audit-skill.skill` and upload it via **Claude → Settings → Skills → Upload Skill**.

## Files
```
blockchain-audit-skill/
├── README.md
├── blockchain-audit-skill.skill   ← Install this in Claude
├── SKILL.md                       ← Skill instructions
└── references/
    └── audited-projects.md        ← Full project database
```

## Usage
Once installed, Claude will use this skill automatically when you ask things like:
- *"Is Aave safe to use?"*
- *"Which protocols have never been hacked?"*
- *"What auditors reviewed Uniswap v4?"*
- *"Compare Chainlink vs Pyth on security"*

---
*Last updated: May 2026 | Built with Claude*
