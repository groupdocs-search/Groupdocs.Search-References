---
title: create_phrase_search_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a phrase search query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_phrase_search_query/
is_root: false
weight: 1070
---


## create_phrase_search_query {#queries}

Creates a phrase search query.

```python
def create_phrase_search_query(cls, queries):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| queries | `list[SearchQuery]` | The child queries. |

**Returns:** A phrase search query.

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.options import CommonFieldNames

# Combine individual word and wildcard queries into a phrase query
word1 = SearchQuery.create_word_query("theory")
word2 = SearchQuery.create_word_query("of")
wildcard = SearchQuery.create_wildcard_query(0, 1)  # matches any single token
word3 = SearchQuery.create_word_query("relativity")
phrase_query = SearchQuery.create_phrase_search_query(word1, word2, wildcard, word3)

# Use the phrase query in a field query
field_query = SearchQuery.create_field_query(CommonFieldNames.CONTENT, phrase_query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
