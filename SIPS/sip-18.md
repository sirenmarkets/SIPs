---
sip: 18
title: Shifting Liquidity Towards Utilization
author: Zareth-San @zareth-san
discussions-to: https://gov.sirenmarkets.com/t/sip-18-shifting-liquidity-towards-utilization/268
status: Draft
type: SIPs
created: 2021-08-31
---

<!--You can leave these HTML comments in your merged SIP and delete the visible duplicate text guides, they will not appear and may be helpful to refer to if you edit it again. This is the suggested template for new SIPs. Note that an SIP number will be assigned by an editor. When opening a pull request to submit your SIP, please use an abbreviated title in the filename, `eip-draft_title_abbrev.md`. The title should be 44 characters or less.-->


## Simple Summary
<!--"If you can't explain it simply, you don't understand it well enough." Provide a simplified and layman-accessible explanation of the SIP.-->
This SIP change some of the parameters defined in [SIP-11](https://gov.sirenmarkets.com/t/sip-11-implement-dynamic-lp-rewards/214) in order to decrease the rewards coming from LP liquidity, and increase the rewards coming from option trading volume. There are 3 particular changes:

1. Reduce the minimum liquidity threshold from $1M to $250K
2. Reduce the steepness of the liquidity rewards function from 10 to 4
3. Reduce the S-point of utilization function from 0.5 to 0.4

## Motivation
<!--The motivation is critical for SIPs that want to change the SIREN protocol. It should clearly explain why the existing protocol specification is inadequate to address the problem that the SIP solves. SIP submissions without sufficient motivation may be rejected outright.-->
With the current parameters from SIP-11, the protocol is over-incentivizing LP liquidity. Our AMM pools have far more liquidity than is currently being used to mint options. It is not a good use of SI rewards to pay for liquidity that's not used, so we should reduce those payouts to fall in line with the actual amount of liquidity we need.

## Specification
<!--The technical specification should describe the syntax and semantics of any new feature.-->
In order to bring the current reward scheme closer to that vision we propose the following:
1. Reduce the minimum liquidity threshold from $1M to $250K. This would drive down yields in pools with low capital and low utilization.
2. Reduce the steepness of the liquidity rewards function from 10 to 4 to preserve the shape of the curve after the liquidity threshold adjustment above.
3. Reduce the S-point of utilization function from 0.5 to 0.4 in order to further incentivize utilization. 

## Rationale
<!--The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->
The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.-->

## Backwards Compatibility
<!--All SIPs that introduce backwards incompatibilities must include a section describing these incompatibilities and their severity. The SIP must explain how the author proposes to deal with these incompatibilities. SIP submissions without a sufficient backwards compatibility treatise may be rejected outright.-->
Whenever this SIP is accepted and a date determined for when to turn it on, we will update the reward code to use the old parameters prior to this date, and these new parameters for all days after the date.

## Test Cases
<!--Test cases for an implementation are mandatory for SIPs that are affecting consenss changes. Other SIPs can choose to include links to test cases if applicable.-->
There are no consensus changes

## Implementation
<!--The implementations must be completed before any SIP is given status "Final", but it need not be completed before the SIP is accepted. While there is merit to the approach of reaching consensus on the specification and rationale before writing code, the principle of "rough consensus and running code" is still useful when it comes to resolving many discussions of API details.-->


## Security Considerations
<!--All SIPs must contain a section that discusses the security implications/considerations relevant to the proposed change. Include information that might be important for security discussions, surfaces risks and can be used throughout the life cycle of the proposal. E.g. include security-relevant design decisions, concerns, important discussions, implementation-specific guidance and pitfalls, an outline of threats and risks and how they are being addressed. SIP submissions missing the "Security Considerations" section will be rejected. An SIP cannot proceed to status "Final" without a Security Considerations discussion deemed sufficient by the reviewers.-->
This is a simple parameter update to non-smart contract code. Security impact is low to non-existent.

## Copyright
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

