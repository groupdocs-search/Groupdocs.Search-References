---
title: get_indexing_reports method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the reports on indexing operations."
type: docs
url: /python-net/groupdocs.search/index/get_indexing_reports/
is_root: false
weight: 1120
---


## get_indexing_reports

Gets the reports on indexing operations.

```python
def get_indexing_reports(self):
    ...
```

**Returns:** list[IndexingReport]: The indexing reports.

### Example

```python
    from groupdocs.search import Index

    index = Index("./index")
    index.add("./documents")
    for report in index.get_indexing_reports():
        print(len(report.indexed_documents), report.indexing_time)
    ```

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
