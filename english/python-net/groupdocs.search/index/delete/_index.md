---
title: delete method
second_title: GroupDocs.Search for Python via .NET API References
description: "Deletes indexed files or folders from the index and updates the index without the deleted paths."
type: docs
url: /python-net/groupdocs.search/index/delete/
is_root: false
weight: 1040
---


## delete {#paths-options}

Deletes indexed files or folders from the index and updates the index without the deleted paths.

Note that an individual document cannot be deleted from the index if it was added as part of a folder.

```python
def delete(self, paths, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| paths | `list[str]` | The paths to files or folders to delete. |
| options | `UpdateOptions` | The update options. |

**Returns:** DeleteResult: An object describing the result of deleting files or folders from the index.

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import UpdateOptions

index_folder = "./MyIndex"
documents_folder1 = "./documents"
documents_folder2 = "./documents2"

# Create an index in the specified folder
index = Index(index_folder)

# Index documents from the specified folders
index.add(documents_folder1)
index.add(documents_folder2)

# Get indexed paths
indexed_paths1 = index.get_indexed_paths()
print("Indexed paths:")
for path in indexed_paths1:
    print("\t", path)

# Delete a path from the index
delete_result = index.delete([documents_folder1], UpdateOptions())
print("\nDeleted paths:", delete_result.success_count)

# Get indexed paths after deletion
indexed_paths2 = index.get_indexed_paths()
print("\nIndexed paths:")
for path in indexed_paths2:
    print("\t", path)
```

## delete {#options-document_keys}

Deletes documents indexed from streams or structures and updates the index without the deleted documents.

```python
def delete(self, options, document_keys):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| options | `UpdateOptions` | The update options. |
| document_keys | `list[str]` | The keys of documents added from streams or structures. |

**Returns:** An object describing the result of deleting documents from the index.

### Aliases

These names call `delete` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `delete_files` | `delete_files(paths, options)`<br>`delete_files(options, document_keys)` |
| `delete_strings` | `delete_strings(paths, options)`<br>`delete_strings(options, document_keys)` |
| `delete_update_options` | `delete_update_options(options, document_keys)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
