---
title: use_case_sensitive_search property
second_title: GroupDocs.Search for Python via .NET API References
description: "The flag indicating whether the search is case‑sensitive."
type: docs
url: /python-net/groupdocs.search.options/searchoptions/use_case_sensitive_search/
is_root: false
weight: 2110
---


## use_case_sensitive_search property

The flag indicating whether the search is case‑sensitive. The default value is False.

Case‑sensitive search cannot be combined with fuzzy search, synonym search, homophone search, word‑forms search, spelling correction, or keyboard‑layout correction; attempting to do so results in an empty result set and an error indicating the conflict.

### Definition:
```python
@property
def use_case_sensitive_search(self):
    ...
@use_case_sensitive_search.setter
def use_case_sensitive_search(self, value):
    ...
```

### See Also
* class [`SearchOptions`](/search/python-net/groupdocs.search.options/searchoptions/)
