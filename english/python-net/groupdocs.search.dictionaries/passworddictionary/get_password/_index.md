---
title: get_password method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves the password for the specified file."
type: docs
url: /python-net/groupdocs.search.dictionaries/passworddictionary/get_password/
is_root: false
weight: 1060
---


## get_password {#key}

Retrieves the password for the specified file.

```python
def get_password(self, key):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| key | `str` | The full file path or a document key. |

**Returns:** str: The password for the document.

### Example

```python
import os

from groupdocs.search import Index

index = Index("./index")
passwords = index.dictionaries.document_passwords

# The key is the full path of the document
document_path = os.path.abspath("./documents/protected.pdf")
passwords.add(document_path, "123456")
print(passwords.get_password(document_path))
```

### Aliases

These names call `get_password` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_password_file` | `get_password_file(key)` |
| `get_password_string` | `get_password_string(key)` |

### See Also
* class [`PasswordDictionary`](/search/python-net/groupdocs.search.dictionaries/passworddictionary/)
