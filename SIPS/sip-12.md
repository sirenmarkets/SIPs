---
  sip: 12
  title: Consolidate USDC liquidity in WETH Puts pool
  author: seafi (@seafi)
  comments-uri: https://gov.sirenmarkets.com/t/sip-12-consolidate-usdc-liquidity-in-weth-puts-pool/230
  status: Proposed
  type: SIPs
  created: 2021-05-22
---



## Abstract

Puts and Calls in crypto are not symmetrically opposite. They serve different purposes:

Calls are typically used to bet on an alpha in a particular project: usage growth, buybacks, new products or partnerships announcements, etc.
Puts, on the other hand, are used to protect against broader market downside movements. It is rare to see traders shorting specific tokens of legitimate projects in this market. Current near-0 open interest in Siren’s Put pools validates this point.
ETH can be seen as a proxy for broader DeFi market index. As such, it would be valuable for Siren community to have a deep liquidity and strike/expirations selection in the ETH Puts pool. This will enable market participants to efficiently hedge their broader market exposure while staying net-bullish on DeFi.

## Proposal

WETH Puts pool, which is denominated in USDC, was launched last week and is currently in a bootstrapping phase. We propose to extract USDC from the unused put pools for other assets and consolidate all of Siren’s Puts liquidity in the WETH pool.

In order to do so we propose to discontinue SI rewards for other puts pools (SUSHI, YFI, UNI) which have 0 or near-0 open interest so far. The rewards will be reallocated to incentivize deeper USDC liquidity in the WETH Puts pool.