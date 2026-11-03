---
title: search_next method
second_title: GroupDocs.Search for Python via .NET API References
description: "Continues a search in the distributed search index."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/search_next/
is_root: false
weight: 1060
---


## search_next {#network_search_token}

Continues a search in the distributed search index.

```python
def search_next(self, network_search_token):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| network_search_token | `NetworkSearchToken` | The network search token. |

**Returns:** GroupDocs.Search.SearchResult: The search result.

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions

index = Index("./index")
options = SearchOptions()
options.is_chunk_search = True

# Perform the initial search to obtain the first chunk and a token for the next chunk
result = index.search("Einstein", options)
while result.next_chunk_search_token is not None:
    result = index.search_next(result.next_chunk_search_token)
    print(f"Found {result.document_count} documents in this chunk.")
```

## search_next {#network_image_search_token}

Continues a reverse image search in the distributed search index.

```python
def search_next(self, network_image_search_token):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| network_image_search_token | `NetworkImageSearchToken` | The network image search token. |

**Returns:** GroupDocs.Search.Scaling.NetworkImageSearchResult: The reverse image search result.

### Example

```python
    from groupdocs.search import Index
    from groupdocs.search.options import SearchOptions

    index = Index("./index")
    index.add("./documents")
    options = SearchOptions()
    options.is_chunk_search = True

    # Perform the initial search to obtain the first chunk and a token for the next chunk
    result = index.search("Einstein", options)
    while result.next_chunk_search_token is not None:
        result = index.search_next(result.next_chunk_search_token)
        print("Documents found in this chunk:", result.document_count)
    ```

### Aliases

These names call `search_next` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_next_network_search_token` | `search_next_network_search_token(network_search_token)` |
| `search_next_network_image_search_token` | `search_next_network_image_search_token(network_image_search_token)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
