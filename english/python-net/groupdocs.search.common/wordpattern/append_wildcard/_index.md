---
title: append_wildcard method
second_title: GroupDocs.Search for Python via .NET API References
description: "Appends a wildcard to the word pattern."
type: docs
url: /python-net/groupdocs.search.common/wordpattern/append_wildcard/
is_root: false
weight: 1050
---


## append_wildcard {#min-max}

Appends a wildcard to the word pattern.

Appends a wildcard for the specified minimum and maximum numbers of characters (?(min~max) in text form). Both values must be in the range from 0 to 255, and the minimum must not be greater than the maximum; otherwise, a ValueError is raised.

```python
def append_wildcard(self, min, max):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| min | `int` | The minimum number of characters. |
| max | `int` | The maximum number of characters. |

| Raises | Description |
| :- | :- |
| `ValueError` | If `min` or `max` is outside the range 0‑255 or if `min` is greater than `max`. |

### Example

```python
from groupdocs.search.common import WordPattern

pattern = WordPattern()
pattern.append_string("card")
pattern.append_wildcard(1, 6)  # matches "cardiff", "cardinal", "cardio", etc.
```

### Aliases

These names call `append_wildcard` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `append_wildcard_int32` | `append_wildcard_int32(min, max)` |

### See Also
* class [`WordPattern`](/search/python-net/groupdocs.search.common/wordpattern/)
