# Zealous Swap Whitepaper

### The Premier Decentralized Exchange on Igra L2

Version 1.0

### Abstract

Zealous Swap is pioneering decentralized finance as the first DEX on Igra, Kaspa's Layer 2 scaling solution. Leveraging the battle-tested V2 AMM architecture, Zealous Swap introduces an innovative NFT-based fee tier system that rewards early adopters while maintaining deep liquidity—critical for a nascent ecosystem. This whitepaper outlines our strategic approach to solving the liquidity bootstrapping challenge while establishing sustainable financial infrastructure for the Igra ecosystem.

### 1. Introduction

Zealous Swap aims to be the cornerstone of decentralized trading on Igra L2, providing a secure, efficient, and user-friendly platform for token swaps and liquidity provision. Our mission is to build sustainable DeFi infrastructure that grows alongside the Igra ecosystem, focusing on deep liquidity, capital efficiency, and accessible user experience.

The launch of a new Layer 2 ecosystem presents unique challenges, including fragmented liquidity, user education, and achieving network effects. Zealous Swap addresses these challenges through thoughtful protocol design and innovative incentive mechanisms.

### 2. Technical Architecture: Why V2?

After careful consideration of the nascent Igra ecosystem, Zealous Swap has strategically chosen to implement the V2 AMM architecture for its initial deployment. This decision was guided by several key factors that prioritize ecosystem bootstrapping and user experience:

#### 2.1 Concentrated Liquidity in a Single Pool

- V2 architecture centralizes all liquidity for each trading pair in a single pool

- Avoids fragmentation across multiple fee tiers (as seen in V3)

- Results in deeper liquidity and reduced price impact for traders

- Critical for a new ecosystem where total liquidity may be limited initially

#### 2.2 Simplified Liquidity Provision

- Lower barrier to entry for liquidity providers

- No complex range setting or active management required

- Passive yield generation through a straightforward deposit model

- Encourages broader participation across the Igra community

#### 2.3 Scalability Path

- Establishes foundation for future protocol upgrades

- Allows for V3 implementation as ecosystem matures

- Enables smooth transition with minimal disruption to users

### 3. Innovative NFT-Based Fee Mechanism

Zealous Swap introduces a novel dual-fee system powered by exclusive membership NFTs, carefully designed to incentivize early adoption while maintaining the mathematical integrity of our liquidity pools.

#### 3.1 Mechanism Design

Limited Edition Membership NFTs: Only 505 NFTs will ever be minted

##### Tiered Fee Structure:

- NFT holders: 0.2% swap fee (33% discount)

- Standard users: 0.3% swap fee

##### Fee Distribution:

- Standard users: 0.25% to liquidity providers, 0.05% to protocol treasury

- NFT holders: 0.17% to liquidity providers, 0.03% to protocol treasury

#### 3.2 Mathematical Consistency

The NFT fee mechanism preserves the constant product formula (x * y = k) at the pool level while introducing user-specific fee tiers at the interface level. This approach ensures:

- All trades, regardless of fee tier, interact with the same underlying liquidity pool

- The constant product curve remains unchanged for price calculation

- Fee differentiation occurs at transaction execution rather than pool calculation

This implementation differs from V3's multi-tier pools, where liquidity is fragmented across separate pools with different fee settings. Instead, our approach maintains unified liquidity while still offering fee advantages to NFT holders.

#### 3.3 Fee Mechanics & Pool Integrity

The fee discount does not disrupt the V2 constant product formula. Fees are applied externally to the swap input:

- User submits a swap of Δx tokens

- Protocol deducts a fee (0.2% or 0.3%) from Δx

- Remaining Δx_net is used to compute output Δy via k

Thus, pool reserves (x, y) and k update identically regardless of user fee tier, preserving mathematical integrity.

#### 3.4 Fairness of the 0.3% Fee for Regular Traders

While the 0.3% fee applies to non-NFT holders, it remains competitive within the broader decentralized exchange landscape. Given the liquidity advantages of Zealous Swap, which ensures deeper liquidity pools and reduced slippage, regular traders still benefit from favorable trading conditions. Furthermore, the fee structure aligns with the standard fees seen across most decentralized exchanges, making it a fair and accessible option for traders not holding NFTs. The ecosystem’s design ensures that everyone—whether holding NFTs or not—can access a highly efficient trading platform without compromising fairness or usability.

### 4. Strategic Advantages of the NFT Fee System

#### 4.1 Accelerated Liquidity Bootstrapping

- Creates immediate value proposition for early supporters

- Drives initial acquisition of strategic users and liquidity providers

- Establishes protocol revenue streams from day one

#### 4.2 Enhanced Market Efficiency

- Enables privileged arbitrage opportunities for NFT holders

- Tightens spreads and reduces price dislocations across markets

- Improves overall market efficiency while maintaining unified liquidity

#### 4.3 Competitive Advantage for Strategic Traders

- Provides tangible fee advantages for high-frequency traders

