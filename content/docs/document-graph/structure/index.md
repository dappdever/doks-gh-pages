---
title: "Data Model"
description: "Flexible graph of KV pairs"
lead: ""
date: 2021-02-18T10:43:15-05:00
lastmod: 2021-02-18T10:43:15-05:00
draft: false
images: []
menu: 
  docs:
    parent: "document-graph"
weight: 210
toc: true
---

The platform stores on- and off-chain data in a flexible, content-addressed document graph. 

A graph is a set of documents that are connected with labeled, directional edges.

{{< img-simple src="doc-graph-structure.png" alt="Document Graph" class="border-0 rounded-circle" >}}

### Document
A document is comprised of three primary components: 
- a header
- content - an ordered 'list of labeled lists' of key-value pairs
- certificates

##### Header
The document header stores the following:
- creator (blockchain account)
- created_date 
- hash of the contents

The document graph uses content-addressing, which means the unique identifier of the document is a hash of the contents.  See here for the benefits of content-addressing.

##### Content
The content of a document is an ordered list of labeled lists of key-value pairs. Here's a psuedo-code representation:

```
Content:
  Group: Label: 'content-group #1', Sequence: 1
    Item: Key: 'content-item A', Value: 'content-item-value A', Sequence: 1
    Item: Key: 'content-item B', Value: 'content-item-value B', Sequence: 2
    Item: Key: 'content-item C', Value: 'content-item-value C', Sequence: 3
    ...
  Group: Label: 'content-group #2', Sequence: 2
    Item: Key: 'content-item D', Value: 'content-item-value D', Sequence: 1
    Item: Key: 'content-item E', Value: 'content-item-value E', Sequence: 2
    Item: Key: 'content-item F', Value: 'content-item-value F', Sequence: 3
    ...
  ...
```

The ```content-item-values``` can be of any native EOSIO data type. Any data that can be stored within a smart contract can be stored within a document. 

##### Certificates
Certificates represent an attestation by any available authorization on-chain, which could be an organization member, group of members, any outside party, etc. 

A certificates is comprised of: 
- certified_date
- permission used to certify (the account)
- notes, any abitrary screen added by the certifier

### Edges

Edges are a labeled, directional link between two documents. Edges are also content-addressed across the ``from-document```, ```to-document```, and ```edge-name```.  Other than that, there are no limitations on cardinality and uniqueness.

Edges are not scored, or ranked, as in some graph theory, but this is something we may add in the future.

Edges are indexed based on every combination of ``from-document```, ```to-document```, and ```edge-name```, and also by ```created_date``` and ```creator```.

### Merkle tree
A document graph enjoys all of the benefits of being a merkle tree, including verification by its merkle root.

#### Badge and membership example
Here is an example of how the graph is used for organizational membership, badges, and payments.

{{< img-simple src="graph-example.png" alt="Document Graph" class="border-0 rounded-circle" >}}
