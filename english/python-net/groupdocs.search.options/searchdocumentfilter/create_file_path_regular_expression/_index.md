---
title: create_file_path_regular_expression method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that skips documents whose full path does not match the given regular expression."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_file_path_regular_expression/
is_root: false
weight: 1040
---


## create_file_path_regular_expression {#pattern}

Creates a filter that skips documents whose full path does not match the given regular expression.

```python
def create_file_path_regular_expression(cls, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern. |

**Returns:** SearchDocumentFilter: A search document filter by file name.

### Example

```python
    from groupdocs.search.options import SearchDocumentFilter

    # Filter documents whose full path contains "Einstein"
    document_filter = SearchDocumentFilter.create_file_path_regular_expression(
        "Einstein"
    )
    ```

## create_file_path_regular_expression {#pattern-options}

Creates a filter that skips documents not matching a regular expression.

```python
def create_file_path_regular_expression(cls, pattern, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern. |
| options | `System.Text.RegularExpressions.RegexOptions` | The regular expression options. |

**Returns:** SearchDocumentFilter: A search document filter by file name.

### Example

```python
from groupdocs.search import RegexOptions
from groupdocs.search.options import SearchDocumentFilter

# Filter documents whose full path contains "Einstein" (case‑insensitive)
filter = SearchDocumentFilter.create_file_path_regular_expression(
    "Einstein", RegexOptions.IGNORE_CASE
)
```

### Aliases

These names call `create_file_path_regular_expression` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_file_path_regular_expression_file` | `create_file_path_regular_expression_file(pattern, options)`<br>`create_file_path_regular_expression_file(pattern)` |
| `create_file_path_regular_expression_string` | `create_file_path_regular_expression_string(pattern, options)`<br>`create_file_path_regular_expression_string(pattern)` |

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
