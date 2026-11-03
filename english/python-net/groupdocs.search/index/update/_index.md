---
title: update method
second_title: GroupDocs.Search for Python via .NET API References
description: "Re-indexes documents that have been changed or deleted since the last update and adds new files that have been added to the indexed folders."
type: docs
url: /python-net/groupdocs.search/index/update/
is_root: false
weight: 1220
---


## update

Re-indexes documents that have been changed or deleted since the last update and adds new files that have been added to the indexed folders.

The update operation reindexes documents that have been changed, deleted, or added to the indexed folders. Changing the filter specified by the `document_filter` property of the [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/) class can also affect the list of indexed documents.

```python
def update(self):
    ...
```

### Example

```python
    from groupdocs.search import Index

    index_folder = "./MyIndex"
    documents_folder = "./documents"

    index = Index(index_folder)  # Create or open the index
    index.add(documents_folder)  # Index documents from the folder

    # Modify, delete, or add files in the documents folder as needed

    index.update()  # Re-index changed, deleted, and new documents
    ```
```

## update {#options}

Re-indexes documents that have been changed or deleted since the last update and adds new files that have been added to the indexed folders.

The update operation reindexes modified, removed, or newly added documents in the indexed folders. Changing the `document_filter` property of [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/) can also affect which documents are indexed.

```python
def update(self, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `UpdateOptions` | The update options. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import UpdateOptions

index_folder = "./MyIndex"
documents_folder = "./documents"

# Create or open the index in the specified folder
index = Index(index_folder)

# Index documents from the specified folder
index.add(documents_folder)

# Modify, delete, or add documents in the documents folder as needed

# Configure update options (e.g., set the number of indexing threads)
options = UpdateOptions()
options.threads = 2

# Update the index with the specified options
index.update(options)
```

### Aliases

These names call `update` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `update_update_options` | `update_update_options(options)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
