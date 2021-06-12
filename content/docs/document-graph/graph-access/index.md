---
title: "Querying the Graph"
description: "The Graph is available from smart contracts and via GraphQL"
lead: "The Graph is available from smart contracts and via GraphQL"
date: 2021-02-18T10:43:15-05:00
lastmod: 2021-02-18T10:43:15-05:00
draft: false
images: []
menu: 
  docs:
    parent: "document-graph"
weight: 220
toc: true
---

### Query
#### Smart Contracts
The graph is highly indexed in order to support fast query access from within smart contracts. Any content within the graph can be accessed without iteration and ```O(1)``` performance.

```
<example on-chain graph query>
```

#### GraphQL
The graph is cached off-chain using DGraph and can be queried using GraphQL.

```
<example graphql query>
```

### Graph navigation
There is a GUI and CLI that enables general purpose graph navigation of the on-chain graph. 

Graph viewer allows the user to select a document and view the contents on the side panel.

{{< img-simple src="graph-viewer.png" alt="Square" class="border-0 rounded-circle" >}}

```daoctl``` offers a CLI-based graph navigator.

{{< img-simple src="daoctl-graph-navigation.png" alt="Square" class="border-0 rounded-circle" >}}

