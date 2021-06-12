---
title: "Payments"
description: "Proposals allow team members to put their ideas to a vote"
lead: ""
date: 2021-02-18T10:43:15-05:00
lastmod: 2021-02-18T10:43:15-05:00
draft: false
images: []
menu: 
  docs:
    parent: "platform"
weight: 150
toc: true
---

The platform supports endless tokenomic and payment opportunities. Here is what we have seen work the best.

#### Reward tokens
Reward tokens are transferable, fungible tokens that are paid to donors, investors, and contributors as a reward in exchange for something of value provided to the organization.

For a reward token to be valuable, it should have a purpose. For example, an open source software team may pay their reward token to their contributors.  

The reward token is also used (burned) when new users are granted access to a hosted instance of their software (freemium model).  This creates demand for their token. The users must purchase the token from the earners, which is they are rewarded for their contributions.

It creates a full economic cycle that allows the community of users to fund continued innovation of the software they use.

#### Escrow payments
Payments can be made as liquid tokens, meaning there are no restrictions are transferability (or selling). Payments may also be made as escrowed tokens. 

Escrowed tokens are still owned by the holder and show in their balances, but they cannot be transfered until they are unlocked. Escrow payments are set to be unlocked based on one of the following criteria:

  - Unlocked automatically on a specific date
  - Unlocked based on an event approval, as approved by voters

Event-based escrow is commonly used for milestones. For example, a software team may escrow 25% of all payments as it is earned, and these tokens may be assigned to a series of milestones that must be voted on by the token holders.

Escrow payments help to keep organizations aligned around common goals.

#### Non-transferable governance tokens
Non-transferable governance tokens may also be issued as payment. This token balance may be used to represent voting power on proposals. 

### Example Configuration
Here's an example of a common configuration for assignment-based, salary payments. Although it seems complex, it creates an effective mix of incentives to attract and reward team members in an aligned manner.
- Members claims pay once per week
- 20% of Reward token salary paid in liquid form
- 30% of Reward token salary paid to event-based escrow (e.g. software "golive")
- Payment of non-transferable voting tokens
- 50% of salary paid in a USD-compatible, liquid peg token

This level of flexibility is powerful because handling incentives in a meaningful way is paramount to driving successful teamwork. The example member earns voting power to influence future proposals, escrow tokens to keep her incentivized to see through to the end of the project, liquid reward tokens that can be transferred, and a USD-based stablecoin that can be exchanged immediately so that the member can support day-to-day needs such as groceries and rent.



