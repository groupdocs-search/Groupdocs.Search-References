---
title: add_to_all method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified attributes to all documents in the index."
type: docs
url: /python-net/groupdocs.search.common/attributechangebatch/add_to_all/
is_root: false
weight: 1020
---


## add_to_all {#attributes}

Adds the specified attributes to all documents in the index.

```python
def add_to_all(self, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| attributes | `list[str]` | The attributes to add. |

### Example

```python
    from groupdocs.search.common import AttributeChangeBatch

    batch = AttributeChangeBatch()
    batch.add_to_all(["public"])
    ```

### Aliases

These names call `add_to_all` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_to_all_files` | `add_to_all_files(attributes)` |
| `add_to_all_strings` | `add_to_all_strings(attributes)` |

### See Also
* class [`AttributeChangeBatch`](/search/python-net/groupdocs.search.common/attributechangebatch/)
