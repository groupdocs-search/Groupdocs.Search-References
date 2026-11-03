---
title: get_text method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns the text associated with the specified alias."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/get_text/
is_root: false
weight: 1070
---


## get_text {#alias}

Returns the text associated with the specified alias.

```python
def get_text(self, alias):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alias | `str` | The alias to locate in the `AliasDictionary` object. |

**Returns:** str or None: The text associated with the specified alias, or `None` if the alias does not exist.

| Raises | Description |
| :- | :- |
| `ValueError` | If `alias` is `None`. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
aliases = index.dictionaries.alias_dictionary
aliases.add("e", "(Einstein OR Albert)")

if aliases.contains("e"):
    replacement = aliases.get_text("e")
    print(replacement)  # "(Einstein OR Albert)"
```

### Aliases

These names call `get_text` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_text_file` | `get_text_file(alias)` |
| `get_text_string` | `get_text_string(alias)` |

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
