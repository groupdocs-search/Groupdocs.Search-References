---
title: password_required event
second_title: GroupDocs.Search for Python via .NET API References
description: "Occurs when a document requires password for opening."
type: docs
url: /python-net/groupdocs.search/extractor/password_required/
is_root: false
weight: 4030
---


## password_required event

Occurs when a document requires password for opening.

### Definition:
```python
extractor.password_required += handler    # subscribe handler(sender, args)
extractor.password_required -= handler    # remove the last subscription of handler
extractor.password_required.clear()       # remove every handler added from Python
```

### Handler arguments
| Argument | Description |
| :- | :- |
| `sender` | The object that raised the event. |
| `args` | [`PasswordRequiredEventArgs`](/search/python-net/groupdocs.search.events/passwordrequiredeventargs/) |

The handler runs on the thread that raises the event, which can be an engine worker thread. An exception it raises there is printed to stderr and ignored; on the calling thread it reaches the engine, as in .NET.

### See Also
* class [`Extractor`](/search/python-net/groupdocs.search/extractor/)
