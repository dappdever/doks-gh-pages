---
title: "Proposals"
description: "Proposals allow team members to put their ideas to a vote"
lead: "Proposals allow team members to put their ideas to a vote"
date: 2021-02-18T10:43:15-05:00
lastmod: 2021-02-18T10:43:15-05:00
draft: false
images: []
menu: 
  docs:
    parent: "platform"
weight: 135
toc: true
---

Proposals are documents that may have special powers if and when they are passed by the organization.

The one common factor among all proposal types is that they may activate the organizational permission. This is activating full *sudo* permissions for the DAO.

## Policy proposals
Policy proposals are as it sounds. A passing policy proposal uses the organizational permission to attest, or certify, the content that is included within the proposal.

These are most common for organizational constitutions or charters. Policy documents may include many sections or clauses, and they may be modified via a subsequent policy modification proposal. All of the content is stored on chain by default, but we also support uploading files to IPFS and anchoring them into a proposal.

## Role proposals
A role proposal includes the following data:
- Title
- Description
- Salary amounts (per period, per token)
- Available dates (begin and end)
- Minimum commitment (e.g. no less than a 50% commitment)
- Available slots (1 person budgeted? or many?)

When a role is approved, it becomes available for members to apply for.

## Assignment proposals
Members may apply for roles, and this proposal type supports the following information.
- Application text
- Commitment %
- Payment composition (see Payments)
- Begin and end dates

When an assignment proposal passes, the assignee is then able to claim compensation for the approved time period. The salary amounts from the role are automatically pro-rated according to approvals and they are adjusted to the assignee's commitment level.

## Badge proposals
Create a new badge or credential, or assign an existing badge to a member. See Credentials.

## Smart contract upgrades
Proposals may be used to upgrade any smart contracts, although upgrades may also be assigned to a multisig authority of a technical steering committee. 

## Organizational authority
Since proposals activate an organizational authority, they can be used for nearly any transaction on chain that requires that authority. 

The platform supports also rollup proposals, where the final authority requires that a quorum and percentage of sub-organizations independently vote to approve.  

