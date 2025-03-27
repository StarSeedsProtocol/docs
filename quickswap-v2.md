---
hidden: true
---

# QuickSwap V2

#### QuickSwap V2

QuickSwap, a fork of Uniswap V2, originally deployed on the Polygon blockchain, provides efficient and user-friendly liquidity pools.

**Uniswap V2: Pioneering the AMM Landscape**

Uniswap V2 is a cornerstone in the decentralized exchange (DEX) ecosystem, introducing the Constant Product Market Maker model, which revolutionized liquidity pool mechanics.

Technology Overview:

* Model: Uniswap V2 contracts operate on the Constant Product Market Maker formula ( x \* y = k) where ( x ) and ( y ) are the reserve quantities of two tokens, and ( k ) is a constant ensuring liquidity across all price levels.

Liquidity Provision:

* Liquidity providers (LPs) deposit equal value of two ERC20 tokens into the pool.
* The initial provider determines the exchange rate by setting the first pair of token deposits.
* LPs receive liquidity tokens that represent their proportional ownership in the pool.

Fee Mechanism:

* A 0.3% trading fee is charged on every swap, distributed among LPs in proportion to their stake.

Key Innovations:

* Decentralized Liquidity Provision: Any user can add liquidity and earn fees without requiring permission.
* Price Stability and Arbitrage: Prices are adjusted dynamically by trades, promoting efficient market conditions.
* Oracles: Time-weighted average price (TWAP) oracles for secure off-chain integrations.
