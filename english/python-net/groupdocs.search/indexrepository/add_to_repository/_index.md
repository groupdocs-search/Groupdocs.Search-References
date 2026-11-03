---
title: add_to_repository method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds an index to the index repository."
type: docs
url: /python-net/groupdocs.search/indexrepository/add_to_repository/
is_root: false
weight: 1010
---


## add_to_repository {#index}

Adds an index to the index repository.

```python
def add_to_repository(self, index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index | `Index` | The index to add. |

### Example

```python
from groupdocs.search import Index, IndexRepository

index = Index("./index1")
repo = IndexRepository()
repo.add_to_repository(index)
```

## add_to_repository {#index_folder}

Opens and adds an index to the index repository.

```python
def add_to_repository(self, index_folder):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder. |

### Example

```python
from groupdocs.search import IndexRepository

repo = IndexRepository()
repo.add_to_repository("./index1")
```

### Aliases

These names call `add_to_repository` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_to_repository_index` | `add_to_repository_index(index)` |
| `add_to_repository_file` | `add_to_repository_file(index_folder)` |
| `add_to_repository_string` | `add_to_repository_string(index_folder)` |

### See Also
* class [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/)
