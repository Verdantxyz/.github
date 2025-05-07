# Verdant Lens Whitepaper

## Abstract

**Verdant Lens** is a decentralized platform enabling creators on the Lens ecosystem to launch their own personalized tokens through a reputation-gated system. By leveraging bonding curve mechanisms and progressive liquidity migration to Uniswap V2, creators and their communities can participate in economic, reputational, and social growth in a sustainable and gamified way.

---

## 1. Introduction

In the Lens ecosystem, reputation and influence are key drivers of value. **Verdant Lens** empowers top creators to tokenize their presence, letting their supporters back them financially while gaining exclusive access to their communities and rewards.

Verdant Lens introduces:

- A **reputation-gated token launcher**: only users with a Lens Reputation Score > 700 can create tokens.
- A **bonding curve mechanism** to bootstrap liquidity.
- An automatic **migration to Uniswap V2** once liquidity thresholds are met.
- An integrated **XP system** rewarding participants for supporting creators.

---

## 2. Use Cases

Why would someone buy a creator’s token?

- **Support**: Backing a creator you believe in.
- **Exclusive access**: Token holders can join private groups or channels managed by the creator.
- **Potential appreciation**: Early buyers benefit as token demand grows.
- **Fee-sharing in Uniswap V2**: Once migrated, token holders can provide liquidity in Uniswap V2 and earn trading fees.
  
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

\[
P(s) = a \cdot \frac{1}{1 + e^{-b(s - c)}}
\]

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
