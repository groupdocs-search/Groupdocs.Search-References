---
title: optimize method
second_title: GroupDocs.Search for Python via .NET API References
description: "Minimizes the number of index segments by merging them, improving search performance."
type: docs
url: /python-net/groupdocs.search/index/optimize/
is_root: false
weight: 1180
---


## optimize

Minimizes the number of index segments by merging them, improving search performance.

An index optimization operation reduces the number of segments in an index, thereby increasing search performance. Each indexing operation adds at least one new segment, so indexes that receive frequent document additions should be optimized periodically.

```python
def optimize(self):
    ...
```

### Example

```python
from groupdocs.search import Index

# Create or open an index
index = Index("./index")

# Add documents to the index (each call creates at least one new segment)
index.add("./documents")

# Re-index only documents changed since the last add/update
index.update()

# Merge segments for faster subsequent searches
index.optimize()
```

## optimize {#options}

Minimizes the number of index segments by merging them, improving search performance.

An index optimization operation reduces the number of segments in an index, thereby increasing search performance. Each indexing operation adds at least one new segment, so indexes that receive frequent document additions should be optimized periodically.

```python
def optimize(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `MergeOptions` | The merge options. |

### Aliases

These names call `optimize` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `optimize_merge_options` | `optimize_merge_options(options)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
