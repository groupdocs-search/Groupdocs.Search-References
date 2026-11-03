---
title: export_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Exports the dictionary to a file with the specified name."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionarybase/export_dictionary/
is_root: false
weight: 1020
---


## export_dictionary {#file_path}

Exports the dictionary to a file with the specified name.

The method does not raise an exception if the file cannot be written, read, or has an invalid format.

```python
def export_dictionary(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The file to export to. |

### Example

```python
# Export an alias dictionary to a file
aliases.export_dictionary("./Aliases.dat")

# Export a homophone dictionary to a file
homophones.export_dictionary("./Homophones.dat")
```

### Aliases

These names call `export_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `export_dictionary_file` | `export_dictionary_file(file_path)` |
| `export_dictionary_string` | `export_dictionary_string(file_path)` |

### See Also
* class [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)
