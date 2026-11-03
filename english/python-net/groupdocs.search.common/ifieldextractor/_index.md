---
title: IFieldExtractor class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides methods for extracting fields from a document."
type: docs
url: /python-net/groupdocs.search.common/ifieldextractor/
is_root: false
weight: 190
---


## IFieldExtractor class

Provides methods for extracting fields from a document.

Learn more:
- https://docs.groupdocs.com/search/python-net/custom-text-extractors/

The IFieldExtractor type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [get_fields](/search/python-net/groupdocs.search.common/ifieldextractor/get_fields/#file_path) | Extracts all fields from the specified document. |
| [get_fields](/search/python-net/groupdocs.search.common/ifieldextractor/get_fields/#stream) | Extracts all fields from the specified document. |

### Properties
| Property | Description |
| :- | :- |
| [extensions](/search/python-net/groupdocs.search.common/ifieldextractor/extensions/) | The supported extensions. |

### Example

```python
from groupdocs.search import Index, IndexSettings
from groupdocs.search.common import DocumentField


# A custom extractor: the extensions it handles, and the fields it extracts
class LogExtractor(object):
    extensions = [".log"]

    def get_fields(self, source):
        # source is a file path, or a binary stream for a document added from a stream
        if isinstance(source, str):
            with open(source, encoding="utf-8-sig") as f:
                text = f.read()
        else:
            text = source.read().decode("utf-8-sig")
        return [DocumentField("Content", text)]


# Using the custom extractor for indexing
settings = IndexSettings()
settings.custom_extractors.add(LogExtractor())
index = Index("./MyIndex", settings)  # Create or load an index
index.add("./documents")  # Index documents
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
