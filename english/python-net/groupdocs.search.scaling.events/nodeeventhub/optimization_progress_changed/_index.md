---
title: optimization_progress_changed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when the progress of the optimization operation has changed."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/optimization_progress_changed/
is_root: false
weight: 4120
---


## optimization_progress_changed event

Occurs when the progress of the optimization operation has changed.

### Definition:
```python
node_event_hub.optimization_progress_changed += handler    # subscribe handler(sender, args)
node_event_hub.optimization_progress_changed -= handler    # remove the last subscription of handler
node_event_hub.optimization_progress_changed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`NetworkOptimizationProgressEventArgs`](/search/python-net/groupdocs.search.scaling.events/networkoptimizationprogresseventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
