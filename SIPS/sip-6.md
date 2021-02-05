---
  sip: 6
  title: Liquidity Mining Emission Proposal for Next ERC-20 Pairing
  author: Rand Hydra (@randhydra)
  comments-uri: https://gov.sirenmarkets.com/t/sip-6-liquidity-mining-emission-proposal-for-next-erc-20-pairing/141
  status: Proposed
  type: SIPs
  created: 2021-02-05
---

## Simple Summary

In order to incentivize usage of the network and increase TVL, a rewards program
is proposed to incentivize liquidity providers to provide funds to the network,
for the next ERC-20 pair to be added to SIREN. The candidates to be added are:

* SUSHI/USDC
* UNI/USDC
* YFI/USDC
* LINK/USDC

## Abstract

The recommendation is that 1,000,000 [Si
tokens](https://etherscan.io/token/0xD23Ac27148aF6A2f339BD82D0e3CFF380b5093de)
be placed into a staking contract as a reward to liquidity providers during a
fixed time window of 90 days for both the ERC-20 to be added, along with it's
corresponding USDC pool, beginning on February 22nd and ending on May 23rd.

Rewards will be distributed every 24 hours based on respective pool shares, with
no caps on liquidity.

## Motivation

Currently there is no reward to drive liquidity to the platform when new pairs
are added. Major defi platforms such as [Uniswap](https://www.coindesk.com/uniswap-dharma-retroactive-uni-airdrop-defi-governance)
and [Synthetix](https://blog.synthetix.io/what-you-need-to-know-before-staking-snx-for-the-first-time/)
provide rewards to incentivize usage of the platform, this drives liquidity into
those platforms. In order to be competitive in the defi market, a grant program
using the Synthetix [staking](https://github.com/Synthetixio/synthetix/blob/v2.27.2/contracts/StakingRewards.sol)
and [distribution](https://github.com/Synthetixio/synthetix/blob/v2.27.2/contracts/StakingRewards.sol) contracts would help drive liquidity to the Siren markets pools.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
