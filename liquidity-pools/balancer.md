# Balancer

Balancer is a decentralized automated market maker (AMM) that allows users to create liquidity pools with custom token weights. It generalizes the constant product formula used in many AMMs, enabling more flexible configurations such as multi-token pools and uneven weight distributions.\
\
**Balancer’s Key Features:**

1. **Trade Execution:**\
   When a trade occurs, the product of weighted reserves remains constant. The balances and adjust to reflect the new token quantities while preserving the invariant .
2. **Multi-Token Pools:**\
   Balancer pools can hold more than two tokens, making them versatile for liquidity providers and enabling complex asset management strategies.
3. **Dynamic Fee Adjustments:**\
   Balancer V2 allows for dynamic fee adjustments depending on market conditions, offering improved capital efficiency.
4. **Custom Weights:** \
   Each token in the pool can have a different weight, enabling configurations like 70/30 or 90/10 pools instead of the standard 50/50 ratio used in traditional AMMs.
5.  **Custom Weights:**\
    Each token in the pool can have a different weight, enabling configurations like 70/30 or 90/10 pools instead of the standard 50/50 ratio used in traditional AMMs.



The formula for a constant-product pool of assets is an extension of Uniswap’s x \* y = k.

For three assets, it would calculate as: x \* y \* z = k\
For four assets, it would calculate as w \* x \* y \* z = k\
(w, x, y, and z are balances of each tokens in a pool).

\
Weighted spot price formula to determine swap exchange rates as follows:

\


<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcgCcSwmsEw6Ar6FJa6O9TLnGcDxG-ccaVkBtxj9VXLBSZmHHCQQPrp2_-5LsHRuP9eBnuj8NdYEQ-jw4p0ePCmwGLdAbvJHNOvP3p1EhwsxKi5nGr5WjtLoXBNRAm9GyDDsmKQAA?key=Mn8gS0mHdvtDkUHdD1jktvk7" alt=""><figcaption></figcaption></figure>

\


Liquidity pools on Balancer can be Controlled or Finalized. Controlled pools are updatable by the pool creator. The Controlled pool allows for asset weight, asset type, and fee adjustments. Finalized pools have fixed pool asset types, weights, and fees.

\
While Balancer can be thought of as an exchange, it can also be thought of as an index protocol, where the token weightings are set to specific percentages of a pool and arbitrageurs ensure that weighting is maintained.

\
