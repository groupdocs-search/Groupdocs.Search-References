---
title: DateFormat class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a date format."
type: docs
url: /python-net/groupdocs.search.options/dateformat/
is_root: false
weight: 60
---


## DateFormat class

Represents a date format.

Learn more: Date range search (https://docs.groupdocs.com/search/python-net/date-range-search/).

The class provides two constructors:
- `DateFormat(format_elements, date_separator)` creates a format with the specified date separator; `format_elements` is a list of [`DateFormatElement`](/search/python-net/groupdocs.search.options/dateformatelement/) values. Month names, if the format contains them, are taken from the current culture.
- `DateFormat(culture_name, format_elements)` creates a format that uses the date separator and month names of the specified culture (e.g., `"en-US"` or `"de-DE"`). This constructor is useful for formats containing [`DateFormatElement.MONTH_ABBREVIATED_NAME`](/search/python-net/groupdocs.search.options/dateformatelement/month_abbreviated_name/) or [`DateFormatElement.MONTH_FULL_NAME`](/search/python-net/groupdocs.search.options/dateformatelement/month_full_name/).

The DateFormat type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/dateformat/__init__/#culture_name-format_elements) | Initializes a new DateFormat instance. |
| [__init__](/search/python-net/groupdocs.search.options/dateformat/__init__/#format_elements-date_separator) | Initializes a new DateFormat instance. |

### Methods
| Method | Description |
| :- | :- |
| [to_string](/search/python-net/groupdocs.search.options/dateformat/to_string/) | Returns a str that represents the current DateFormat. |

### Properties
| Property | Description |
| :- | :- |
| [date_separator](/search/python-net/groupdocs.search.options/dateformat/date_separator/) | The date separator. |

### Example

```python
from groupdocs.search.options import DateFormat, DateFormatElement

# German culture with month names
elements = [
    DateFormatElement.DAY_OF_MONTH_TWO_DIGITS,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.MONTH_FULL_NAME,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.YEAR_FOUR_DIGITS,
]
date_format = DateFormat("de-DE", elements)

# Custom separator
elements2 = [
    DateFormatElement.MONTH_TWO_DIGITS,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.DAY_OF_MONTH_TWO_DIGITS,
    DateFormatElement.DATE_SEPARATOR,
    DateFormatElement.YEAR_FOUR_DIGITS,
]
date_format2 = DateFormat(elements2, "/")
```

### Guides
Task guides that use `DateFormat`:

* [Build search query](/search/python-net/guides/build-search-query/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
