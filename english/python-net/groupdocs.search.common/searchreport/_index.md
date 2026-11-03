---
title: SearchReport class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents detailed information on a search operation."
type: docs
url: /python-net/groupdocs.search.common/searchreport/
is_root: false
weight: 300
---


## SearchReport class

Represents detailed information on a search operation.

Learn more:
- Search reports: https://docs.groupdocs.com/search/python-net/search-reports/

The SearchReport type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [to_string](/search/python-net/groupdocs.search.common/searchreport/to_string/) | Returns a string that represents the current SearchReport. |

### Properties
| Property | Description |
| :- | :- |
| [document_count](/search/python-net/groupdocs.search.common/searchreport/document_count/) | The number of documents found. |
| [end_time](/search/python-net/groupdocs.search.common/searchreport/end_time/) | The end time of the search. |
| [object_query](/search/python-net/groupdocs.search.common/searchreport/object_query/) | The search query in object form. |
| [occurrence_count](/search/python-net/groupdocs.search.common/searchreport/occurrence_count/) | The total number of occurrences found. |
| [search_duration](/search/python-net/groupdocs.search.common/searchreport/search_duration/) | The search duration. |
| [search_options](/search/python-net/groupdocs.search.common/searchreport/search_options/) | The search options. |
| [start_time](/search/python-net/groupdocs.search.common/searchreport/start_time/) | The start time of the search. |
| [text_query](/search/python-net/groupdocs.search.common/searchreport/text_query/) | The search query in text form. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")
index.search("contract")
for report in index.get_search_reports():
    print(report.text_query, report.document_count)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
