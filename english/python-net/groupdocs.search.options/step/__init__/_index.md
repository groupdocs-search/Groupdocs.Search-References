---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new Step instance."
type: docs
url: /python-net/groupdocs.search.options/step/__init__/
is_root: false
weight: 10
---


## __init__ {#lower_limit-level}

Initializes a new [`Step`](/search/python-net/groupdocs.search.options/step/) instance.

```python
def __init__(self, lower_limit, level):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_limit | `int` | The lower limit. |
| level | `int` | The level. |

### Example

```python
from groupdocs.search.options import Step, TableDiscreteFunction

# Define steps for the fuzzy search algorithm
step1 = Step(5, 2)
step2 = Step(8, 3)

# Create the table discrete function using the steps
fuzzy_algo = TableDiscreteFunction(1, [step1, step2])
```

### See Also
* class [`Step`](/search/python-net/groupdocs.search.options/step/)
