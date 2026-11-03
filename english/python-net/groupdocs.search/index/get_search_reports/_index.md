---
title: get_search_reports method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves the reports on search operations."
type: docs
url: /python-net/groupdocs.search/index/get_search_reports/
is_root: false
weight: 1130
---


## get_search_reports

Retrieves the reports on search operations.

```python
def get_search_reports(self):
    ...
```

**Returns:** list[SearchReport]: The search reports.

### Example

```python
    from groupdocs.search import Index

    index = Index("./index")
    index.add("./documents")
    index.search("contract")
    for r in index.get_search_reports():
        print(r.text_query, r.document_count)  # SearchReport, one per query
    ```

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
