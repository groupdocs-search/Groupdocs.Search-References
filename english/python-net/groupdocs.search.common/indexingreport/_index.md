---
title: IndexingReport class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents detailed information on an indexing operation."
type: docs
url: /python-net/groupdocs.search.common/indexingreport/
is_root: false
weight: 250
---


## IndexingReport class

Represents detailed information on an indexing operation.

Learn more:
- Indexing reports: https://docs.groupdocs.com/search/python-net/indexing-reports/

The IndexingReport type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [end_time](/search/python-net/groupdocs.search.common/indexingreport/end_time/) | The indexing end time. |
| [errors](/search/python-net/groupdocs.search.common/indexingreport/errors/) | The list of errors. |
| [indexed_documents](/search/python-net/groupdocs.search.common/indexingreport/indexed_documents/) | The list of indexed documents. |
| [indexed_documents_size](/search/python-net/groupdocs.search.common/indexingreport/indexed_documents_size/) | The total length of indexed documents in MB. |
| [indexing_time](/search/python-net/groupdocs.search.common/indexingreport/indexing_time/) | The indexing duration. |
| [removed_documents](/search/python-net/groupdocs.search.common/indexingreport/removed_documents/) | The list of documents removed from the index. |
| [segment_count](/search/python-net/groupdocs.search.common/indexingreport/segment_count/) | The number of index segments. |
| [start_time](/search/python-net/groupdocs.search.common/indexingreport/start_time/) | The indexing start time. |
| [total_documents_in_index](/search/python-net/groupdocs.search.common/indexingreport/total_documents_in_index/) | The total number of documents in the index. |
| [total_index_size](/search/python-net/groupdocs.search.common/indexingreport/total_index_size/) | The total index size in bytes. |
| [total_term_count](/search/python-net/groupdocs.search.common/indexingreport/total_term_count/) | The total number of terms in index. |
| [updated_documents](/search/python-net/groupdocs.search.common/indexingreport/updated_documents/) | The list of updated documents. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")
# Perform indexing; reports are generated per batch
for report in index.get_indexing_reports():
    print(report.start_time)          # report.StartTime
    print(report.indexing_time)       # report.IndexingTime
    print(report.total_documents_in_index)  # report.TotalDocumentsInIndex
    print(report.total_term_count)    # report.TotalTermCount
    print(report.indexed_documents_size)    # report.IndexedDocumentsSize
    print(report.total_index_size / 1024.0 / 1024.0)  # size in MB
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
