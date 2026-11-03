---
title: error_occurred event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when an error occurs in one of the nodes of the search network."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/error_occurred/
is_root: false
weight: 4070
---


## error_occurred event

Occurs when an error occurs in one of the nodes of the search network.

### Definition:
```python
node_event_hub.error_occurred += handler    # subscribe handler(sender, args)
node_event_hub.error_occurred -= handler    # remove the last subscription of handler
node_event_hub.error_occurred.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`ErrorOccurredEventArgs`](/search/python-net/groupdocs.search.scaling.events/erroroccurredeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
