# Zealous Swap Whitepaper

## The First AMM-Based Decentralized Exchange on the Kaspa Ecosystem

_Version 3.0_

## Abstract

Zealous Swap is pioneering decentralized finance as the first DEX on the Kaspa ecosystem. Leveraging the battle-tested V2 AMM architecture, Zealous Swap introduces an innovative NFT-based fee tier system that rewards early adopters while maintaining deep liquidity—critical for a nascent ecosystem. The protocol features built-in security and sustainability mechanisms through its insurance fund and protocol-owned liquidity initiatives, ensuring long-term viability and user protection. This whitepaper outlines our strategic approach to solving the liquidity bootstrapping challenge while establishing secure and sustainable financial infrastructure for the Kaspa ecosystem.

## 1. Introduction

Zealous Swap aims to be the cornerstone of decentralized trading on the Kaspa ecosystem, providing a secure, efficient, and user-friendly platform for token swaps and liquidity provision. Our mission is to build sustainable DeFi infrastructure that grows alongside the Kaspa ecosystem, focusing on deep liquidity, capital efficiency, and accessible user experience.

The launch of a new blockchain ecosystem presents unique challenges, including fragmented liquidity, user education, and achieving network effects. Zealous Swap addresses these challenges through thoughtful protocol design and innovative incentive mechanisms. Our protocol incorporates two key sustainability features: an insurance fund that protects users against potential security incidents, and protocol-owned liquidity that ensures stable trading conditions regardless of market volatility. Both mechanisms receive fees as LP tokens, further enhancing the protocol's liquidity depth while serving their distinct protective and stabilizing functions.

## 2. Technical Architecture: Why V2?

After careful consideration of the nascent Kaspa ecosystem, Zealous Swap has strategically chosen to implement the V2 AMM architecture for its initial deployment. This decision was guided by several key factors that prioritize ecosystem bootstrapping and user experience:

### 2.1 Concentrated Liquidity in a Single Pool

- V2 architecture centralizes all liquidity for each trading pair in a single pool
- Avoids fragmentation across multiple fee tiers (as seen in V3)
- Results in deeper liquidity and reduced price impact for traders
- Critical for a new ecosystem where total liquidity may be limited initially

### 2.2 Simplified Liquidity Provision

- Lower barrier to entry for liquidity providers
- No complex range setting or active management required
- Passive yield generation through a straightforward deposit model
- Encourages broader participation across the Kaspa community

### 2.3 Scalability Path

- Establishes foundation for future protocol upgrades
- Allows for V3 implementation as ecosystem matures
- Enables smooth transition with minimal disruption to users

## 3. Innovative NFT-Based Fee Mechanism

Zealous Swap has partnered with Nacho to integrate the NACHO KAT NFTs collection as the cornerstone of our innovative dual-fee system. This partnership enhances our platform with an established NFT collection while maintaining the mathematical integrity of our liquidity pools.

### 3.1 Mechanism Design

- **NACHO KAT NFTs Integration**: All 10,000 NACHO KAT NFTs will serve as membership tokens for Zealous Swap
- **Tiered Fee Structure**:
  - NACHO KAT NFT holders: 0.2% swap fee (33% discount)
  - Standard users: 0.3% swap fee
- **Fee Distribution**:
  - Standard users: 0.25% to liquidity providers, 0.05% to protocol treasury
  - NFT holders: 0.17% to liquidity providers, 0.03% to protocol treasury

### 3.2 Mathematical Consistency

The NFT fee mechanism preserves the constant product formula (x * y = k) at the pool level while introducing user-specific fee tiers at the interface level. This approach ensures:

- All trades, regardless of fee tier, interact with the same underlying liquidity pool
- The constant product curve remains unchanged for price calculation
- Fee differentiation occurs at transaction execution rather than pool calculation

This implementation differs from V3's multi-tier pools, where liquidity is fragmented across separate pools with different fee settings. Instead, our approach maintains unified liquidity while still offering fee advantages to NFT holders.

### 3.3 Fee Mechanics & Pool Integrity

The fee discount does not disrupt the V2 constant product formula. Fees are applied externally to the swap input:

1. User submits a swap of Δx tokens
2. Protocol deducts a fee (0.2% or 0.3%) from Δx
3. Remaining Δx_net is used to compute output Δy via k

Thus, pool reserves (x, y) and k update identically regardless of user fee tier, preserving mathematical integrity.

### 3.4 Fairness of the 0.3% Fee for Regular Traders

