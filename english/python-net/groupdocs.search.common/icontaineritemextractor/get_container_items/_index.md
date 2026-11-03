---
title: get_container_items method
second_title: GroupDocs.Search for Python via .NET API References
description: "Extracts items from a container document."
type: docs
url: /python-net/groupdocs.search.common/icontaineritemextractor/get_container_items/
is_root: false
weight: 1010
---


## get_container_items {#file_path}

Extracts items from a container document.

```python
def get_container_items(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The document file path. |

**Returns:** list: An array of extracted items.

## get_container_items {#stream}

Extracts items from container document.

```python
def get_container_items(self, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The document stream. |

**Returns:** list[GroupDocs.Search.Common.IContainerItem]: An array of extracted items.

### Aliases

These names call `get_container_items` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_container_items_file` | `get_container_items_file(file_path)` |
| `get_container_items_string` | `get_container_items_string(file_path)` |
| `get_container_items_stream` | `get_container_items_stream(stream)` |
| `get_container_items_streams` | `get_container_items_streams(stream)` |

### See Also
* class [`IContainerItemExtractor`](/search/python-net/groupdocs.search.common/icontaineritemextractor/)
