---
name: blockchain-audit-skill
description: >
  Blockchain protocol security audit reference skill. Use this skill whenever a user asks about:
  audited blockchain protocols, smart contract security track records, which DeFi/Web3 projects
  are safe or battle-tested, security ratings of crypto protocols, audit firm recommendations,
  exploit history of blockchain projects, or whether a specific project has been audited.
  Also trigger when users compare protocols by security, ask "is X safe?", "which protocols
  have never been hacked?", "what auditors did X use?", or "show me clean audit records."
  Always use this skill before answering any question about blockchain protocol security posture.
---

# Blockchain Audit Skill

A curated reference of blockchain protocols and projects with verified, successful audits
and **no known critical smart contract exploits** as of May 2026.

> ⚠️ "No exploit" means: no successful smart contract-level hack of the core protocol.
> Minor incidents (e.g., compromised external keys, post-audit governance bugs not classified
> as hacks, or off-chain issues) are noted where relevant. An audit does NOT guarantee future safety.

---

## How to Use This Skill

1. **Lookup**: Check `references/audited-projects.md` for a protocol by name or category.
2. **Assess**: Cross-reference audit firm tier, number of audits, and exploit history.
3. **Score**: Use the Security Score rubric below to rate a protocol's security posture.
4. **Report**: Summarize findings using the standard output format at the bottom of this file.

---

## Audit Firm Tiers

| Tier | Firms |
|------|-------|
| **Tier 1** (highest rigor) | Trail of Bits, OpenZeppelin, ConsenSys Diligence, Sigma Prime |
| **Tier 2** (highly respected) | Zellic, Spearbit/Cantina, Halborn, Quantstamp, ChainSecurity, Runtime Verification |
| **Tier 3** (reputable) | CertiK, Hacken, PeckShield, SlowMist, Cyfrin, QuillAudits |

More audit firms = stronger signal. Cross-tier audits (e.g., Tier 1 + Tier 2) are the gold standard.

---

## Security Score Rubric (0–100)

| Factor | Max Points | Notes |
|--------|-----------|-------|
| Number of audits | 20 | 1–2 = 10pts, 3–5 = 15pts, 6+ = 20pts |
| Audit firm tier | 20 | Tier 1 only = 20pts, Tier 1+2 = 18pts, Tier 2 only = 12pts, Tier 3 only = 6pts |
| Years exploit-free | 20 | 1yr = 8pts, 2yr = 12pts, 3yr = 16pts, 4yr+ = 20pts |
| TVL/usage track record | 15 | High TVL + long history = max |
| Bug bounty program | 10 | Active program = 10pts |
| Formal verification | 10 | Proven FV = 10pts, partial = 5pts |
| Open source & transparency | 5 | Fully open source = 5pts |

**Score Guide**: 85–100 = Excellent | 70–84 = Strong | 50–69 = Moderate | <50 = Caution

---

## Reference File

→ See `references/audited-projects.md` for the full curated project list organized by category.

---

## Standard Output Format

When reporting on a protocol's security posture, use this structure:

```
## [Protocol Name] — Security Posture

**Category**: DEX / Lending / Oracle / L1 / Bridge / etc.
**Chain(s)**: Ethereum, Solana, etc.

### Audit Record
| Firm | Year | Report Link |
|------|------|-------------|
| ...  | ...  | ...         |

### Exploit History
- ✅ No critical smart contract exploits as of [date]
- ⚠️ [Note any minor incidents if applicable]

### Security Score: XX/100
[Brief justification]

### Verdict
[1–2 sentence summary for the user]
```

---

## Key Principles When Answering

- Never claim a protocol is "100% safe" — audits reduce risk, they don't eliminate it.
- Always note the date of last audit vs. last major code change (stale audits lose value).
- Distinguish between *core protocol exploits* vs. *peripheral/integration exploits*.
- When a protocol has been exploited post-audit, flag it clearly — do NOT include in the clean list.
- If a user asks about a protocol not in the reference list, reason from first principles and note the gap.
