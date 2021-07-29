---
  sip: 16
  title: Layer 2 Solutions for SIREN 
  author: Dalakos
  comments-uri: https://gov.sirenmarkets.com/t/sip-16-layer-2-solutions-for-siren/262
  status: Proposed
  type: SIPs
  created: 2021-07-29
---

![sip16](https://gov.sirenmarkets.com/uploads/default/original/1X/6b0ba4aa0a4dadb8c6173b328bf9ae82575538e5.jpeg)
 
# Layer 2 Solutions for SIREN

SIREN’s north star is mass adoption and usability of DeFi Options. This requires new and existing traders to onboard, test and utilise the protocol with minimum friction (i.e. efficient gas costs + user experience). 

Due to the current challenges with Ethereum Layer 1 (L1), many protocols have deployed on Layer 2 (L2) solutions to improve the user experience. 

One of the most requested items from the SIREN community is to launch on a Layer 2 (L2) solution. This will solve the higher gas fees for users which will make the various actions on the protocol more efficient (trading and managing pool liquidity). 

As we finish up our v2 contracts release (more info here), we would like to propose v2 deployment to **Polygon Network** and soon after to **Arbitrum.**


## L2 Landscape

Currently there are a handful of scaling solutions in the ecosystem including Optimism, Starkware, zkSync, Polygon and Arbitrum. 

We have been keeping up to date with each solution's progress and spent several months researching the most suitable option for SIREN. Polygon Network and Arbitrum have been our conclusions.
  
***Polygon Network***
Polygon (formerly known as Matic Network) has become the industry standard for an L2 Sidechain solution. Over [43 DeFi protocols](https://defiprime.com/polygon) have deployed on Polygon as a scaling solution. Most notably, companies such as Aave and Sushiswap.

Our reason for choosing:
- EVM Compatible and Subgraph compatible.
- Strong community support
- People are becoming familiar with its network.
- 1000x improvement threshold on transactions.
- $8 Billion+ of liquidity available

***Arbitrum***
Arbitrum is the simplest L2 rollup network to deploy to, and offers between 50x and 200x lower transaction fees. We've also seen many popular DeFi projects express their intent to deploy to Arbitrum. The transaction fee savings are not as high as on Polygon, but optimistic rollups represent a fundamental technical improvement to Ethereum's scalability, and going forward we think it shows the most promise for becoming a core component of the Ethereum ecosystem.

***Why Polygon first, not Arbitrum?***
Polygon Network has already been tested by many DeFi protocols. The network is more efficient, cheaper and there are more users/liquidity at the moment. This makes it a great avenue to test our v2 before rolling to other L2 solutions. 


## Proposed Product Timeline
August 2021
- Deployment to Mainnet Polygon Network
- Assess community feedback
- Host incentives to utilize the network.
September - October 2021:
- Start on our Arbitrium implementation. 

## Rewards Mechanism
On L1 we currently run two reward programs: one for providing liquidity to [Siren’s AMM pools](https://app.sirenmarkets.com/pool) and one for providing liquidity to the [SI/ETH Sushiswap pool](https://app.sirenmarkets.com/stake). Because DEX pool volume is still significantly larger on L1, we will keep the reward program for our L1 Sushiswap pool as is. Users can continue to receive rewards for providing Sushiswap liquidity on L1. 

However, the rewards for AMM pool liquidity will be discontinued on L1, and only run on the L2 pools, starting with Polygon. Users who provide liquidity to Siren’s pools on the Polygon network will receive SI on the Polygon network. Users who wish to aggregate their SI on a single network can use the L1 Polygon bridge to send their SI rewards to either network they choose.

## Next Steps
- Please provide any feedback on the above SIP proposal + cast a deep sea vote below. 
- Quorum Voting will be open for 48 hours from time of posting (28 July 4PM PT - 30 July 4PM PT)
- Snapshot is close to be finalised. SIREN community members will be able to vote via the token in Q3. 

  
## Siren Grants Program Work Flow

The Siren Grants Program will follow the SIP process as all proposals must go through a vote. 
[ WIP ] -> [ PROPOSED ] -> [ APPROVED ] -> [ IMPLEMENTED ] X [ REJECTED ] 

Each status change is requested by the grants author and reviewed by the SIP
editors. Use a pull request to update the status. Please include a link to where
people should continue discussing your SIP. The SIP editors will process these
requests as per the conditions below.

* **Work in progress (WIP)** -- Once the champion has asked the SIREN community
  whether an idea has any chance of support, they will write a draft SIP as a
[pull request]. Consider including an implementation if this will aid people in
studying the SIP.
* **Proposed** If agreeable, SIP editor will assign the SIP a number (generally
  the issue or PR number related to the SIP) and merge your pull request. The
SIP editor will not unreasonably deny an SIP. Proposed SIPs will be discussed on
governance calls and in Discord. If there is a reasonable level of consensus
around the change on the governance call the change will be moved to approved.
If the change is contentious a vote of token holders may be held to resolve the
issue or approval may be delayed until consensus is reached.
* **Approved** -- This SIP has passed community governance and is now being
  prioritised for development.
  
* **Implemented** -- This SIP has been implemented and deployed to mainnet.

* **Rejected** -- This SIP has failed to reach community consensus.

The current SIP editors are

` * Seafi (@seafi)`

` * Zareth San (@zareth-san)`

` * Dalakos (@dalakos88)`


See [the revision history for further
details](https://github.com/sirenmarkets/SIPs), which is also available by
clicking on the History button in the top right of the SIP.

[the SIREN GitHub]: https://github.com/sirenmarkets/SIPs/issues
[pull request]: https://github.com/sirenmarkets/SIPs/pulls
[markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[Bitcoin's BIP-0001]: https://github.com/bitcoin/bips
[Python's PEP-0001]: https://www.python.org/dev/peps/

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
