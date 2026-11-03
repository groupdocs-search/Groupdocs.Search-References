---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new DateFormat instance."
type: docs
url: /python-net/groupdocs.search.options/dateformat/__init__/
is_root: false
weight: 10
---


## __init__ {#culture_name-format_elements}

Initializes a new DateFormat instance.

```python
def __init__(self, culture_name, format_elements):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| culture_name | `str` | The culture name. |
| format_elements | `list[DateFormatElement]` | The format elements. |

### Example

```python
from groupdocs.search.options import DateFormat, DateFormatElement

elements = [
    DateFormatElement.DAY_OF_MONTH_TWO_DIGITS,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.MONTH_FULL_NAME,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.YEAR_FOUR_DIGITS,
]

date_format = DateFormat("de-DE", elements)
```

## __init__ {#format_elements-date_separator}

Initializes a new DateFormat instance.

```python
def __init__(self, format_elements, date_separator):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| format_elements | `list[DateFormatElement]` | The format elements. |
| date_separator | `str` | The date separator. |

### Example

```python
from groupdocs.search.options import DateFormat, DateFormatElement

elements = [
    DateFormatElement.DAY_OF_MONTH_TWO_DIGITS,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.MONTH_FULL_NAME,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.YEAR_FOUR_DIGITS,
]

date_format = DateFormat(elements, "/")
```

### See Also
* class [`DateFormat`](/search/python-net/groupdocs.search.options/dateformat/)
