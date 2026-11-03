---
title: status_changed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when the index status changes."
type: docs
url: /python-net/groupdocs.search.events/eventhub/status_changed/
is_root: false
weight: 4090
---


## status_changed event

Occurs when the index status changes.

### Definition:
```python
event_hub.status_changed += handler    # subscribe handler(sender, args)
event_hub.status_changed -= handler    # remove the last subscription of handler
event_hub.status_changed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`BaseIndexEventArgs`](/search/python-net/groupdocs.search.events/baseindexeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
