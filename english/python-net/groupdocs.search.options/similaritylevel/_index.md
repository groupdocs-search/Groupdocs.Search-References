---
title: SimilarityLevel class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an algorithm of the fuzzy search that specifies the similarity level."
type: docs
url: /python-net/groupdocs.search.options/similaritylevel/
is_root: false
weight: 370
---


## SimilarityLevel class

Represents an algorithm of the fuzzy search that specifies the similarity level.

Learn more
- Fuzzy search: https://docs.groupdocs.com/search/python-net/fuzzy-search/

The SimilarityLevel type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/similaritylevel/__init__/#value) | Initializes a new SimilarityLevel instance. |

### Methods
| Method | Description |
| :- | :- |
| [get_max_mistake_count](/search/python-net/groupdocs.search.options/similaritylevel/get_max_mistake_count/#term_length) | Gets the maximum allowed number of mistakes for the specified term length. |
| [get_similarity_level](/search/python-net/groupdocs.search.options/similaritylevel/get_similarity_level/#term_length) | Gets the similarity level value for the specified term length. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions, SimilarityLevel

index = Index("./index")
index.add("./documents")
options = SearchOptions()
options.fuzzy_search.enabled = True
options.fuzzy_search.fuzzy_algorithm = SimilarityLevel(0.8)  # 0.0 loose .. 1.0 strict
result = index.search("contarct", options)
print(result.document_count)
```

### Guides
Task guides that use `SimilarityLevel`:

* [Fuzzy search](/search/python-net/guides/fuzzy-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
