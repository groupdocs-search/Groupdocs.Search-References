---
title: search_first method
second_title: GroupDocs.Search for Python via .NET API References
description: "Starts a search with a query in text form in the distributed search index."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/search_first/
is_root: false
weight: 1050
---


## search_first {#query-options}

Starts a search with a query in text form in the distributed search index.

```python
def search_first(self, query, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `str` | The search query. |
| options | `SearchOptions` | The search options. |

**Returns:** NetworkSearchResult: The search result.

### Example

```python
from groupdocs.search.options import SearchOptions

# `node` is the master node of a configured and started search network
searcher = node.searcher

options = SearchOptions()
options.is_chunk_search = True  # a search network searches by chunks only

result = searcher.search_first("einstein", options)
print("Documents found:", result.document_count)
```

## search_first {#query-options}

Starts a search with a query object in the distributed search index.

```python
def search_first(self, query, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The search query. |
| options | `SearchOptions` | The search options. |

**Returns:** The search result.

### Example

```python
# Assuming `searcher` is an instance of Searcher, and `query` and `options` are prepared:
result = searcher.search_first(query, options)
```

## search_first {#image-options}

Starts a reverse image search in the distributed search index.

```python
def search_first(self, image, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image | `SearchImage` | The image to search. |
| options | `ImageSearchOptions` | The image search options. |

**Returns:** NetworkImageSearchResult: The reverse image search result.

### Example

```python
from groupdocs.search.options import ImageSearchOptions
from groupdocs.search.scaling import Searcher

# Assume `searcher` is an initialized Searcher instance and `image` is a loaded image.
result = searcher.search_first(image, ImageSearchOptions())
# `result` is a NetworkImageSearchResult containing the images found in one shard.
```

### Aliases

These names call `search_first` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_first_file` | `search_first_file(query, options)` |
| `search_first_string` | `search_first_string(query, options)` |
| `search_first_search_query` | `search_first_search_query(query, options)` |
| `search_first_search_image` | `search_first_search_image(image, options)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
