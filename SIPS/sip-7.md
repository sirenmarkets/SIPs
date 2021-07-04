---
  sip: 7
  title: $SI Token Distribution Event
  author: ChadoftheSea (@chadofthesea)
  comments-uri: https://gov.sirenmarkets.com/t/sip-7-si-token-distribution-event/146
  status: Proposed
  type: SIPs
  created: 2020-02-17
---


## Simple Summary

In response to community requests and in order to continue the decentralization of the network, it is proposed that between 2 and 5 Million SI tokens be released through a distribution channel. This distribution may be comprised of but not limited to a token sale, supplying liquidity by the DAO into an AMM (to be chosen by the SI community) or a decentralized auction mechanism. A community priority is that the token launch occurs sooner rather than later in order to allow vesting of SI tokens to LPs to begin and also to take advantage of a favorable crypto market.

We recommend launching via a Balancer Liquidity Bootstrapping Pool (LBP) as this is the most effective form of decentralized price discovery that we have seen work for numerous other public launches including Perp Protocol, APY Finance, and NSure

## Abstract

The recommendation is that the DAO will distribute between 2 and 5 MM SI Tokens from the treasury to the SIREN community.

The options for token launch include 1) Seeding a Uniswap pool, 2) Direct listing on a centralized exchange, and 3) Running a Balancer LBP followed by a Uniswap pool.

Seeding a Uniswap pool is the simplest option. The DAO would move tokens into a Uniswap pool in order to allow people on the open market to purchase SI using another currency.

Listing on a centralized exchange requires negotiating with exchanges in order to find one willing to list SI. Listing on an exchange may require a fee and may take some amount of time to execute.

Running a Balancer LBP is slightly more complicated than a Uniswap pool, but does not rely on an outside party for execution. The DAO would move both tokens and some stablecoin into a Balancer smart contract and over the course of several days the price would start high and decrease in order to allow for price discovery. The parameters for the LBP will be modeled after those used by other projects such as Perpetual Protocol, e.g. 90-10 to 30-70 weight shifts and a 3-day sale duration. After the LBP, either the DAO or community members would create a Uniswap pool to provide ongoing liquidity for the SI token.

## Motivation

Community members of the SIREN Project, including Liquidity Providers (LPs) that have participated in the existing Liquidity Provider Program (LPP) https://gov.sirenmarkets.com/t/sip-6-liquidity-mining-emission-proposal-for-next-erc-20-pairing/141 2, have an interest in seeing the SI token have a successful launch.

Multiple mechanisms exist to move tokens to the public, each having their own benefits and drawbacks. The community has multiple different priorities, including launching relatively quickly, ensuring a stable and well-supported price for the token on the open market, having good liquidity for the SI token, whether it behooves the DAO to raise money for future project support, and using decentralized solutions that align with SIREN community values.

### Option 1: Uniswap Pool

The simplest possible way to facilitate a token listing is to create a Uniswap pool. Benefits of this option include its ease and its decentralized nature which aligns with the priorities of the SIREN project. This option also allows the DAO to raise funds for future project support. A Uniswap pool can be deployed quickly, allowing for rapid token deployment.

The main drawback of a Uniswap pool is the potential for bots to front run token purchase transactions in the early life of the pool while the price is low, potentially shutting community members out of participating in acquiring tokens at a favorable price. This situation may cause the price of SIREN to spike and subsequently crash.

An additional drawback to the Uniswap pool method is that there are no marketing services included in creating a Uniswap pool. A priority of community members is that the price of SI following the launch is favorable—i.e. not too low. Without additional marketing it is possible that there will be low demand for the SI token, resulting in a poor token price.

### Option 2: Centralized Exchange Listing

Listing SI on a centralized exchange provides some pros over the Uniswap pool, while having its own cons. One benefit is significant marketing support and tapping into an existing user base. Having marketing support for the SI token launch may provide for a higher final price for the SI token.

Another benefit of a centralized listing is price stabilization—a centralized listing generally occurs at a fixed price and will be supported by market makers, ensuring a stable price movement and that buyers can acquire SI tokens on demand.

Drawbacks of a centralized exchange listing include difficulty, potential expense, inability for the DAO to raise money, and lack of alignment with SIREN community principles and values. An exchange listing may be difficult to facilitate and may cost the project a listing fee, and negotiating with exchanges may take a significant amount of time, resulting in delays in the token launch.

With a direct listing, typically the project does not sell tokens as part of the listing, which means the DAO cannot use the token launch as an opportunity to raise funds. Finally, SIREN is a decentralized project, and the SIREN community prioritizes decentralization as the path to the future. Launching a token on a centralized exchange does not align well with these priorities.

### Option 3: Balancer LBP plus Uniswap Pool

A relatively recent addition to the DeFi community, a Balancer Liquidity Bootstrapping Pool (LBP) is becoming an increasingly popular option for a token launch. Benefits of an LBP include ease of deployment, protection from front running bots and price spikes, the ability for the DAO to raise funds, and alignment with community values. Following the LBP with a Uniswap pool will ensure ongoing liquidity for the SI token post launch. For detailed information on Balancer LBPs, see the Balancer info post here: https://docs.balancer.finance/smart-contracts/smart-pools/liquidity-bootstrapping-faq 2

A Balancer LBP is relatively simple to deploy—deployment involves seeding a pool with both SI and a stablecoin (likely USDT or USDC) and setting the weights and run time of the pool. The price of SI starts very high and drops over time according to a predetermined algorithm, which prevents bots from front running transactions to get a lower price. The controlled nature of the LBP is also designed to prevent significant price spikes and crashes during the pool run time. The LBP will allow the DAO to raise funds for ongoing project support. Additionally, the decentralized structure aligns with SIREN community values and also allows for rapid token deployment.

Drawbacks of the LBP include the lack of dedicated marketing services and ongoing token price support. Market makers are unlikely to manage the price of SI in a Uniswap pool as compared to on a centralized exchange, and running a Balancer LBP also does not come with marketing support that may bring people to the token launch, which may result in a lower final token price.

Of the three options, we recommend moving forward with a Balancer LBP