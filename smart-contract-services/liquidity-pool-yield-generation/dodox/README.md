# DodoX

StarSeeds Protocol utilizes DODO's Proactive Market Maker (PMM) algorithm to manage its liquidity pools, specifically employing Private Pools, Pegged Pools, and Single-Sided Liquidity Pools. These configurations are part of DODO's V2 offerings, designed to enhance capital efficiency and provide flexible liquidity solutions.

Proactive Market Maker (PMM) Algorithm

DODO's PMM algorithm is an advanced inventory management strategy that adjusts asset prices based on real-time supply changes. When the quantity of an asset decreases, the PMM algorithm automatically increases the price quoted for this asset in anticipation of buying back the missing inventory from the market.

[Dodoex Documentation](https://docs.dodoex.io/en/product/pmm-algorithm?utm_source=chatgpt.com)

The PMM pricing formula is expressed as:

P = i / (1 - k + (Q₀ / Q)² \* k)

Where:

* P is the price of the asset.
* i is the initial "guide price."
* k is the "slippage factor," determining the sensitivity of price to inventory changes.
* Q denotes the current token supply.
* Q₀ denotes the equilibrium supply, representing the desired inventory level.

This formula allows the PMM to concentrate liquidity around a target price, enhancing capital efficiency compared to traditional Automated Market Makers (AMMs). By adjusting the slippage factor k, liquidity providers can control how aggressively prices respond to inventory changes, thereby managing slippage and impermanent loss more effectively.

Differences Between DODO's PMM and Traditional AMMs

Traditional AMMs, such as Uniswap's constant product formula (x \* y = k), maintain a fixed relationship between asset quantities, leading to passive pricing that doesn't account for external market conditions. In contrast, DODO's PMM algorithm proactively adjusts prices based on real-time inventory levels and external price feeds, resulting in:

* Concentrated Liquidity: Liquidity is focused around the market price, providing better rates for traders and reducing slippage.
* Reduced Impermanent Loss: By aligning pool prices more closely with external markets, the PMM minimizes the divergence between pool prices and market prices, thereby reducing impermanent loss for liquidity providers.
* Single-Sided Liquidity Provision: Liquidity providers can supply a single asset to a pool, simplifying the process and lowering the barrier to entry.

These innovations make DODO's PMM algorithm a flexible and efficient alternative to traditional AMMs, offering improved trading experiences and better capital utilization for liquidity providers

\
