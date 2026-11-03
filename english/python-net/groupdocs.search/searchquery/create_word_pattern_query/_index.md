---
title: create_word_pattern_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a word pattern query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_word_pattern_query/
is_root: false
weight: 1100
---


## create_word_pattern_query {#pattern}

Creates a word pattern query.

```python
def create_word_pattern_query(cls, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `WordPattern` | The word pattern. |

**Returns:** SearchQuery: A word pattern query.

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.common import WordPattern

# Build a pattern that matches "merry", "marry", etc.
pattern = WordPattern()
pattern.append_string("m")
pattern.append_one_character_wildcard()
pattern.append_string("rry")

query = SearchQuery.create_word_pattern_query(pattern)
result = index.search(query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
