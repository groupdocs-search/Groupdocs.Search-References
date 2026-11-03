---
title: update method
second_title: GroupDocs.Search for Python via .NET API References
description: "Updates all indexes in the repository."
type: docs
url: /python-net/groupdocs.search/indexrepository/update/
is_root: false
weight: 1050
---


## update

Updates all indexes in the repository.

```python
def update(self):
    ...
```

### Example

```python
from groupdocs.search import IndexRepository

index_folder = "./MyIndex"
documents_folder = "./documents"

repository = IndexRepository()
index = repository.create(index_folder)  # Creating index
index.add(documents_folder)  # Indexing documents

# Delete, modify, or add documents in the folder as needed

repository.update()
```

## update {#options}

Updates all indexes in the repository.

```python
def update(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `UpdateOptions` | The update options. |

### Example

```python
from groupdocs.search import IndexRepository
from groupdocs.search.options import UpdateOptions

# Create repository and index
repository = IndexRepository()
index = repository.create("./MyIndex")
index.add("./documents")

# Modify documents in the folder as needed, then update the index
options = UpdateOptions()
options.threads = 2  # Number of indexing threads
repository.update(options)
```

### Aliases

These names call `update` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `update_update_options` | `update_update_options(options)` |

### See Also
* class [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/)
