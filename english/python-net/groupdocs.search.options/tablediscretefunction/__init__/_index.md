---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new TableDiscreteFunction instance."
type: docs
url: /python-net/groupdocs.search.options/tablediscretefunction/__init__/
is_root: false
weight: 10
---


## __init__ {#offset_of_inputs-table_of_outputs}

Initializes a new TableDiscreteFunction instance.

```python
def __init__(self, offset_of_inputs, table_of_outputs):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| offset_of_inputs | `int` | The offset of the table indices relative to the input values. |
| table_of_outputs | `list[int]` | The table of output values. |

| Raises | Description |
| :- | :- |
| `ValueError` | When the number of table elements is 0. |

### Example

```python
from groupdocs.search.options import TableDiscreteFunction

# Create a function with an offset of 0 and a table defining the maximum
# number of differences for word lengths.
fuzzy_algo = TableDiscreteFunction(0, [0, 1, 1, 2, 2])
```

## __init__ {#first_step_level-steps}

Initializes a new TableDiscreteFunction.

```python
def __init__(self, first_step_level, steps):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| first_step_level | `int` | The level of the first step of the step function. |
| steps | `list[Step]` | The next steps of the step function. |

| Raises | Description |
| :- | :- |
| `ValueError` | If limits of steps are not strictly increasing. |

### Example

```python
from groupdocs.search.options import Step, TableDiscreteFunction

# 1 mistake for words of 1-4 characters, 2 for 5-7 characters, and 3 from 8 characters on
fuzzy_algorithm = TableDiscreteFunction(1, [Step(5, 2), Step(8, 3)])
```

### See Also
* class [`TableDiscreteFunction`](/search/python-net/groupdocs.search.options/tablediscretefunction/)
