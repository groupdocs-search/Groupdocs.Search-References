---
title: append_zero_or_one_character_wildcard method
second_title: GroupDocs.Search for Python via .NET API References
description: "Appends a zero-or-one character wildcard to the word pattern."
type: docs
url: /python-net/groupdocs.search.common/wordpattern/append_zero_or_one_character_wildcard/
is_root: false
weight: 1070
---


## append_zero_or_one_character_wildcard

Appends a zero-or-one character wildcard to the word pattern.

The wildcard matches either no character or a single character, represented as `?(0~1)` in the textual query syntax. Known characters are converted to lower case because words are stored in lower case in the index.

```python
def append_zero_or_one_character_wildcard(self):
    ...
```

### Example

```python
from groupdocs.search import Index, SearchQuery
from groupdocs.search.common import WordPattern

pattern = WordPattern()
pattern.append_string("m")
pattern.append_zero_or_one_character_wildcard()
pattern.append_string("rry")
query = SearchQuery.create_word_pattern_query(pattern)
result = index.search(query)
```

### See Also
* class [`WordPattern`](/search/python-net/groupdocs.search.common/wordpattern/)
