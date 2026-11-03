---
title: add method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds a password for a document to the dictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/passworddictionary/add/
is_root: false
weight: 1010
---


## add {#key-password}

Adds a password for a document to the dictionary.

```python
def add(self, key, password):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| key | `str` | The full file path or a document key. |
| password | `str` | The document password. |

### Example

```python
# Assuming `index` is an opened GroupDocs Search index
passwords = index.dictionaries.document_passwords
passwords.add(key="/docs/confidential.pdf", password="mySecret")
```

### Aliases

These names call `add` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_file` | `add_file(key, password)` |
| `add_string` | `add_string(key, password)` |

### See Also
* class [`PasswordDictionary`](/search/python-net/groupdocs.search.dictionaries/passworddictionary/)
