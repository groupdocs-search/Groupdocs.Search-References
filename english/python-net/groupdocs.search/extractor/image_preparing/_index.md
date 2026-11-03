---
title: image_preparing event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when an image is going to be prepared for indexing."
type: docs
url: /python-net/groupdocs.search/extractor/image_preparing/
is_root: false
weight: 4020
---


## image_preparing event

Occurs when an image is going to be prepared for indexing.

### Definition:
```python
extractor.image_preparing += handler    # subscribe handler(sender, args)
extractor.image_preparing -= handler    # remove the last subscription of handler
extractor.image_preparing.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`ImagePreparingEventArgs`](/search/python-net/groupdocs.search.events/imagepreparingeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`Extractor`](/search/python-net/groupdocs.search/extractor/)
