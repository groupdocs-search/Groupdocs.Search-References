---
title: WordsFieldNames class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a list of field names for the faceted search."
type: docs
url: /python-net/groupdocs.search.options/wordsfieldnames/
is_root: false
weight: 460
---


## WordsFieldNames class

Represents a list of field names for the faceted search.

Learn more
- https://docs.groupdocs.com/search/python-net/faceted-search/

The WordsFieldNames type exposes the following members:

### Fields
| Field | Description |
| :- | :- |
| [APPLICATION](/search/python-net/groupdocs.search.options/wordsfieldnames/application/) | The application field name. |
| [APPLICATION_VERSION](/search/python-net/groupdocs.search.options/wordsfieldnames/application_version/) | The application version field name. |
| [TEMPLATE](/search/python-net/groupdocs.search.options/wordsfieldnames/template/) | The template field name. |
| [TITLE](/search/python-net/groupdocs.search.options/wordsfieldnames/title/) | The title field name. |
| [SUBJECT](/search/python-net/groupdocs.search.options/wordsfieldnames/subject/) | The subject field name. |
| [COMMENTS](/search/python-net/groupdocs.search.options/wordsfieldnames/comments/) | The comments field name. |
| [KEYWORDS](/search/python-net/groupdocs.search.options/wordsfieldnames/keywords/) | The keywords field name. |
| [CONTENT_STATUS](/search/python-net/groupdocs.search.options/wordsfieldnames/content_status/) | The content status field name. |
| [CATEGORY](/search/python-net/groupdocs.search.options/wordsfieldnames/category/) | The category field name. |
| [MANAGER](/search/python-net/groupdocs.search.options/wordsfieldnames/manager/) | The manager field name. |
| [AUTHOR](/search/python-net/groupdocs.search.options/wordsfieldnames/author/) | The author field name. |
| [LAST_AUTHOR](/search/python-net/groupdocs.search.options/wordsfieldnames/last_author/) | The last author field name. |
| [COMPANY](/search/python-net/groupdocs.search.options/wordsfieldnames/company/) | The company field name. |
| [HYPERLINK_BASE](/search/python-net/groupdocs.search.options/wordsfieldnames/hyperlink_base/) | The hyperlink base field name. |
| [CREATED_TIME](/search/python-net/groupdocs.search.options/wordsfieldnames/created_time/) | The created time field name. |
| [LAST_SAVED_TIME](/search/python-net/groupdocs.search.options/wordsfieldnames/last_saved_time/) | The last saved time field name. |
| [LAST_PRINTED_TIME](/search/python-net/groupdocs.search.options/wordsfieldnames/last_printed_time/) | The last printed time field name. |
| [REVISION_NUMBER](/search/python-net/groupdocs.search.options/wordsfieldnames/revision_number/) | The revision number field name. |
| [TOTAL_EDITING_TIME](/search/python-net/groupdocs.search.options/wordsfieldnames/total_editing_time/) | The total editing time field name. |

### Example

```python
from groupdocs.search import Index, SearchQuery
from groupdocs.search.options import WordsFieldNames

# Search using a text query on the COMPANY field
query = f"{WordsFieldNames.COMPANY}: Dycum"
result = index.search(query)

# Search using an object query on the COMPANY field
word_query = SearchQuery.create_word_query("Dycum")
field_query = SearchQuery.create_field_query(WordsFieldNames.COMPANY, word_query)
result2 = index.search(field_query)
```

### Guides
Task guides that use `WordsFieldNames`:

* [Faceted search](/search/python-net/guides/faceted-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
