---
title: file_indexing event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when a document is going to be indexed."
type: docs
url: /python-net/groupdocs.search.events/eventhub/file_indexing/
is_root: false
weight: 4020
---


## file_indexing event

Occurs when a document is going to be indexed.

### Definition:
```python
event_hub.file_indexing += handler    # subscribe handler(sender, args)
event_hub.file_indexing -= handler    # remove the last subscription of handler
event_hub.file_indexing.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`FileIndexingEventArgs`](/search/python-net/groupdocs.search.events/fileindexingeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`EventHub`](/search/python-net/groupdocs.search.events/eventhub/)
