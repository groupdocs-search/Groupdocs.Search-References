---
title: get_child method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets a child query by its index."
type: docs
url: /python-net/groupdocs.search/searchquery/get_child/
is_root: false
weight: 1120
---


## get_child {#index}

Gets a child query by its index.

```python
def get_child(self, index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index | `int` | The index. |

**Returns:** SearchQuery: A child query corresponding to the specified index.

### Example

```python
    for i in range(phrase_query.child_count):
        child = phrase_query.get_child(i)
        print("\t" + child.to_string() + " (field: " + str(child.field_name) + ")")
    ```

### Aliases

These names call `get_child` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_child_int32` | `get_child_int32(index)` |

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
