---
title: get_fields method
second_title: GroupDocs.Search for Python via .NET API References
description: "Extracts all fields from the specified document."
type: docs
url: /python-net/groupdocs.search.common/icontaineritemextractor/get_fields/
is_root: false
weight: 1020
---


## get_fields {#file_path}

Extracts all fields from the specified document.

```python
def get_fields(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The document file path. |

**Returns:** The extracted fields.

## get_fields {#stream}

Extracts all fields from the specified document.

```python
def get_fields(self, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The document stream. |

**Returns:** The extracted fields.

### Aliases

These names call `get_fields` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_fields_file` | `get_fields_file(file_path)` |
| `get_fields_string` | `get_fields_string(file_path)` |
| `get_fields_stream` | `get_fields_stream(stream)` |
| `get_fields_streams` | `get_fields_streams(stream)` |

### See Also
* class [`IContainerItemExtractor`](/search/python-net/groupdocs.search.common/icontaineritemextractor/)
