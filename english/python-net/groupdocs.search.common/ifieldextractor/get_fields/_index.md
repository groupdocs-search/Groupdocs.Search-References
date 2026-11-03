---
title: get_fields method
second_title: GroupDocs.Search for Python via .NET API References
description: "Extracts all fields from the specified document."
type: docs
url: /python-net/groupdocs.search.common/ifieldextractor/get_fields/
is_root: false
weight: 1010
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

**Returns:** list[DocumentField]: The extracted fields.

### Example

```python
from groupdocs.search.common import DocumentField

class LogExtractor:
    extensions = [".log"]

    def get_fields(self, source):
        if isinstance(source, str):
            # source is a file path
            return [
                DocumentField("FileName", source),
                DocumentField("Content", open(source, encoding="utf-8-sig").read()),
            ]
        # source is a stream
        return [DocumentField("Content", source.read().decode("utf-8-sig"))]

extractor = LogExtractor()
fields = extractor.get_fields("example.log")
for field in fields:
    print(f"{field.name}: {field.value}")
```

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
* class [`IFieldExtractor`](/search/python-net/groupdocs.search.common/ifieldextractor/)
