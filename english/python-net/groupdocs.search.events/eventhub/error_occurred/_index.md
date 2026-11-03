---
title: error_occurred event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when an error occurs during an index operation."
type: docs
url: /python-net/groupdocs.search.events/eventhub/error_occurred/
is_root: false
weight: 4010
---


## error_occurred event

Occurs when an error occurs during an index operation.

### Definition:
```python
event_hub.error_occurred += handler    # subscribe handler(sender, args)
event_hub.error_occurred -= handler    # remove the last subscription of handler
event_hub.error_occurred.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`IndexErrorEventArgs`](/search/python-net/groupdocs.search.events/indexerroreventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
