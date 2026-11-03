---
title: data_extracted event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when the data has been extracted from a document."
type: docs
url: /python-net/groupdocs.search.scaling.events/nodeeventhub/data_extracted/
is_root: false
weight: 4030
---


## data_extracted event

Occurs when the data has been extracted from a document.

### Definition:
```python
node_event_hub.data_extracted += handler    # subscribe handler(sender, args)
node_event_hub.data_extracted -= handler    # remove the last subscription of handler
node_event_hub.data_extracted.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`DataExtractedEventArgs`](/search/python-net/groupdocs.search.scaling.events/dataextractedeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`NodeEventHub`](/search/python-net/groupdocs.search.scaling.events/nodeeventhub/)
