---
title: CommonFieldNames class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a list of field names for the faceted search."
type: docs
url: /python-net/groupdocs.search.options/commonfieldnames/
is_root: false
weight: 40
---


## CommonFieldNames class

Represents a list of field names for the faceted search.

Learn more: https://docs.groupdocs.com/search/python-net/faceted-search/

The CommonFieldNames type exposes the following members:

### Fields
| Field | Description |
| :- | :- |
| [CONTENT](/search/python-net/groupdocs.search.options/commonfieldnames/content/) | The content field name. |
| [FILE_NAME](/search/python-net/groupdocs.search.options/commonfieldnames/file_name/) | The file name field name. |
| [FORMAT_FAMILY](/search/python-net/groupdocs.search.options/commonfieldnames/format_family/) | The format family field name. |
| [CREATION_DATE](/search/python-net/groupdocs.search.options/commonfieldnames/creation_date/) | The creation date field name. |
| [MODIFICATION_DATE](/search/python-net/groupdocs.search.options/commonfieldnames/modification_date/) | The modification date field name. |
| [EMBEDDED_IMAGE_OCR](/search/python-net/groupdocs.search.options/commonfieldnames/embedded_image_ocr/) | The embedded image OCR field name. |

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.options import CommonFieldNames

word_query = SearchQuery.create_word_query("Einstein")
field_query = SearchQuery.create_field_query(CommonFieldNames.CONTENT, word_query)
result = index.search(field_query)
```

### Guides
Task guides that use `CommonFieldNames`:

* [Faceted search](/search/python-net/guides/faceted-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
