---
  sip: 11
  title: Implement dynamic LP rewards
  author: HeyChristopher (@HeyChristopher)
  comments-uri: https://gov.sirenmarkets.com/t/sip-11-implement-dynamic-lp-rewards/214
  status: Proposed
  type: SIPs
  created: 2021-03-07
---


Siren is currently spending 17,857 SI per day (125k per week) to incentivize liquidity which is working well within its desired bounds. However, only the SUSHI Call options seem to have sufficient open interest.

Every liquidity pool currently earns 2.976 SI, but only one pool (SUSHI Call) is appropriately used. Therefore Siren is now overpaying almost 15,000 SI per day to liquidity pools with little traction. That’s more than 80%.

Therefore, we suggest implementing a dynamic reward scheme that takes the pool utilization, current SI price, and default interest rate across DeFi into consideration.

Pool utilization: How many percent of the pool liquidity is currently sold. Calculated as Open Interest across strike prices/liquidity.

Default interest rate: The base rate we would have to outbid to attract liquidity - Curve 3pool for stablecoins and Aave interest rates for UNI and YFI. The SUSHI interest rate would be XSUSHI and can be obtained from Sushi. To incentivize liquidity beyond this base rate, we suggest adding a further 5%. We call this the incentivized base rate.

Current base rates would be:

USDC: 15% (from Curve 3pool)
UNI: 0.04% (from Aave)
YFI: 0.74% (from Aave)
SUSHI: 4% (from xSUSHI staking)
Other parameters:

Max SI per day per pool: 3,000 (slightly more than what is currently being paid)
Minimum liquidity per pool: 1,000,000 USD (if we have less than this amount in any liquidity pool, we have to increase our rewards)
Given these parameters, we suggest the following distribution of rewards:

<INSERT SCREENSHOT>

Notebook: https://gesis.mybinder.org/binder/v2/gh/HeyChristopher/siren-rewards-sip/52bcaaa8aa23aff121eac8701cfdfa5564a8b2b9 14

Source: https://github.com/HeyChristopher/siren-rewards-sip 2

Explanation:

When total liquidity per pool is below our minimum liquidity (0%), the rewards should reach their maximum. Or to say it in another way: The APY should be very high when there is not a lot of capital in the pool so that we attract more capital quickly
Once we have enough liquidity, we start to look at the utilization of the pool. We are suggesting to approximately pay the incentivized base rate between 20% and 50% utilization. Above 50% utilization, the rewards quickly increase towards their maximum to ensure that we always have enough capacity. The rewards drop below the base rate when the utilization is very low (<20%)
With this model, we can increase the current liquidity mining program’s duration by a few times, even with increased utilization.

Open questions:

- Are the curves too steep? The APY could jump from 300% to 10% quickly for certain pairs with just 100k USD added, resulting in too many people hopping in and out of the pool.
- Is the base rate + 5% appropriate? Is this too much, or is this too low?
- What is an appropriate minimum liquidity amount we want to make sure is always in the pool? Is $1m too much or too little?