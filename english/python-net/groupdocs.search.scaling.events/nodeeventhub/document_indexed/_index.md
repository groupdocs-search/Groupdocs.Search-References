---
title: document_indexed event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when a document has been indexed."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/document_indexed/
is_root: false
weight: 4060
---


## document_indexed event

Occurs when a document has been indexed.

### Definition:
```python
node_event_hub.document_indexed += handler    # subscribe handler(sender, args)
node_event_hub.document_indexed -= handler    # remove the last subscription of handler
node_event_hub.document_indexed.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`DocumentIndexedEventArgs`](/search/python-net/groupdocs.search.scaling.events/documentindexedeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