While the 0.3% fee applies to non-NFT holders, it remains competitive within the broader decentralized exchange landscape. Given the liquidity advantages of Zealous Swap, which ensures deeper liquidity pools and reduced slippage, regular traders still benefit from favorable trading conditions. Furthermore, the fee structure aligns with the standard fees seen across most decentralized exchanges, making it a fair and accessible option for traders not holding NFTs. The ecosystem's design ensures that everyone—whether holding NFTs or not—can access a highly efficient trading platform without compromising fairness or usability.

## 4. Strategic Advantages of the NFT Fee System

### 4.1 Accelerated Liquidity Bootstrapping

- Creates immediate value proposition for NACHO KAT NFT holders
- Drives initial acquisition of strategic users and liquidity providers
- Establishes protocol revenue streams from day one
- Leverages existing NFT community for rapid ecosystem growth

### 4.2 Enhanced Market Efficiency

- Enables privileged arbitrage opportunities for NFT holders
- Tightens spreads and reduces price dislocations across markets
- Improves overall market efficiency while maintaining unified liquidity

### 4.3 Competitive Advantage for Strategic Traders

- Provides tangible fee advantages for high-frequency traders
- Attracts institutional and professional market makers
- Creates positive feedback loop between volume and liquidity

## 5. Economic Analysis: NFT Fee Impact

The 0.1% fee differential between NFT holders and standard users creates significant economic advantages, particularly for high-frequency traders and arbitrageurs.

| Trading Volume (Monthly) | Standard Fee Cost | NFT Holder Fee Cost | Monthly Savings | Annual Savings |
|--------------------------|-------------------|---------------------|-----------------|----------------|
| $100,000                 | $300              | $200                | $100            | $1,200         |
| $1,000,000               | $3,000            | $2,000              | $1,000          | $12,000        |
| $10,000,000              | $30,000           | $20,000             | $10,000         | $120,000       |

This cost advantage creates a natural price floor for NFT membership, as the value proposition becomes immediately apparent for traders exceeding certain monthly volumes. For professional market makers and arbitrageurs, NFT acquisition represents a strategic competitive advantage.

### 5.1 Arbitrage Enhancement

The fee differential provides NFT holders with privileged arbitrage opportunities. When price discrepancies between Zealous Swap and external markets fall within the 0.1% fee differential, only NFT holders can profitably execute arbitrage trades, leading to:

- More efficient price discovery
- Tighter spreads across the ecosystem
- Enhanced trading volume through arbitrage activity
- Additional utility and demand for NACHO KAT NFTs

### 5.2 Economic Flywheel

- Early Adopters: NFT holders trade at lower costs, increasing volume and LP fee earnings
- Liquidity Growth: Higher LP rewards attract more providers, tightening spreads
- Arbitrageurs: Low fees and tight spreads attract arbitrage, improving price accuracy
- Increased NFT Utility: NACHO KAT NFTs gain additional utility, enhancing their value proposition

### 5.3 Sustainability Analysis

- Protocol Revenue: Even with 50% of volume from NFT holders, effective fee averages 0.25%, ensuring sustainable revenue
- Volume Leverage: A 0.1% fee reduction can increase whale trading volume thus generating more fee for LPs

## 6. NFT Utility & Governance

Holders of NACHO KAT NFTs will enjoy multiple benefits within the Zealous Swap ecosystem:

- Reduced trading fees (0.2% vs 0.3%)
- Participation in protocol governance (future implementation)
- Token airdrop eligibility (future consideration)
- Whitelist access to any other platforms we build

## 7. Benefits to the Kaspa Ecosystem

Zealous Swap plays a key role in supporting the growth of decentralized applications (dApps) on the Kaspa ecosystem by providing essential infrastructure, such as deep liquidity pools and reliable price oracles.

Scalable Liquidity for dApp Integration: Zealous Swap's deep liquidity pools offer the necessary foundation for seamless token swaps in other dApps. By reducing slippage and ensuring smooth transactions, these pools make it easier for developers to integrate token swapping functionalities into their applications.

Reliable Price Oracles: Zealous Swap provides an accurate on-chain price oracle, using a time-weighted average price (TWAP) model. This ensures dApps have access to reliable, real-time price data, vital for use cases like lending, borrowing, and derivatives trading.

Supporting Ecosystem Growth: By offering these services, Zealous Swap lays the foundation for future dApp developers on the Kaspa ecosystem, helping to create a sustainable and thriving DeFi ecosystem that attracts new projects to build on Kaspa's scalable blockchain solution.

