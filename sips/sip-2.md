---
sip: 2
title: Liquidity Mining Token Emission Schedule
status: WIP
author: yours truly, @swiss-miss
discussions-to: https://github.com/sirenmarkets/SIPs/issues
created: 2020-11-20
requires (*optional): [1](https://github.com/sirenmarkets/SIPs/blob/master/sips/sip-1.md)
---
<!--You can leave these HTML comments in your merged SIP and delete the visible duplicate text guides, they 
will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new SIPs. 
Note that an SIP number will be assigned by an editor. When opening a pull request to submit your SIP, 
please use an abbreviated title in the filename, `sip-draft_title_abbrev.md`. The title should be 44 characters or less.-->
This is the suggested template for new SIPs. Note that an SIP number will be assigned by an editor. When opening 
a pull request to submit your SIP, please use an abbreviated title in the filename, `sip-draft_title_abbrev.md`. 
The title should be 44 characters or less.

## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Simply describe the outcome the proposed 
changes intends to achieve. This should be non-technical and accessible to a casual community member.-->
In order to incentivize usage of the network and increase TVL, a rewards program is proposed to bring users 
to incentivize liquidity providers to provide funds to the network.

## Abstract
<!--A short (~200 word) description of the proposed change, the abstract should clearly describe the proposed 
change. This is what *will* be done if the SIP is implemented, not *why* it should be done or *how* it will be done. 
If the SIP proposes deploying a new contract, write, "we propose to deploy a new contract that will do x".-->
The recommendation is that a reward based on the schedule below in [Si tokens](https://etherscan.io/token/0xD23Ac27148aF6A2f339BD82D0e3CFF380b5093de) 
be placed into the staking contract as a reawrd to liquidity providers during a fixed time window of 84 days for both the 
WBTC and USDC pools. This is 3.8% of the total supply of tokens and strikes the right balance to incentivize early players. An illustrative
set of values is placed for reference. Its recommended these pools be unlocked as TVL increases.

| Total Si Reward | Value at $0.25 | Value at $0.50 | Value at $0.75 | Value at $1.00  |
|-----------------|----------------|----------------|----------------|-----------------|
|          50,000 |        $12,500 |        $25,000 |        $37,500 |         $50,000 |
|         100,000 |        $25,000 |        $50,000 |        $75,000 |        $100,000 |
|         150,000 |        $37,500 |        $75,000 |       $112,500 |        $150,000 |
|         200,000 |        $50,000 |       $100,000 |       $150,000 |        $200,000 |
|       2,500,000 |       $625,000 |     $1,250,000 |     $1,875,000 |      $2,500,000 |
|         800,000 |       $200,000 |       $400,000 |       $600,000 |        $800,000 |

## Motivation
<!--This is the problem statement. This is the *why* of the SIP. It should clearly explain *why* the current state 
of the protocol is inadequate.  It is critical that you explain *why* the change is needed, if the SIP proposes changing 
how something is calculated, you must address *why* the current calculation is innaccurate or wrong. This is not the 
place to describe how the SIP will address the issue!-->
Currently there is no reward to drive liquidity to the platform. Major defi platforms such 
as [Uniswap](https://www.coindesk.com/uniswap-dharma-retroactive-uni-airdrop-defi-governance) and 
[Synthetix](https://blog.synthetix.io/what-you-need-to-know-before-staking-snx-for-the-first-time/) provide rewards 
to incentivize usage of the platform, this drives liquidity into those platforms. In order to be competitive in the defi 
market, a grant program using the Synthetix [staking](https://github.com/Synthetixio/synthetix/blob/v2.27.2/contracts/StakingRewards.sol) and [distribution](https://github.com/Synthetixio/synthetix/blob/v2.27.2/contracts/RewardsDistribution.sol) contracts would help drive liquidity to the Siren markets pools.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
