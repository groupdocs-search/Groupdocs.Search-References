---
title: TableDiscreteFunction class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the fuzzy search algorithm that contains correspondences between word lengths and the number of allowed mistakes."
type: docs
url: /python-net/groupdocs.search.options/tablediscretefunction/
is_root: false
weight: 420
---


## TableDiscreteFunction class

Represents the fuzzy search algorithm that contains correspondences between word lengths and the number of allowed mistakes.

Learn more:
- https://docs.groupdocs.com/search/python-net/fuzzy-search/

The TableDiscreteFunction type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/tablediscretefunction/__init__/#offset_of_inputs-table_of_outputs) | Initializes a new TableDiscreteFunction instance. |
| [__init__](/search/python-net/groupdocs.search.options/tablediscretefunction/__init__/#first_step_level-steps) | Initializes a new TableDiscreteFunction. |

### Methods
| Method | Description |
| :- | :- |
| [get_max_mistake_count](/search/python-net/groupdocs.search.options/tablediscretefunction/get_max_mistake_count/#term_length) | Returns the maximum allowed number of mistakes for the specified term length. |
| [get_similarity_level](/search/python-net/groupdocs.search.options/tablediscretefunction/get_similarity_level/#term_length) | Gets a similarity level for the specified term length. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions, TableDiscreteFunction, Step

index = Index("./index")
index.add("./documents")

options = SearchOptions()
options.fuzzy_search.enabled = True
# Use a step function: max 1 mistake for words 1‑4 characters,
# 2 mistakes for 5‑7 characters, and 3 mistakes for 8+ characters.
options.fuzzy_search.fuzzy_algorithm = TableDiscreteFunction(1, [Step(5, 2), Step(8, 3)])

result = index.search("Einstein", options)
print(result.document_count)
```

### Guides
Task guides that use `TableDiscreteFunction`:

* [Work with search results](/search/python-net/guides/work-with-search-results/)
* [Fuzzy search](/search/python-net/guides/fuzzy-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
