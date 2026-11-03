---
title: add method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified pair of alias and associated text to this instance of the AliasDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/add/
is_root: false
weight: 1010
---


## add {#alias-text}

Adds the specified pair of alias and associated text to this instance of the AliasDictionary.

```python
def add(self, alias, text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alias | `str` | The alias to add to the dictionary. |
| text | `str` | The text to be associated with the alias. |

| Raises | Description |
| :- | :- |
| `ValueError` | If `alias` contains characters outside the ranges a‑z and 0‑9. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
aliases = index.dictionaries.alias_dictionary
aliases.add("usa", "United States of America")
```

### Aliases

These names call `add` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_file` | `add_file(alias, text)` |
| `add_string` | `add_string(alias, text)` |

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
