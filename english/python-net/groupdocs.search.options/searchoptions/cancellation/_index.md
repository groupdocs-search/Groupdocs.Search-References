---
title: cancellation property
second_title: GroupDocs.Search for Python via .NET API References
description: "The operation cancellation object, defaulting to None."
type: docs
url: /python-net/groupdocs.search.options/searchoptions/cancellation/
is_root: false
weight: 2010
---


## cancellation property

The operation cancellation object, defaulting to None.

Specifies a [`Cancellation`](/search/python-net/groupdocs.search.common/cancellation/) object that can be used to cancel the search operation. It applies to the first call to the search method; to cancel subsequent chunk searches, pass a [`Cancellation`](/search/python-net/groupdocs.search.common/cancellation/) as the second argument of `search_next`. The search can also be canceled immediately by calling its `cancel` method, or after a delay with `cancel_after`, in milliseconds.

### Definition:
```python
@property
def cancellation(self):
    ...
@cancellation.setter
def cancellation(self, value):
    ...
```

### See Also
* class [`SearchOptions`](/search/python-net/groupdocs.search.options/searchoptions/)
