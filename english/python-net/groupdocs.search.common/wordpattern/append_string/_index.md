---
title: append_string method
second_title: GroupDocs.Search for Python via .NET API References
description: "Appends a string to the word pattern."
type: docs
url: /python-net/groupdocs.search.common/wordpattern/append_string/
is_root: false
weight: 1040
---


## append_string {#text}

Appends a string to the word pattern.

The string is appended as UTF-16 code units rather than as code points, which is how the terms of an index are stored. A character above the basic plane therefore becomes the pair of its surrogates and is searched for as such. Appending it as a single code point would have set the bit that marks a wildcard and turned the character into one.

```python
def append_string(self, text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text | `str` | The string to append. |

### Example

```python
from groupdocs.search.common import WordPattern

pattern = WordPattern()
pattern.append_string("card")
```

### Aliases

These names call `append_string` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `append_string_file` | `append_string_file(text)` |
| `append_string_string` | `append_string_string(text)` |

### See Also
* class [`WordPattern`](/search/python-net/groupdocs.search.common/wordpattern/)
