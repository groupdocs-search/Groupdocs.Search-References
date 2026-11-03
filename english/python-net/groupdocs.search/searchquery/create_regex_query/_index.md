---
title: create_regex_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a regular expression query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_regex_query/
is_root: false
weight: 1080
---


## create_regex_query {#pattern}

Creates a regular expression query.

```python
def create_regex_query(cls, pattern):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern to match. |

**Returns:** SearchQuery: A regular expression query.

## create_regex_query {#pattern-options}

Creates a regular expression query.

The `options` argument must include the `RegexOptions.IGNORE_CASE` flag; otherwise a `ValueError` is raised. If only the `pattern` argument is provided, `IGNORE_CASE` is applied automatically. Python's `re` module flags are accepted and translated (e.g., `re.IGNORECASE` becomes `RegexOptions.IGNORE_CASE`).

```python
def create_regex_query(cls, pattern, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| pattern | `str` | The regular expression pattern to match. |
| options | `System.Text.RegularExpressions.RegexOptions` | A bitwise combination of `RegexOptions` values that modify the regular expression. Must contain `RegexOptions.IGNORE_CASE`. |

**Returns:** SearchQuery: A regular expression query.

| Raises | Description |
| :- | :- |
| `ValueError` | If `options` does not contain the `IGNORE_CASE` flag. |

### Example

```python
from groupdocs.search import SearchQuery, RegexOptions

# Create a regex query with custom options
regex_options = RegexOptions.IGNORE_CASE | RegexOptions.CULTURE_INVARIANT
query = SearchQuery.create_regex_query(r"^(.)\\1{1,}", regex_options)

# Simple query using the default IGNORE_CASE option
simple_query = SearchQuery.create_regex_query(r"(.)\1")
```

### Aliases

These names call `create_regex_query` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_regex_query_file` | `create_regex_query_file(pattern, options)`<br>`create_regex_query_file(pattern)` |
| `create_regex_query_string` | `create_regex_query_string(pattern, options)`<br>`create_regex_query_string(pattern)` |

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
