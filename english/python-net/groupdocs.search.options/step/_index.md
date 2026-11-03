---
title: Step class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a step of a step function."
type: docs
url: /python-net/groupdocs.search.options/step/
is_root: false
weight: 400
---


## Step class

Represents a step of a step function.

Learn more:
- Fuzzy search (https://docs.groupdocs.com/search/python-net/fuzzy-search/)

The Step type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/step/__init__/#lower_limit-level) | Initializes a new [`Step`](/search/python-net/groupdocs.search.options/step/) instance. |

### Properties
| Property | Description |
| :- | :- |
| [level](/search/python-net/groupdocs.search.options/step/level/) | The level. |
| [lower_limit](/search/python-net/groupdocs.search.options/step/lower_limit/) | The lower limit. |

### Example

```python
from groupdocs.search.options import Step, TableDiscreteFunction

# Define a step function for fuzzy search:
# First step applies to words of length >= 5 with level 2,
# second step applies to words of length >= 8 with level 3.
fuzzy_algo = TableDiscreteFunction(1, [Step(5, 2), Step(8, 3)])
```

### Guides
Task guides that use `Step`:

* [Fuzzy search](/search/python-net/guides/fuzzy-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
