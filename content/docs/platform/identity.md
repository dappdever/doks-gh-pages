---
title: "Identity"
description: "Know your members"
lead: "Know your members"
date: 2021-02-18T10:43:15-05:00
lastmod: 2021-02-18T10:43:15-05:00
draft: false
images: []
menu: 
  docs:
    parent: "platform"
weight: 110
toc: true
---

Modern organizations are borderless, virtual, and asynchronous. The platform features a suite of tools that allow members to know each other, if they want to.

### Account names
We use account names, but not just public keys.

### Profiles
Like all modern social platforms, we support profiles that allow members to describe themselves to the community. The platform uses blockchain authentication and encryption to secure appropriate information in a GDPR compliant manner.

### Double Blind Contact Gateway
It is most common for members to share some contact information, such as their Element or Discord handle, an email, and perhaps even a telephone number.

However, the platform also supports notifications that are sent only *to* a members' blockchain account and is forwarded to that members' preferred contact method. The recipient can then respond to the message and have it routed back to the original sender based on their preferred contact method. Neither party knows the other party's contact information, or even preferred contact method. 

The gateway also supports end-to-end encrypted elements, although the counterparty account name and thread token are required to be readable by the gateway.

### Social Media Proofs
Members can post a cryptographic proof that guarantees the person behind the blockchain account is the same person running a social media or Github account. This protects against Sybil attacks and also creates a sense of trust in your organization.

Identity validators are also available in the community at large to provide additional confidence as required.

