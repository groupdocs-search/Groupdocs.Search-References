---
title: create_file_path_regular_expression method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that skips documents whose full path does not match a regular expression."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_file_path_regular_expression/
is_root: false
weight: 1090
---


## create_file_path_regular_expression {#pattern}

Creates a filter that skips documents whose full path does not match a regular expression.

```python
def create_file_path_regular_expression(cls, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern. |

**Returns:** DocumentFilter: A document filter based on file path.

### Example

```python
from groupdocs.search.options import DocumentFilter

document_filter = DocumentFilter.create_file_path_regular_expression("Einstein")
print(document_filter)
```

## create_file_path_regular_expression {#pattern-options}

Creates a filter for skipping documents that do not match a regular expression. The regular expression is applied to the full path of a document.

```python
def create_file_path_regular_expression(cls, pattern, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern. |
| options | `System.Text.RegularExpressions.RegexOptions` | The regular expression options. |

**Returns:** DocumentFilter: A document filter by file name.

### Example

```python
from groupdocs.search.options import DocumentFilter
from groupdocs.search import RegexOptions

document_filter = DocumentFilter.create_file_path_regular_expression(
    "Einstein", RegexOptions.IGNORE_CASE
)
print(document_filter)
```

### Aliases

These names call `create_file_path_regular_expression` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_file_path_regular_expression_file` | `create_file_path_regular_expression_file(pattern, options)`<br>`create_file_path_regular_expression_file(pattern)` |
| `create_file_path_regular_expression_string` | `create_file_path_regular_expression_string(pattern, options)`<br>`create_file_path_regular_expression_string(pattern)` |

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