## 8. Protocol-Owned Liquidity and Insurance Mechanisms

### 8.1 Protocol-Owned Liquidity (POL)

A portion of trading fees allocated to the Zealous Swap treasury will be directed to protocol-owned liquidity initiatives, creating sustainable infrastructure for the Kaspa ecosystem. These funds will be received as LP tokens, which directly improves the protocol's liquidity depth. Key aspects include:

- Long-term protocol sustainability independent of mercenary liquidity
- Ability to support strategic trading pairs even with initially lower volume
- Protection against liquidity crises during market downturns
- Permanent liquidity that will never be sold, ensuring consistent trading capabilities
- Future DAO governance can vote to reallocate this liquidity between different pools, while maintaining its presence within the protocol at all times

### 8.2 Insurance Fund (IF)

Zealous Swap will implement an insurance fund as a protective mechanism for users against potential protocol exploits or hacks. The insurance fund operates as follows:

- A portion of fees directed to the Zealous Swap treasury will be allocated to the insurance fund
- Insurance fund contributions are held as LP tokens, further enhancing protocol liquidity
- Unlike protocol-owned liquidity, these LP tokens can be sold when necessary to cover emergency situations
- The fund can accommodate various tokens including KAS and Zealous Swap's native token
- Provides an additional layer of security for users while simultaneously improving market depth

## 9. Flash Swaps

Flash Swaps represent a groundbreaking feature of Zealous Swap, enabling users to temporarily borrow any token without upfront capital requirements. This powerful functionality allows traders to utilize borrowed tokens freely within a transaction, with the simple condition that they either pay for the borrowed tokens with corresponding pair tokens or return them with a minimal fee by the transaction's conclusion.

Flash Swaps democratize sophisticated trading strategies that traditionally required substantial initial capital, such as arbitrage opportunities where price differences between Zealous Swap and other exchanges can be exploited for profit. Additionally, they streamline complex operations like leveraging positions on lending platforms, reducing multiple gas-intensive steps into a single efficient transaction.

 By removing capital barriers and simplifying intricate DeFi interactions, Flash Swaps make advanced trading techniques accessible to all participants while simultaneously contributing to market efficiency through increased arbitrage activity.

## 10. Modular-Fee Engine

The Modular-Fee Engine represents a cornerstone innovation of Zealous Swap, designed to optimize trading efficiency across diverse token ecosystems. This sophisticated system transcends the limitations of fixed-fee models by implementing adaptable fee tiers customized to the specific characteristics and volatility profiles of different token pairs.

Particularly beneficial for stablecoin trading, where price movements tend to be more constrained, the engine enables significantly reduced fees—as low as 0.05% standard and 0.03% discounted for stable pools, compared to 0.3% and 0.2% respectively for volatile token pairs.

This granular approach to fee structuring not only enhances capital efficiency and reduces slippage but also creates deeper liquidity pools that benefit all ecosystem participants. With future capabilities including DAO governance integration and dynamic fee adjustments based on real-time market conditions, the Modular-Fee Engine establishes Zealous Swap as a trading platform that continuously evolves to meet the nuanced demands of DeFi traders while maintaining optimal liquidity provider incentives.

## 11. Conclusion

Zealous Swap represents the next evolution in decentralized exchange design, thoughtfully optimized for the emerging Kaspa ecosystem. By implementing a strategic V2 architecture enhanced with innovative NFT-based fee mechanics through our partnership with Nacho, we create a platform that balances immediate usability with long-term sustainability.

Our approach prioritizes liquidity depth, user accessibility, and economic incentives that align all ecosystem participants. Through careful consideration of the unique challenges faced by emerging blockchain networks, Zealous Swap is engineered to solve the liquidity cold-start problem while establishing the foundation for a thriving DeFi ecosystem on Kaspa.

As the Kaspa ecosystem grows, Zealous Swap will evolve alongside it, maintaining our commitment to providing premier decentralized trading infrastructure.

Join us in building the financial foundation of the Kaspa ecosystem.

## 12. Team

Zealous Swap is built by a dedicated team with experience in blockchain and decentralized finance. Led by Louis Saad and Ramy Lahoud, we are focused on creating a decentralized exchange that supports the growth of the Kaspa ecosystem.

---

Disclaimer: This whitepaper is provided for informational purposes only and does not constitute financial advice or an offer to sell securities. Cryptocurrency trading involves significant risk. Users should conduct their own research before participating in any DeFi protocol.
