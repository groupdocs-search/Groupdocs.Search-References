---
title: append_one_character_wildcard method
second_title: GroupDocs.Search for Python via .NET API References
description: "Appends a wildcard for exactly one character to the word pattern."
type: docs
url: /python-net/groupdocs.search.common/wordpattern/append_one_character_wildcard/
is_root: false
weight: 1020
---


## append_one_character_wildcard

Appends a wildcard for exactly one character to the word pattern.

```python
def append_one_character_wildcard(self):
    ...
```

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.common import WordPattern

pattern = WordPattern()
pattern.append_string("m")
pattern.append_one_character_wildcard()
pattern.append_string("rry")
query = SearchQuery.create_word_pattern_query(pattern)
result = index.search(query)
```

### See Also
* class [`WordPattern`](/search/python-net/groupdocs.search.common/wordpattern/)
