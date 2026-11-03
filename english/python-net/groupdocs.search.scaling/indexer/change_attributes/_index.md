---
title: change_attributes method
second_title: GroupDocs.Search for Python via .NET API References
description: "Applies the specified batch of attribute changes to indexed documents without reindexing."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/change_attributes/
is_root: false
weight: 1020
---


## change_attributes {#batch-options}

Applies the specified batch of attribute changes to indexed documents without reindexing.

```python
def change_attributes(self, batch, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| batch | `AttributeChangeBatch` | The attribute change batch. |
| options | `ChangeAttributesOptions` | The change attributes options. |

### Example

```python
from groupdocs.search.common import AttributeChangeBatch

# Prepare a batch of attribute changes
batch = AttributeChangeBatch()
# TODO: add attribute changes to the batch, e.g., batch.add(...)

# Apply the changes to the indexer
index.change_attributes(batch)
```

### Aliases

These names call `change_attributes` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `change_attributes_attribute_change_batch` | `change_attributes_attribute_change_batch(batch, options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
