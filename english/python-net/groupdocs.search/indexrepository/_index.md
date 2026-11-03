---
title: IndexRepository class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a container for combining multiple indexes and performing common operations on them."
type: docs
url: /python-net/groupdocs.search/indexrepository/
is_root: false
weight: 50
---


## IndexRepository class

Represents a container for combining multiple indexes and performing common operations on them.

- Search index repository (https://docs.groupdocs.com/search/python-net/search-index-repository/)

The IndexRepository type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search/indexrepository/__init__/) | Initializes a new instance of the [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/) class. |

### Methods
| Method | Description |
| :- | :- |
| [add_to_repository](/search/python-net/groupdocs.search/indexrepository/add_to_repository/#index) | Adds an index to the index repository. |
| [add_to_repository](/search/python-net/groupdocs.search/indexrepository/add_to_repository/#index_folder) | Opens and adds an index to the index repository. |
| [create](/search/python-net/groupdocs.search/indexrepository/create/) | Creates a new index in memory. |
| [create](/search/python-net/groupdocs.search/indexrepository/create/#settings) | Creates a new index in memory. |
| [create](/search/python-net/groupdocs.search/indexrepository/create/#index_folder) | Creates a new index on disk, cleaning the index folder before creation. |
| [create](/search/python-net/groupdocs.search/indexrepository/create/#index_folder-settings) | Creates a new index on disk. The index folder will be cleaned before the index creation. |
| [dispose](/search/python-net/groupdocs.search/indexrepository/dispose/) | Releases all resources used by the [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/). |
| [search](/search/python-net/groupdocs.search/indexrepository/search/#query) | Searches in all indexes of the repository. |
| [search](/search/python-net/groupdocs.search/indexrepository/search/#query-options) | Searches in all indexes of the repository. |
| [search](/search/python-net/groupdocs.search/indexrepository/search/#query) | Searches in all indexes of the repository. |
| [search](/search/python-net/groupdocs.search/indexrepository/search/#query-options) | Searches in all indexes of the repository. |
| [update](/search/python-net/groupdocs.search/indexrepository/update/) | Updates all indexes in the repository. |
| [update](/search/python-net/groupdocs.search/indexrepository/update/#options) | Updates all indexes in the repository. |

### Properties
| Property | Description |
| :- | :- |
| [events](/search/python-net/groupdocs.search/indexrepository/events/) | The event hub for subscribing to events. |
| [indexes](/search/python-net/groupdocs.search/indexrepository/indexes/) | The indexes contained in this IndexRepository. |

### Example

```python
from groupdocs.search import IndexRepository

index_folder1 = "./MyIndex"
index_folder2 = "./MyIndex"
query = "Einstein"

repo = IndexRepository()
repo.add_to_repository(index_folder1)  # Load an existing index
repo.add_to_repository(index_folder2)  # Load another existing index

result = repo.search(query)  # Search across all indexes in the repository
```

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
