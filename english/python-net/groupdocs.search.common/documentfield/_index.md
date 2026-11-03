---
title: DocumentField class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a document field data."
type: docs
url: /python-net/groupdocs.search.common/documentfield/
is_root: false
weight: 60
---


## DocumentField class

Represents a document field data.

- Custom text extractors: https://docs.groupdocs.com/search/python-net/custom-text-extractors/
- Indexing additional fields: https://docs.groupdocs.com/search/python-net/indexing-additional-fields/

The DocumentField type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/documentfield/__init__/#name-value) | Initializes a new DocumentField. |

### Properties
| Property | Description |
| :- | :- |
| [name](/search/python-net/groupdocs.search.common/documentfield/name/) | The field name. |
| [value](/search/python-net/groupdocs.search.common/documentfield/value/) | The field value. |

### Example

```python
from groupdocs.search.common import DocumentField

# Create a field with a name and a value
field = DocumentField("FileName", "/path/to/file.txt")
```

### Guides
Task guides that use `DocumentField`:

* [Search index events](/search/python-net/guides/search-index-events/)
* [Custom text extractors](/search/python-net/guides/custom-text-extractors/)

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
