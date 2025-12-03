# ABTC: Astral BTC (WBTC)

ABTC (Astral BTC) is a yield-bearing derivative token built on WBTC (Wrapped Bitcoin). ABTC tokens in circulation are backed by WBTC that is deployed into various DeFi Strategies to generate yield.

* Contract Address (Fraxtal deployment): 0xfE2A4651B142B96EB6c6EDfF61C1333e0cAB4BB0<br>

### How ABTC Generates Yield:

Strategy A: WBTC is bridged to Ethereum and deposited into the yield-basis WBTC pool.&#x20;

Strategy B: WBTC is used as collateral to borrow crvUSD which is then deposited with leverage on resupply&#x20;

1. WBTC Collateral on Ethereum: WBTC tokens backing the circulating ABTC supply are bridged to Ethereum (if they originated on another chain) and deposited into Curve’s WBTC lending market (using the crvUSD stablecoin system).&#x20;
2. Borrowing crvUSD: Against the WBTC collateral, crvUSD stablecoins are borrowed. This effectively unlocks liquidity from the WBTC without selling it. The borrowing is managed by Curve’s LLAMMA mechanism which allows for soft-liquidations if Bitcoin’s price fluctuates, thus reducing risk of sudden liquidation. ABTC maintains a conservative collateral ratio (e.g. 50% LTV) to protect against massive and sudden market drops.
3. Leveraged Yield via Resupply: The borrowed crvUSD is then deposited into Resupply – a stablecoin yield optimizer protocol – to greatly amplify the yield. Resupply allows Astral to lend the crvUSD (and also FRAX stable if applicable) into high-yield opportunities while borrowing Resupply's own stablecoin (reUSD) to multiply exposure.
4. Yield tokens are converted to WBTC: The yield generated from those Resupply placements (interest earnings, reward tokens like RSUP, etc.) is systematically used to buy additional WBTC. Essentially, as interest accrues in stablecoins (and any reward tokens are harvested), the strategy swaps that yield into WBTC. The newly acquired WBTC is added to ABTC’s collateral reserves and used to generate more yield.

### How ABTC Distributes Yield

Distributing Rewards: When yield tokens are converted into WBTC, a proportionate amount of ABTC is minted. This newly minted ABTC is then distributed through the following programmed pathways in proportion to how circulating ABTC tokens are being used.\
\
A. ABTC Token Holders: ABTC tokens held in wallets and Gnosis safe contracts receive a rebase via [Merkle.xyz](http://merkle.xyz) distribution campaigns (airdrop/claim mechanism). This distribution distributes yield earnings to ABTC holders: over time, each ABTC holder can claim additional ABTC rewards.\
\
B. BTCWITCH/ABTC Liquidity Pool Deposits: Yield generated from ABTC tokens is deposited into the BTCWITCH/ABTC Curve Pool and the LP tokens received from this action are transferred to a burn address, making the liquidity permanent.
