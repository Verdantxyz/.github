# Verdant Lens Whitepaper

## Abstract

Verdant is a decentralized launchpad that empowers reputable creators within the Lens ecosystem to issue their own community tokens, backed by a sigmoid bonding curve and a transparent path to liquidity. By leveraging social reputation as a gating mechanism, Verdant fosters sustainable, trust-based token economies where ownership unlocks access, participation, and shared upside. Minting is powered by GHO, Lens Chain’s native stablecoin, and every interaction contributes to a gamified XP system that incentivizes community growth.

---

## 1. Introduction

The creator economy in Web3 lacks tools for credible creators to launch tokens without speculative dynamics or predatory structures. Verdant addresses this gap by combining on-chain reputation, bonding curve mechanics, and community incentives to offer a launchpad tailored for Lens-native creators.

Unlike typical permissionless launchpads, Verdant **requires a Lens Score ≥700** to be eligible to launch a token, ensuring each creator has proven credibility and sustained contribution to the ecosystem.

Verdant differentiates itself by aligning social reputation, progressive liquidity, and community utility, positioning tokens not just as tradable assets, but as **keys to social and participatory privileges**.

---

## 2. Why Verdant

Verdant stands apart from other launchpads through several key differentiators:

- **Reputation-Gated Access**: Launches are exclusive to creators with a Lens Score ≥700, ensuring trusted, active participants.
- **Sigmoid Bonding Curve Pricing**: Tokens are minted along a sigmoid curve, providing fair early pricing and progressive increase based on demand.
- **Social Utility First**: Tokens grant access to exclusive communities, content, or governance, with liquidity as an optional next step.
- **Progressive Liquidity Path**: Once token liquidity reaches a predefined threshold, the token can migrate to Uniswap V2 pools for broader trading and fee earning.
- **GHO-Powered Minting**: Minting requires GHO, ensuring stable inflows and reinforcing Lens Chain’s economy.
- **Gamified Incentives**: Users earn XP for minting, swapping, or providing liquidity, fostering continuous engagement.

Verdant redefines token launches as **socially-aligned, reputation-backed, and utility-driven**, rather than purely speculative.

---

## 3. Token Creation

### 3.1 Eligibility

Only Lens users with a **Reputation Score ≥ 700** can launch their own token.

Each creator token:

- Is minted through a **sigmoidal bonding curve**.
- Uses **GHO (native stablecoin of Lens Chain)** as the base currency.
- Has a supply dynamically minted by buyers along the bonding curve.

### 3.2 Price Mechanism

The token price follows a **sigmoid bonding curve**:

$$ P(s) = \frac{a}{1 + e^{-b(s - c)}} $$

Where:
- \(P(s)\): price at supply \(s\)
- \(a\): price scaling factor
- \(b\): steepness
- \(c\): midpoint

Early tokens are cheaper; price accelerates with supply.

**All purchases are made in GHO.** Collected GHO is locked in the bonding curve contract to back liquidity.

---

## 4. Migration to Uniswap V2

Once a creator's token reaches a preset liquidity threshold (e.g., **5,000 GHO locked**), it is:

1. Migrated automatically to a **Uniswap V2 pool (TOKEN/GHO)**.
2. Uses locked GHO and corresponding token supply as initial liquidity.
3. Allows public trading and liquidity provision by users.

### 💡 Key difference:

During the bonding curve phase:
- Buy/sell interacts directly with the curve contract.

After migration:
- Buy/sell happens via **Uniswap V2 AMM**, enabling fee-sharing for LPs.

---

## 5. Incentives & Rewards

### 5.1 Why buy a token?

✅ Support a creator  
✅ Gain **access to exclusive groups/channels**  
✅ Benefit from early price appreciation  
✅ Become eligible to provide liquidity and earn **Uniswap fees**

---

### 5.2 Rewards for creators

- **No commission on bonding curve purchases** → 100% of GHO stays in liquidity → preserves price integrity.
- Creator receives an **initial allocation of tokens** (e.g., 10-20% reserved at genesis) for:
  - Adding liquidity to Uniswap
  - Selling gradually
  - Incentivizing community (airdrops, giveaways)

---

### 5.3 Rewards for holders

- Earn **XP** for holding creator tokens.
- Access to **creator’s private groups**.
- Optionally participate in **future governance** if enabled.
- **Eligible to provide liquidity** on Uniswap after migration → earn trading fees.

| Action                   | XP Earned                |
|-------------------------|-------------------------|
| Buy tokens               | +2 XP per 100 GHO       |
| Swap (buy/sell)          | +1 XP per swap          |
| Provide Liquidity        | +5 XP per 100 GHO added |
| Hold tokens              | +1 XP per day per 100 tokens |

---

## 6. Tokenomics

| Parameter                    | Value (example)        |
|-----------------------------|-----------------------|
| Base currency                | GHO                   |
| Bonding curve formula        | Sigmoid               |
| Creator initial allocation    | 10-20% of total       |
| Liquidity migration threshold | 5,000 GHO locked     |
| Post-migration AMM           | Uniswap V2 (TOKEN/GHO)|

✅ No direct fee on bonding curve purchases (all funds locked as liquidity).  
✅ Sustainable liquidity bootstrap → smooth transition to public market.

---

## 7. Risks & Mitigations

| Risk                                 | Mitigation                              |
|-------------------------------------|----------------------------------------|
| Low token demand                     | Launch gated by reputation threshold    |
| Creator sells all tokens post-launch | Vesting/vesting recommendations        |
| Lack of utility                      | Incentivized exclusive access + XP      |
| Rugpull fear                         | GHO locked in bonding curve → verifiable |

---

## 8. Conclusion

**Verdant Lens** empowers reputable creators to tokenize their influence in a transparent, community-aligned, and gamified system. Supporters gain social, economic, and access-based benefits, while creators build sustainable token economies tied to their reputation.

---

## 9. Future Directions

- DAO governance for creator communities
- Cross-token collaboration between creators
- NFT perks linked to holding tokens
- Integration with Lens-based dApps

---

Verdant Lens: growing value, one connection at a time 🌱
