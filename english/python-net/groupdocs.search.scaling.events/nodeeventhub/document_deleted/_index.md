---
title: document_deleted event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when a document has been deleted."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/document_deleted/
is_root: false
weight: 4050
---


## document_deleted event

Occurs when a document has been deleted.

### Definition:
```python
node_event_hub.document_deleted += handler    # subscribe handler(sender, args)
node_event_hub.document_deleted -= handler    # remove the last subscription of handler
node_event_hub.document_deleted.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`DocumentDeletedEventArgs`](/search/python-net/groupdocs.search.scaling.events/documentdeletedeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
