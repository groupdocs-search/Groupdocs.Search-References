---
title: AliasReplacementPair class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an alias/replacement pair."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasreplacementpair/
is_root: false
weight: 20
---


## AliasReplacementPair class

Represents an alias/replacement pair.

See also [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/).

The AliasReplacementPair type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.dictionaries/aliasreplacementpair/__init__/#alias-replacement) | Initializes a new AliasReplacementPair instance. |

### Properties
| Property | Description |
| :- | :- |
| [alias](/search/python-net/groupdocs.search.dictionaries/aliasreplacementpair/alias/) | The alias. |
| [replacement](/search/python-net/groupdocs.search.dictionaries/aliasreplacementpair/replacement/) | The replacement string. |

### Example

```python
from groupdocs.search.dictionaries import AliasReplacementPair

pairs = [
    AliasReplacementPair("d", "daterange(2017-01-01 ~~ 2019-12-31)"),
    AliasReplacementPair("n", "(100 ~~ 900)"),
]
```

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
