---
title: search_phase_completed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when the search phase is completed."
type: docs
url: /python-net/groupdocs.search.events/eventhub/search_phase_completed/
is_root: false
weight: 4080
---


## search_phase_completed event

Occurs when the search phase is completed.

### Definition:
```python
event_hub.search_phase_completed += handler    # subscribe handler(sender, args)
event_hub.search_phase_completed -= handler    # remove the last subscription of handler
event_hub.search_phase_completed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`SearchPhaseEventArgs`](/search/python-net/groupdocs.search.events/searchphaseeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
