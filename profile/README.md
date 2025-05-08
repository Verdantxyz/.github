# Verdant: A Reputation-Gated Social Token Launchpad on Lens

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

## 3. Tokenomics

Each creator token follows these principles:

- **Total Supply**: Defined dynamically by the bonding curve’s capacity.
- **Initial Supply Allocation**: A portion of the token supply is allocated directly to the creator, enabling them to hold, distribute, or provide liquidity post-migration.
- **Minting Currency**: Users mint tokens by paying with GHO.
- **No Initial Liquidity Required**: Liquidity is progressively built through user minting; migration to Uniswap V2 occurs once a liquidity threshold is achieved.

---

## 4. Pricing Model

Verdant uses a **sigmoid bonding curve** to determine the token price as a function of circulating supply:

**Formula:**

![Sigmoid Bonding Curve Formula](A_digital_image_displays_the_sigmoid_curve_formula.png)

Where:

- `P(x)`: Price at supply `x`
- `L`: Maximum price limit
- `k`: Curve steepness
- `x₀`: Inflection point (mid-supply)

Example values for a balanced system:

| Variable | Value  |
|----------|--------|
| L        | 10 GHO |
| k        | 0.1    |
| x₀       | 500    |

This curve ensures fair early pricing, gradual increase, and price stabilization as supply grows.

---

## 5. User Incentives

### 5.1 Creator Incentives
- Direct allocation of an initial token supply for optional liquidity or treasury purposes.
- No upfront capital requirement to provide liquidity.
- Potential fee-sharing once liquidity is migrated to Uniswap V2.

### 5.2 Holder Incentives
- XP earned per token minted, swap performed, or liquidity provided.
- Access to creator’s gated communities (e.g., Discord roles, Telegram channels).
- Once migrated to Uniswap V2, holders may participate in liquidity pools and earn trading fees.

---

## 6. Use Cases

- Fans mint tokens to support their favorite creator while gaining access to private communities or exclusive perks.
- Creators leverage token ownership for content gating, voting mechanisms, or contributor roles.
- Holders can swap, provide liquidity, and earn XP across multiple creator tokens, building platform-wide reputation.

---

## 7. Migration to Uniswap V2

Tokens can migrate to a Uniswap V2 pool once an established liquidity threshold (defined per token) is reached. This enables broader trading, liquidity provision, and external market discovery.

During migration:
- The creator may contribute their allocated supply into the pool.
- Holders may provide liquidity and earn fees.
- The bonding curve mechanism halts further minting; pricing transitions to the open AMM.

---

## 8. Risks and Mitigations

| Risk                   | Mitigation                                     |
|-----------------------|------------------------------------------------|
| Low liquidity          | Gated migration until liquidity threshold met   |
| Low demand             | Reputation gating ensures initial interest base |
| Price volatility post-migration | Creator LP incentives, optional liquidity mining |

---

## 9. Conclusion

Verdant offers a **unique launchpad tailored to the Lens ecosystem**, prioritizing reputation, community alignment, and sustainable token economies. By gating access to credible creators, leveraging a sigmoid bonding curve, and rewarding participants through XP, Verdant builds an ecosystem of **social tokens with intrinsic community value**.

Verdant empowers creators not just to launch a token, but to **grow an interconnected, incentivized, and reputation-backed micro-economy** within the Lens network.

---

## 10. References

- Lens Protocol: https://lens.xyz
- Uniswap Docs: https://docs.uniswap.org
- GHO: https://aave.com/gho
