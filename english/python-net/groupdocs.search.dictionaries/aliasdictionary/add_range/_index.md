---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of alias/replacement pairs to this AliasDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/add_range/
is_root: false
weight: 1020
---


## add_range {#pairs}

Adds the specified collection of alias/replacement pairs to this AliasDictionary.

```python
def add_range(self, pairs):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pairs | `Iterable[KeyValuePair[str, str]]` | The collection of alias/replacement pairs to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | Raised when `pairs` is None. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
aliases = index.dictionaries.alias_dictionary

# Each pair is an alias and the text that replaces it in queries
aliases.add_range([
    ["d", "daterange(2017-01-01 ~~ 2019-12-31)"],
    ["n", "(100 ~~ 900)"],
])
```

## add_range {#pairs}

Adds the specified collection of alias/replacement pairs to this AliasDictionary.

```python
def add_range(self, pairs):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pairs | `Iterable[AliasReplacementPair]` | The collection of alias/replacement pairs to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | If `pairs` is None. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import AliasReplacementPair

index = Index("./MyIndex")
aliases = index.dictionaries.alias_dictionary
pairs = [
    AliasReplacementPair("d", "daterange(2017-01-01 ~~ 2019-12-31)"),
    AliasReplacementPair("n", "(100 ~~ 900)"),
]
aliases.add_range(pairs)
```

## add_range {#pairs}

Adds the specified collection of alias/replacement pairs to this AliasDictionary.

```python
def add_range(self, pairs):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pairs | `list[AliasReplacementPair]` | The collection of alias/replacement pairs to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | If `pairs` is None. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import AliasReplacementPair

index = Index("./MyIndex")
aliases = index.dictionaries.alias_dictionary
pairs = [
    AliasReplacementPair("d", "daterange(2017-01-01 ~~ 2019-12-31)"),
    AliasReplacementPair("n", "(100 ~~ 900)"),
]
aliases.add_range(pairs)
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_ienumerable` | `add_range_ienumerable(pairs)`<br>`add_range_ienumerable(pairs)` |
| `add_range_alias_replacement_pair` | `add_range_alias_replacement_pair(pairs)` |

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
