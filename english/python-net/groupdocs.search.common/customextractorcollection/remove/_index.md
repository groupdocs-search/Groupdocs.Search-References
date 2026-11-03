---
title: remove method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes an extractor from the collection."
type: docs
url: /python-net/groupdocs.search.common/customextractorcollection/remove/
is_root: false
weight: 1070
---


## remove {#extractor}

Removes an extractor from the collection.

```python
def remove(self, extractor):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| extractor | `IFieldExtractor` | The extractor to remove from the collection. |

**Returns:** bool: True if `extractor` was successfully removed from the collection; otherwise, False. This method also returns False if `extractor` is not found in the original collection.

### Aliases

These names call `remove` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_ifield_extractor` | `remove_ifield_extractor(extractor)` |

### See Also
* class [`CustomExtractorCollection`](/search/python-net/groupdocs.search.common/customextractorcollection/)
