---
title: operation_progress_changed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when the progress of the indexing or update operation changes."
type: docs
url: /python-net/groupdocs.search.events/eventhub/operation_progress_changed/
is_root: false
weight: 4050
---


## operation_progress_changed event

Occurs when the progress of the indexing or update operation changes.

### Definition:
```python
event_hub.operation_progress_changed += handler    # subscribe handler(sender, args)
event_hub.operation_progress_changed -= handler    # remove the last subscription of handler
event_hub.operation_progress_changed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`OperationProgressEventArgs`](/search/python-net/groupdocs.search.events/operationprogresseventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
