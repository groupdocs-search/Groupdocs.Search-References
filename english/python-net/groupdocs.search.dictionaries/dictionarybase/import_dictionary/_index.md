---
title: import_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Imports a dictionary from the specified file."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionarybase/import_dictionary/
is_root: false
weight: 1030
---


## import_dictionary {#file_path}

Imports a dictionary from the specified file.

Each dictionary class derives from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/), which provides `export_dictionary` and `import_dictionary` for saving to and loading from a file. These methods do not raise an exception if the file cannot be written or read, or if it has an invalid format.

```python
def import_dictionary(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The file to import from. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes a dictionary that defines how the text of documents is divided into terms (see `DictionaryRepository`), and the index of the dictionary contains documents, is not in the `IndexStatus.ready` status or is disposed. |

### Example

```python
# Import aliases from a file
aliases.import_dictionary("./Aliases.dat")

# Import homophones from a file
homophones.import_dictionary("./Homophones.dat")
```

### Aliases

These names call `import_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `import_dictionary_file` | `import_dictionary_file(file_path)` |
| `import_dictionary_string` | `import_dictionary_string(file_path)` |

### See Also
* class [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)
