---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new AliasReplacementPair instance."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasreplacementpair/__init__/
is_root: false
weight: 10
---


## __init__ {#alias-replacement}

Initializes a new AliasReplacementPair instance.

```python
def __init__(self, alias, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alias | `str` | The alias to be replaced. |
| replacement | `str` | The replacement. |

### Example

```python
    from groupdocs.search.dictionaries import AliasReplacementPair

    pairs = [
        AliasReplacementPair("d", "daterange(2017-01-01 ~~ 2019-12-31)"),
        AliasReplacementPair("n", "(100 ~~ 900)"),
    ]
    ```

### See Also
* class [`AliasReplacementPair`](/search/python-net/groupdocs.search.dictionaries/aliasreplacementpair/)
