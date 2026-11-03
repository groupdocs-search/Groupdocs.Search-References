---
title: optimization_completed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when optimization of all nodes is finished."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/optimization_completed/
is_root: false
weight: 4110
---


## optimization_completed event

Occurs when optimization of all nodes is finished.

### Definition:
```python
node_event_hub.optimization_completed += handler    # subscribe handler(sender, args)
node_event_hub.optimization_completed -= handler    # remove the last subscription of handler
node_event_hub.optimization_completed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | the event's data, if any |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
