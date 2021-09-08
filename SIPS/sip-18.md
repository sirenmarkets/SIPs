---
  sip: 18
  title: Shifting Liquidity Towards Utilization
  author: Seafi (@seafi)
  comments-uri: [To Add]
  status: Implemented
  type: SIPs
  created: 2021-08-31
---

[SIP18](https://user-images.githubusercontent.com/83624992/131561153-4c4bcfd8-d335-4b8a-9e25-0fd0532a46c8.png)

Current AMM LP rewards are described in the [SIP-11 Implement dynamic LP rewards].(https://gov.sirenmarkets.com/t/sip-11-implement-dynamic-lp-rewards/214) The idea behind it was to incentivize a base level of liquidity in each pool ($1M currently) while giving additional rewards when liquidity is being utilized for options writing. Pools with capital less than the base level earn higher rewards in order to incentivize more capital to be deposited until it reaches the base level of $1M, after which rewards gradually drop off.

One important observation from running the program since March is that pools that are below $1M disproportionately earn their rewards based on the amount of capital, leaving no space for utilization-based rewards. For example, LPs in less-mainstream pools such as MATIC and KNC earn triple-digit APYs even without taking any risk in a form of open interest.

https://user-images.githubusercontent.com/83624992/131561122-400da44f-bd02-40e0-8b3f-571ad5dfb21d.png

## Going Forward

SIREN’s ultimate vision is to enable options across thousands of assets where LPs earn yield proportional to the level of risk they are taking in a form of open interest. Increasing trading volumes drive utilization, generatinge more organic yield and attractingattract more capital to be deposited in the pool. Under thisthat scenario it is acceptable for a less-popular pool to have little capital until options trading in that asset picks up.

In order to bring the current reward scheme closer to that vision we propose the following:
Reduce the minimum liquidity threshold from $1M to $250K. This would drive down yields in pools with low capital and low utilization.
Reduce the steepness of the liquidity rewards function from 10 to 4 to preserve the shape of the curve after the liquidity threshold adjustment above.
Reduce the S-point of utilization function from 0.5 to 0.4 in order to further incentivize utilization. 

The proposed changes are demonstrated using the charts below. The net result will be less rewards for low-capital / low-utilization pools, more rewards for medium-to-high utilization pools.

https://user-images.githubusercontent.com/83624992/131561302-f3723706-1f57-4be0-842d-8ab52b21a7c3.png
