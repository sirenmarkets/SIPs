---
  sip: 19
  title: LP Compensation Plan
  author: Dalakos, SeaFi & Tishana
  comments-uri: https://gov.sirenmarkets.com/t/sip-19-lp-compensation-plan/269
  status: Proposed
  type: SIPs
  created: 2021-09-08
---
![SIP19|690x400](upload://4B2K3AVMh9SJNjDL5vFjVckkjDs.jpeg) 

## Context
On 3 September 2021 at around 12:17 AM UTC several SIREN AMM pools were exploited via a reentrancy attack. As a result, approximately $3.5M worth of assets were drained from the AMM pools. An in-depth incident report can be found [here](https://medium.com/siren-markets/siren-incident-report-264e57f16d7).

The current total damage is assessed to be ~$3.5M USD in value at the time of the attack:

* 266,708 WMATIC
* 689,083 USDC
* 50,959 SUSHI
* 185,392 KNC
* 268 WETH
* 11,995 UNI

The exploited funds are sitting in these four addresses. We are closely monitoring the movement of these addresses and would appreciate extra community support to do the same.

* 0x07Ba7e8947f8Fb4d33f3C7E25c2CB35B858F02Eb
* 0xfAc4088BbA1fA090FD3F1F52fd691a45C30AC053
* 0xf834eFE5B959E52E3b78cB28c4BC501b52CE41da
* 0x99da8fb52f74b7a3e38d9c75c634f6386f1649c7

## Past Reparation Plans
We have extensively looked into different plans for projects that have had similar incidents.

***Harvest Finance***

* Hacked for $25M in October 2020
* Proposed community solutions via [Snapshot](https://snapshot.org/#/harvestfi.eth/proposal/QmYF62qGaqyHAXt88Hmxise6CFaSWxnTmi5VedZ3VX8Zy2)
  * Create an IOU token for USDC/USDT depositors that feeds a percentage of profit sharing cash flow and a percentage of weekly emissions to reparations pools, up to the amount lost in the attack.
  * Don't create an IOU token, USDC/USDT depositors would take the ~13.5% loss. Dedicate all dev time and resources to the existing roadmap.
* 75% of the community was in agreement with the IOU plan
* Harvest is now recovered and are at a 2x of their token price since the hack.

***Origin Protocol***

* $7M hack in November 2020
* First 1000 OUSD would be paid back in full compensation with a newly minted OUSD Stablecoin
* For the rest, 25% of their funds in the new OUSD and 75% in OGN governance token locked for 1 year. To compensate for the lock-up, the OGN will earn interest at 25% over the year.
* Compensation blog post here(https://blog.originprotocol.com/origin-dollar-ousd-detailed-compensation-plan-faa73f87442e)

***Ezfi***

* $60M hack in April 2021
* 25% would be paid out in stableCoin.
* 75% would be paid out in EZ IOU(I owe You) token and would be redeemable over a period of 6 months
* Compensation Plan Blog(https://medium.com/easify-network/interim-compensation-plan-8fa81e46ada4 )
* Security Incident (https://medium.com/easify-network/easyfi-security-incident-66c02a277a91 )

## Our Proposal
We can compensate LPs in two possible ways: either 

***Reparation A***: SI in a vesting wallet at a $1 SI valuation that begins unlocking in 12 months and finishes unlocking at 24 months
***Reparation B***: Create an IOU token for depositors that feeds a percentage of revenue sharing cash flow and a percentage of weekly emissions to reparations pools

The community should decide which proportion of A and B should comprise the reparations out of these three possible scenarios:

Option 1

* 100% future protocol revenue and emissions (Reparation B)

Option 2

* 25% SI at $1 valuation with lockup (Reparation A)
* 75% future protocol revenue and emissions (Reparation B)

Option 3

* 50% SI at $1 valuation with lockup (Reparation A)
* 50% future protocol revenue and emissions (Reparation B)

The Foundation Community Fund currently contains approximately ~16MM SI. A 50% payout in SI represents ~10.5% of the Community Fund, and a 25% payout represents ~5.3% of the Community Fund.

We developed this compensation plan to strike a balance between making LPs whole while also not painfully compromising the runway of the project. We welcome feedback regarding this proposal from the community. This proposal will be open for discussion after which voting will be conducted on Snapshot.

We will continue to fulfill our mission to bring DeFi options to the masses.

Thank you for sticking with us 🧜‍♀️