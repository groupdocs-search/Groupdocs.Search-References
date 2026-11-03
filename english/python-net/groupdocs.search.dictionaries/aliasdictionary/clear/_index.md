---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes all aliases from a AliasDictionary object."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/clear/
is_root: false
weight: 1040
---


## clear

Removes all aliases from a [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/) object.

```python
def clear(self):
    ...
```

### Example

```python
index.add("./documents")
aliases = index.dictionaries.alias_dictionary
if aliases.count > 0:
    # Delete all existing aliases
    aliases.clear()
```

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
