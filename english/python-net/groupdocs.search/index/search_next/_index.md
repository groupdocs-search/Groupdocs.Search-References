---
title: search_next method
second_title: GroupDocs.Search for Python via .NET API References
description: "Continues the chunk search started with method Search."
type: docs
url: /python-net/groupdocs.search/index/search_next/
is_root: false
weight: 1210
---


## search_next {#chunk_search_token}

Continues the chunk search started with method Search.

```python
def search_next(self, chunk_search_token):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| chunk_search_token | `ChunkSearchToken` | The chunk search token. |

**Returns:** SearchResult: The search result.

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions

index = Index("./index")
index.add("./documents")
options = SearchOptions()
options.is_chunk_search = True

result = index.search("Einstein", options)
document_count = result.document_count
while result.next_chunk_search_token is not None:
    result = index.search_next(result.next_chunk_search_token)
    document_count += result.document_count
print("Documents found:", document_count)
```

## search_next {#chunk_search_token-cancellation}

Continues the chunk search started with [`Index.search`](/search/python-net/groupdocs.search/index/search/).

```python
def search_next(self, chunk_search_token, cancellation):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| chunk_search_token | `ChunkSearchToken` | The chunk search token. |
| cancellation | `Cancellation` | The cancellation object. |

**Returns:** SearchResult: The search result.

### Aliases

These names call `search_next` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_next_chunk_search_token` | `search_next_chunk_search_token(chunk_search_token, cancellation)`<br>`search_next_chunk_search_token(chunk_search_token)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
