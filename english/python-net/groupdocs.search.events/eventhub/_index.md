---
title: EventHub class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides index events for subscribing."
type: docs
url: /python-net/groupdocs.search.events/eventhub/
is_root: false
weight: 20
---


## EventHub class

Provides index events for subscribing.

Learn more:
- Search index events: https://docs.groupdocs.com/search/python-net/search-index-events/

The EventHub type exposes the following members:

### Events
| Event | Description |
| :- | :- |
| [error_occurred](/search/python-net/groupdocs.search.events/eventhub/error_occurred/) | Occurs when an error occurs during an index operation. |
| [file_indexing](/search/python-net/groupdocs.search.events/eventhub/file_indexing/) | Occurs when a document is going to be indexed. |
| [image_preparing](/search/python-net/groupdocs.search.events/eventhub/image_preparing/) | Occurs when an image is going to be prepared for indexing. |
| [operation_finished](/search/python-net/groupdocs.search.events/eventhub/operation_finished/) | Occurs when an index operation is finished. |
| [operation_progress_changed](/search/python-net/groupdocs.search.events/eventhub/operation_progress_changed/) | Occurs when the progress of the indexing or update operation changes. |
| [optimization_progress_changed](/search/python-net/groupdocs.search.events/eventhub/optimization_progress_changed/) | Occurs when the progress of the optimization operation changes. |
| [password_required](/search/python-net/groupdocs.search.events/eventhub/password_required/) | Occurs when a document requires password for opening. |
| [search_phase_completed](/search/python-net/groupdocs.search.events/eventhub/search_phase_completed/) | Occurs when the search phase is completed. |
| [status_changed](/search/python-net/groupdocs.search.events/eventhub/status_changed/) | Occurs when the index status changes. |

### Example

```python
from groupdocs.search import Index

index_folder = "./MyIndex"
documents_folder = "./documents"
query = "Einstein"

index = Index(index_folder)

def on_error(sender, args):
    print(args.message)

index.events.error_occurred += on_error

index.add(documents_folder)

result = index.search(query)
```

### See Also
* module [`groupdocs.search.events`](/search/python-net/groupdocs.search.events/)
