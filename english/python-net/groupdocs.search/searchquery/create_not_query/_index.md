---
title: create_not_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates an inverted query that matches all documents not matching the specified query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_not_query/
is_root: false
weight: 1040
---


## create_not_query {#query}

Creates an inverted query that matches all documents not matching the specified query.

```python
def create_not_query(cls, query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The query to invert. |

**Returns:** A combined NOT query.

### Example

```python
from groupdocs.search import SearchQuery

# Create a word query for "Einstein"
einstein_query = SearchQuery.create_word_query("Einstein")

# Invert the query to find documents that do NOT contain "Einstein"
not_query = SearchQuery.create_not_query(einstein_query)

# Combine with another query using AND
relativity_query = SearchQuery.create_word_query("relativity")
combined_query = SearchQuery.create_and_query(relativity_query, not_query)

# Execute the search
results = index.search(combined_query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
