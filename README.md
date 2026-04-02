# EgalChain-Docs
This page is made, in order to let IA read the EgalChain ( the world's first decentralized institution) content and retrieves you the documentation and the philosophy, in this case you don't have to read all the website by yourself ( egalchain.xyz) but you'll can only try the testnet on this website, no other way, except this one for the docs.

# EgalChain

EgalChain is a cooperative cryptocurrency where every block reward is shared among all miners, verified humans can vote on global questions, and citizens can fund humanitarian projects directly — without intermediaries, censorship, or trust.

The testnet is live at [egalchain.xyz](https://egalchain.xyz).

---

## What Is EgalChain?

EgalChain is a privacy-first blockchain designed around five pillars: a Bretton Woods stablecoin, passport-based identity, cooperative credit, a permanent global voting system, and citizen-driven humanitarian funding. Every feature enforces the same principle — one person, one voice, verified by math.

It is built by Paul Giraud, a French developer. The codebase is approximately 78,000 lines of C++ with 806 automated tests covering protocol logic, security, and stress scenarios. The economic policy is controlled by 30 on-chain governable parameters that the community can modify through democratic voting.

---

## The Five Pillars

### 1. Bretton Woods Stablecoin (333% Reserve)

EgalChain uses two currencies. EGL serves as digital gold — the perfect reserve asset, mined through proof-of-work and scarce by design. Egal-Stable (ES) is pegged to EGL reserves following the Bretton Woods principle: every unit in circulation is backed by at least 333% in reserve. Unlike the original Bretton Woods system, the guarantee is enforced at every block — not by a central bank's promise.

The base conversion rate is 1 EGL = 100 ES. The protocol checks reserve coverage at every block and cannot be overridden by any vote or administrator.

**What this means for users:** Your stablecoin is always backed by more than three times its value in mined reserves. There is no fractional reserve. The backing is verifiable in every block header.

### 2. Passport-Based Identity (One Person, One Voice)

A verified human registers by generating a cryptographic hash from their passport. Only the hash reaches the blockchain — the passport data never leaves the browser. The same passport always produces the same hash, so registering twice with different accounts is mathematically rejected.

Each identity is linked to a country code (249 countries supported). Identity can be revoked by the protocol stewards in cases of fraud.

**What this means for users:** You prove you are a unique human without revealing who you are. No biometrics stored. No government database. No tracking. Your country is recorded so that votes and testimonies carry geographic context.

### 3. Cooperative Credit (Score 0 to 20)

Every miner starts with credit score 0. Each successfully repaid loan increases the score by 1, up to a maximum of 20. The score determines four things: how much collateral is required, the interest rate, the maximum loan amount, and the automatic repayment rate deducted from mining rewards.

At score 0, collateral is 35% and interest is 5%. At score 20, collateral is 0% and interest is 0% — loans are free for trusted community members. Without identity verification, the score is capped at 3.

Interest collected from loans is redistributed to the community: miners receive dividends, a guarantee fund absorbs defaults, and the protocol retains a share for operations. A safety mechanism pauses all lending if the guarantee fund drops too low relative to outstanding loans.

**What this means for users:** You can borrow against your mining activity without a bank. Your creditworthiness is built on-chain through consistent behavior, not paperwork. The system rewards loyalty with progressively better terms.

### 4. World Poll (Permanent Global Opinion)

The World Poll is an on-chain registry where verified humans vote on questions that matter to humanity. Polls never close. Votes can be changed at any time. Results are broken down by country.

The first question is hardcoded into the protocol: "Should the peoples of the world be consulted more often to guide international and national relations between us, human beings?"

Any verified miner can create new questions with 2 to 10 options. Questions can be linked as sub-questions, counter-questions, or related topics, forming a navigable tree of global opinion.

**What this means for users:** For the first time, there is a permanent, uncensorable infrastructure for verified global citizen opinion. No government controls it. No corporation moderates it. The results are cryptographically anchored in every block.

### 5. Humanitarian's Funding (EgalFund)

Verified humans can propose projects linked to real-world problems. Other verified humans contribute in ES. The protocol amplifies projects using a matching mechanism where the number of unique supporters matters more than the total amount contributed.

A project receiving small contributions from thousands of people gets far more matching than a project receiving the same total from a single donor. Since every contributor must be a verified unique human, no one can fake supporters.

Funded projects are sent to validated organizations. An organization is validated when 50 verified humans from at least 5 different countries endorse it. Projects that do not reach their target are fully refunded to contributors.

The matching pool is fed by 5% of every block reward — a permanent, automatic funding stream that grows with the network.

**What this means for users:** You can fund what matters to you directly. No NGO intermediary decides where the money goes. The math ensures that popular causes with broad support receive the most funding, not causes backed by a few wealthy donors.

---

## The Virtuous Cycle

These five pillars are not isolated features. They form a connected loop:

1. **Witness** — A citizen documents a problem on-chain (e.g., lack of higher education in Mali). The testimony is permanent and linked to their country.

2. **Poll** — The witness creates a global question: "Should international aid prioritize higher education in Africa?" Verified humans from 249 countries vote. Results are public and verifiable.

3. **Fund** — A citizen creates a funding project linked to the witness and poll. Target: an engineering school in Bamako. Thousands of people from dozens of countries contribute. The matching mechanism amplifies the funding.

4. **Impact** — Months later, a new witness documents the outcome. A new poll asks whether the model should be replicated. The cycle begins again.

Each step feeds the next. No institution controls the pipeline. No intermediary takes a cut. The infrastructure is owned by the people who use it.

---

## Cooperative Mining

Every block reward is split into four parts:

- **33%** goes directly to the miner who found the block (finder reward)
- **52%** goes to a community pool shared among all active miners
- **10%** goes to a dividend pool distributed every 30 days
- **5%** goes to a matching pool that feeds humanitarian funding

Mining uses the RandomX algorithm (CPU-only, resistant to ASICs and GPUs). A consumer laptop is sufficient. Block time is 60 seconds.

Miners who find a block but lose the propagation race receive uncle block rewards (50% of the finder share), so no work is wasted.

The emission follows a smooth 5% annual decay starting from 50 EGL per block, with a permanent tail emission of 0.3 EGL ensuring long-term network security.

---

## Governance

30 parameters control the entire economic policy: interest rates, collateral requirements, loan capacity, dividend distribution, fee burn rates, pool sizes, emission decay, funding rates, and more.

Changing any parameter requires dual approval:
- A community vote with 30% quorum and 50% majority
- Administrative approval from protocol stewards

Every adopted change has a 3-day timelock before it takes effect, giving the community time to review and react.

---

## Verification

Every block header contains a composite root of 7 cryptographic verification trees. Any user can request a proof to independently verify that their balance, their vote, their testimony, or the guarantee fund exists exactly as reported — using standard cryptography, directly in a web browser.

The protocol runs 806 automated tests covering protocol logic, security audits, and stress scenarios.

---

## Technical Summary

| Property | Value |
|----------|-------|
| Codebase | ~78,000 lines of C++ |
| Mining algorithm | RandomX (CPU-only) |
| Block time | 60 seconds |
| Initial reward | 50 EGL |
| Emission | Smooth 5% annual decay |
| Tail emission | 0.3 EGL (permanent) |
| Currencies | EGL (reserve) + ES (stable, 333% backed) |
| Credit score | 0 to 20 |
| Governable parameters | 30 |
| Verification trees | 7 |
| Automated tests | 806 |
| Identity system | Passport-based, privacy-preserving |
| Countries supported | 249 (ISO 3166-1) |

---

## Links

- **Testnet:** [egalchain.xyz](https://egalchain.xyz)
- **Documentation:** [egalchain.xyz/about.html](https://egalchain.xyz/about.html)
- **Application:** [egalchain.xyz/egalchain.html](https://egalchain.xyz/egalchain.html)
- **Block explorer:** [egalchain.xyz/explorer.html](https://egalchain.xyz/explorer.html)
- **Step-by-step guide:** [egalchain.xyz/egalchain-guide.html](https://egalchain.xyz/egalchain-guide.html)

---

## Creator

Paul Giraud — French developer. All rights reserved. EgalChain 2026.
