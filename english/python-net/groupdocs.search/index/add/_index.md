---
title: add method
second_title: GroupDocs.Search for Python via .NET API References
description: "Performs indexing operation by adding a file or folder specified by an absolute or relative path; documents in all subfolders are indexed."
type: docs
url: /python-net/groupdocs.search/index/add/
is_root: false
weight: 1010
---


## add {#path}

Performs indexing operation by adding a file or folder specified by an absolute or relative path; documents in all subfolders are indexed.

```python
def add(self, path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| path | `str` | The path to a file or folder to be indexed. |

### Example

```python
from groupdocs.search import Index

def on_file_indexing(sender, args):
    print("Indexing:", args.document_full_path)

with Index("./index") as index:
    index.events.file_indexing += on_file_indexing
    index.add("./documents")
```

## add {#path-options}

Adds a file or folder by an absolute or relative path, indexing documents from all subfolders.

```python
def add(self, path, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| path | `str` | The path to a file or folder to be indexed. |
| options | `IndexingOptions` | The indexing options. |

## add {#paths}

Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

```python
def add(self, paths):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| paths | `list[str]` | The paths to files or folders to be indexed. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")
```

## add {#paths-options}

Adds files or folders by an absolute or relative path, indexing documents from all subfolders.

```python
def add(self, paths, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| paths | `list[str]` | The paths to files or folders to be indexed. |
| options | `IndexingOptions` | The indexing options. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import IndexingOptions


def on_file_indexing(sender, args):
    print("Indexing:", args.document_full_path)


with Index("./index") as index:
    index.events.file_indexing += on_file_indexing
    index.add(["./documents"], IndexingOptions())
```

## add {#documents-options}

Indexes documents from the file system, a stream, or a structured source.

```python
def add(self, documents, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| documents | `list[Document]` | The documents from the file system, a stream, or a structured source. |
| options | `IndexingOptions` | The indexing options. |

## add {#data-options}

Performs an indexing operation and adds the extracted data to the index.

```python
def add(self, data, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| data | `list[ExtractedData]` | The extracted data. |
| options | `IndexingOptions` | The indexing options. |

### Aliases

These names call `add` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_file` | `add_file(path, options)`<br>`add_file(path)` |
| `add_string` | `add_string(path, options)`<br>`add_string(path)` |
| `add_files` | `add_files(paths, options)`<br>`add_files(paths)` |
| `add_strings` | `add_strings(paths, options)`<br>`add_strings(paths)` |
| `add_document` | `add_document(documents, options)` |
| `add_extracted_data` | `add_extracted_data(data, options)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
