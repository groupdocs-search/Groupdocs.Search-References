---
title: optimize method
second_title: GroupDocs.Search for Python via .NET API References
description: "Minimizes the number of index segments by merging them, improving search performance."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/optimize/
is_root: false
weight: 1170
---


## optimize {#options}

Minimizes the number of index segments by merging them, improving search performance.

Optimization merges the index segments of each shard, reducing their count and physically removing data of deleted documents. This is especially useful after many indexing operations that add new segments.

```python
def optimize(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `OptimizeOptions` | The optimize options (`OptimizeOptions`). |

### Example

```python
from groupdocs.search.options import OptimizeOptions

# `node` is the master node of a configured and started search network
indexer = node.indexer

# Merge the index segments of each shard
indexer.optimize(OptimizeOptions())
```

### Aliases

These names call `optimize` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `optimize_optimize_options` | `optimize_optimize_options(options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