- Attracts institutional and professional market makers

- Creates positive feedback loop between volume and liquidity

### 5. Economic Analysis: NFT Fee Impact

The 0.1% fee differential between NFT holders and standard users creates significant economic advantages, particularly for high-frequency traders and arbitrageurs.

| Trading Volume (Monthly) | Standard Fee Cost | NFT Holder Fee Cost | Monthly Savings | Annual Savings |
|--------------------------|-------------------|---------------------|-----------------|----------------|
| $100,000                 | $300              | $200                | $100            | $1,200         |
| $1,000,000               | $3,000            | $2,000              | $1,000          | $12,000        |
| $10,000,000              | $30,000           | $20,000             | $10,000         | $120,000       |

This cost advantage creates a natural price floor for NFT membership, as the value proposition becomes immediately apparent for traders exceeding certain monthly volumes. For professional market makers and arbitrageurs, NFT acquisition represents a strategic competitive advantage.

#### 5.1 Arbitrage Enhancement

The fee differential provides NFT holders with privileged arbitrage opportunities. When price discrepancies between Zealous Swap and external markets fall within the 0.1% fee differential, only NFT holders can profitably execute arbitrage trades, leading to:

- More efficient price discovery

- Tighter spreads across the ecosystem

- Enhanced trading volume through arbitrage activity

- Additional utility and demand for membership NFTs

#### 5.2 Economic Flywheel

- Early Adopters: NFT holders trade at lower costs, increasing volume and LP fee earnings

- Liquidity Growth: Higher LP rewards attract more providers, tightening spreads

- Arbitrageurs: Low fees and tight spreads attract arbitrage, improving price accuracy

- Scarcity-Driven Demand: Limited NFTs appreciate as utility grows, creating a self-reinforcing adoption loop

#### 5.3 Sustainability Analysis

- Protocol Revenue: Even with 50% of volume from NFT holders, effective fee averages 0.25%, ensuring sustainable revenue

- Volume Leverage: A 0.1% fee reduction can increase whale trading volume thus generating more fee for LPs

### 6. NFT Utility & Governance

The limited edition of 505 Zealous Swap NFTs will serve multiple functions within the ecosystem:

- Reduced trading fees (0.2% vs 0.3%)

- Participation in protocol governance (future implementation)

- Revenue sharing from protocol fees (future consideration)

- Token Airdrop (future consideration)

- Whitelist to any other platform we build

### 7. Benefits to the Igra Ecosystem

Zealous Swap plays a key role in supporting the growth of decentralized applications (dApps) on Igra by providing essential infrastructure, such as deep liquidity pools and reliable price oracles.

- Scalable Liquidity for dApp Integration: Zealous Swap’s deep liquidity pools offer the necessary foundation for seamless token swaps in other dApps. By reducing slippage and ensuring smooth transactions, these pools make it easier for developers to integrate token swapping functionalities into their applications.

- Reliable Price Oracles: Zealous Swap provides an accurate on-chain price oracle, using a time-weighted average price (TWAP) model. This ensures dApps have access to reliable, real-time price data, vital for use cases like lending, borrowing, and derivatives trading.

- Supporting Ecosystem Growth: By offering these services, Zealous Swap lays the foundation for future dApp developers on Igra, helping to create a sustainable and thriving DeFi ecosystem that attracts new projects to build on Igra’s scalable Layer 2 solution.

### 8. Protocol-Owned Liquidity

A portion of trading fees will be directed to protocol-owned liquidity initiatives, creating sustainable infrastructure for the Igra ecosystem. This approach ensures:

- Long-term protocol sustainability independent of mercenary liquidity

- Ability to support strategic trading pairs even with initially lower volume

- Protection against liquidity crises during market downturns

### 9. Conclusion

Zealous Swap represents the next evolution in decentralized exchange design, thoughtfully optimized for the emerging Igra L2 ecosystem. By implementing a strategic V2 architecture enhanced with innovative NFT-based fee mechanics, we create a platform that balances immediate usability with long-term sustainability.

Our approach prioritizes liquidity depth, user accessibility, and economic incentives that align all ecosystem participants. Through careful consideration of the unique challenges faced by emerging L2 networks, Zealous Swap is engineered to solve the liquidity cold-start problem while establishing the foundation for a thriving DeFi ecosystem on Igra.

As Igra grows, Zealous Swap will evolve alongside it, maintaining our commitment to providing premier decentralized trading infrastructure.

Join us in building the financial foundation of the Igra ecosystem.

### 10. Team

Zealous Swap is built by a dedicated team with experience in blockchain and decentralized finance. Led by Louis Saad and Ramy Lahoud, we are focused on creating a decentralized exchange that supports the growth of the Igra L2 ecosystem and Kaspa in general.

---

Disclaimer: This whitepaper is provided for informational purposes only and does not constitute financial advice or an offer to sell securities. Cryptocurrency trading involves significant risk. Users should conduct their own research before participating in any DeFi protocol.
