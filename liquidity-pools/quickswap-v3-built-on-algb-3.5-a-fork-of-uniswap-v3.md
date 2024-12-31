# QuickSwap V3 - Built on ALGB 3.5- A Fork of Uniswap V3

Algebra 3.5 adds Tax-On-Transfer token compatibility along with real-time volume based dynamic swap fee functionality to Uniswap V3 concentrated liquidity.

\


**Uniswap V3**

1. Concentrated Liquidity:

* Liquidity is deposited within a bounded range, defined by two prices.
* Outside this range, liquidity is inactive and composed of a single asset.
* Within the range, liquidity acts as if it has larger "virtual reserves," leading to greater capital efficiency.

2. Flexible Fee Structure:

* Multiple fee tiers (0.05%, 0.3%, and 1%) can be chosen during pool creation.
* Custom tiers can be added by governance (e.g., UNI token holders).

3. Non-Fungible Liquidity Positions:

* Each position is represented as an ERC-721 (NFT).
* Fees are no longer compounded into the pool but stored separately as tokens.

4. Advanced Oracles:

* Time-Weighted Average Price (TWAP) and Geometric Mean Price for improved accuracy.

5. Multi-Pool Per Pair:

* Supports multiple pools per token pair, each with a different fee tier.
