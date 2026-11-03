---
title: synchronize method
second_title: GroupDocs.Search for Python via .NET API References
description: "Synchronizes the list of indexed documents with those on shards."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/synchronize/
is_root: false
weight: 1190
---


## synchronize {#options}

Synchronizes the list of indexed documents with those on shards.

This operation fixes issues with indexing and deletion of documents that resulted from communication problems with the search network nodes.

```python
def synchronize(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `SynchronizeOptions` | The synchronize options. |

### Example

```python
from groupdocs.search.options import SynchronizeOptions

# Assuming `indexer` is an instance of `Indexer` obtained from a configured node
options = SynchronizeOptions()
indexer.synchronize(options)
```

### Aliases

These names call `synchronize` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `synchronize_synchronize_options` | `synchronize_synchronize_options(options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
