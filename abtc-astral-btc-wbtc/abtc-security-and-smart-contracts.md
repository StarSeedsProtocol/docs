# ABTC Security & Smart Contracts

1\. ABTC – Astral BTC Wrapper (Fraxtal)

Blockchain: Fraxtal&#x20;

Smart contract address\
0xfE2A4651B142B96EB6c6EDfF61C1333e0cAB4BB0\
\
This is an multi-chain ERC20 token contract deployed through the Axelar interchain token service.[<br>](https://www.lagrange.dev/blog/cheap-fast-cross-chain-queries-from-fraxtal-with-lagranges-zk-coprocessor?utm_source=chatgpt.com)

***

#### 2. WBTC – Wrapped Bitcoin (Collateral Token on Ethereum)

Blockchain: Ethereum mainnet

Smart contract address\
0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599

What this contract does (short)\
This is the WBTC ERC-20 token contract, representing BTC 1:1 on Ethereum. In the ABTC strategy, WBTC from this contract is used as collateral in Curve’s WBTC lending market to borrow crvUSD (without selling BTC). WBTC itself follows a merchant–custodian model where each token is backed by BTC in custody with on-chain proof of reserves.[\
<br>](https://www.okx.com/how-to-buy/wrapped-bitcoin-wbtc?utm_source=chatgpt.com)

***

#### 3. Resupply – sfrxUSD / Stablecoin Leverage Market

Blockchain: Ethereum

Smart contract address\
sfrxUSD market: 0xC5184cccf85b81EDdc661330acB3E41bd89F34A1

What this contract does (short)\
This Resupply market lets users lend crvUSD or frxUSD into underlying Curve Lend / Fraxlend markets while borrowing reUSD against those positions. In the ABTC strategy, borrowed crvUSD is supplied here to create a leveraged stablecoin yield position. The contract logic follows Resupply’s model of using yield-bearing stablecoins as collateral to “boost” yields.[\
<br>](https://news.curve.finance/curve-resupply-a-proposal-to-mint-5m-crvusd/?utm_source=chatgpt.com)

***

#### 4 WBTC / Curve Lend Market

Blockchain: Ethereum&#x20;

Smart contract address\
WBTC Curve Lend market: 0x2d8ecd48b58e53972dBC54d8d0414002B41Abc9D

What this contract does (short)\
This contract allows users to deposit WBTC collateral to borrow crvUSD tokens.\
<br>
