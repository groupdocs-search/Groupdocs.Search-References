---
title: create_wildcard_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a wildcard for the phrase search."
type: docs
url: /python-net/groupdocs.search/searchquery/create_wildcard_query/
is_root: false
weight: 1090
---


## create_wildcard_query {#count}

Creates a wildcard for the phrase search.

```python
def create_wildcard_query(cls, count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| count | `int` | The number of words in the wildcard. |

**Returns:** SearchQuery: A wildcard for the phrase search.

## create_wildcard_query {#min_count-max_count}

Creates a wildcard for the phrase search.

```python
def create_wildcard_query(cls, min_count, max_count):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| min_count | `int` | The minimum number of words in the wildcard. |
| max_count | `int` | The maximum number of words in the wildcard. |

**Returns:** GroupDocs.Search.WildcardQuery: A wildcard for the phrase search.

### Example

```python
from groupdocs.search import SearchQuery

# Create a wildcard that matches between 1 and 2 words
wildcard = SearchQuery.create_wildcard_query(1, 2)

# Use it in a phrase query
word1 = SearchQuery.create_word_query("theory")
word3 = SearchQuery.create_word_query("relativity")
phrase = SearchQuery.create_phrase_search_query(word1, wildcard, word3)
```

### Aliases

These names call `create_wildcard_query` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_wildcard_query_int32` | `create_wildcard_query_int32(min_count, max_count)`<br>`create_wildcard_query_int32(count)` |

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
