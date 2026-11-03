---
title: operation_finished event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when an index operation is finished."
type: docs
url: /python-net/groupdocs.search.events/eventhub/operation_finished/
is_root: false
weight: 4040
---


## operation_finished event

Occurs when an index operation is finished.

### Definition:
```python
event_hub.operation_finished += handler    # subscribe handler(sender, args)
event_hub.operation_finished -= handler    # remove the last subscription of handler
event_hub.operation_finished.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`OperationFinishedEventArgs`](/search/python-net/groupdocs.search.events/operationfinishedeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
