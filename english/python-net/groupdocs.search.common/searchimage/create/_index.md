---
title: create method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates an image from a file for searching."
type: docs
url: /python-net/groupdocs.search.common/searchimage/create/
is_root: false
weight: 1010
---


## create {#file_path}

Creates an image from a file for searching.

```python
def create(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The image file path. |

**Returns:** SearchImage: An image to search.

### Example

```python
from groupdocs.search.common import SearchImage

search_image = SearchImage.create("./image.png")
```

## create {#file_path-image_index}

Creates an image from a file for searching.

```python
def create(cls, file_path, image_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The image file path. |
| image_index | `int` | The image index in multipage images. |

**Returns:** SearchImage: An image to search.

## create {#stream}

Creates an image from a stream for searching.

```python
def create(cls, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The image stream. |

**Returns:** SearchImage: An image to search.

### Example

```python
from groupdocs.search.common import SearchImage

with open("image.png", "rb") as f:
    search_image = SearchImage.create(f)
```

## create {#stream-image_index}

Creates an image from a stream to search.

```python
def create(cls, stream, image_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The image stream. |
| image_index | `int` | The image index in multipage images. |

**Returns:** SearchImage: An image to search.

### Example

```python
from groupdocs.search.common import SearchImage

# Open an image file as a binary stream
with open("./image.png", "rb") as stream:
    # Create a SearchImage from the stream (first page = 0)
    search_image = SearchImage.create(stream, image_index=0)

# Use `search_image` with a Searcher instance
# searcher.search_first(search_image, ...)
```

### Aliases

These names call `create` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_file` | `create_file(file_path, image_index)`<br>`create_file(file_path)` |
| `create_string` | `create_string(file_path, image_index)`<br>`create_string(file_path)` |
| `create_stream` | `create_stream(stream, image_index)`<br>`create_stream(stream)` |
| `create_streams` | `create_streams(stream, image_index)`<br>`create_streams(stream)` |

### See Also
* class [`SearchImage`](/search/python-net/groupdocs.search.common/searchimage/)
