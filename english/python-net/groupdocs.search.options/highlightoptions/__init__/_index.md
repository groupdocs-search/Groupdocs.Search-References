---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new instance of the HighlightOptions class."
type: docs
url: /python-net/groupdocs.search.options/highlightoptions/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the [`HighlightOptions`](/search/python-net/groupdocs.search.options/highlightoptions/) class.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.search.options import HighlightOptions
from groupdocs.search.options import Color

options = HighlightOptions()
options.terms_before = 5
options.terms_after = 5
options.terms_total = 15
options.highlight_color = Color(0, 0, 127)
options.use_inline_styles = True
```

### See Also
* class [`HighlightOptions`](/search/python-net/groupdocs.search.options/highlightoptions/)
