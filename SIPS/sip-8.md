---
  sip: 8
  title: LPP Extension and Vesting Schedule
  author: Zareth San (@zareth-san)
  comments-uri: https://gov.sirenmarkets.com/t/sip-8-lpp-extension-and-vesting-schedule/157
  status: Proposed
  type: SIPs
  created: 2020-02-23
---

## Simple Summary

The first SIREN Liquidity Provider Program (LPP) will end on Feb 26, 2021. SIP-6 7 suggested a new, second Liquidity Provider Program that releases 1MM SI over 90 days. This SIP (8) suggests releasing 1.5MM SI over a 13-week program. The goal of this new program is to bring liquidity to new asset pools on SIREN, beginning with the SUSHI pool and expanding into more DeFi assets over the course of the program.

If the SIREN LBP occurs the week of March 1, for price discovery to occur there cannot be any tokens in the market prior to the token generation event. Therefore, no SI rewards from either program will unlock before March 5.

The original vesting schedule for LP rewards was planned to be a 3-month linear vesting schedule. However, community members have expressed a desire to receive more tokens upfront. This SIP suggests a vesting schedule of 50% upfront tokens and 50% 12 week linear vesting for rewards earned prior to the March 5, 16:00 UTC launch. This will allow LPs earlier access to their rewards. Rewards from the second LPP for weeks after the launch (the last 12 weeks of the 13 week LPP extension) will be claimable immediately, i.e. there will be no vesting for rewards.

## Abstract

A new LPP will begin on Friday, Feb 26 at 16:00 UTC and continue until Friday, May 28 at 15:59 UTC, for 13 weeks total. 1.5MM SI will be released over the course of the program.

The vesting schedule for the LPP proposed in SIP-2 4, plus the first week of the LPP extension prior to launch, will be set to 50% upfront rewards and 50% distribution over a 12 week linear vesting schedule. Claiming will begin on Friday, March 5, one week after the end of the existing LPP.

There will be no vesting for the rewards earned after the launch (March 5), and for the rewards earned prior to the launch those will be 50% immediately claimable, with the remaining 50% vesting over 12 weeks. For example, on Friday, March 12, one week into the 12 week linear vesting period, participants in the LPP will be able to claim 50% upfront and 1/12 of the remaining rewards after claiming 50%. Participants in the second LPP will be able to claim all of the rewards earned from March 5 to March 12 immediately.

Rewards for the new LPP during the week of February 26 to March 12 will be distributed among the USDC, WBTC, and SUSHI pools equally. Starting on March 12 at 16:00 UTC, rewards will no longer be distributed to the WBTC pools. As new DeFi asset pools are added, rewards will be divided equally among the pools exclusive of WBTC.

## Motivation

The goal of the new LPP is to drive liquidity into the new DeFi asset pools away from WBTC. SIREN can differentiate itself as a project by providing financial products for popular assets that are not supported on other platforms such as Deribit.

In addition, community members have expressed a desire to modify the existing 3-month linear vesting schedule to receive more tokens upfront. While some comments 2 on SIP 6 suggest a desire for a longer vesting schedule, response on the SIREN telegram has been overwhelmingly in favor of more upfront tokens.