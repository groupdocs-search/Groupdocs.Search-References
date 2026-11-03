---
title: get_word_forms method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns the word forms for the specified word, excluding the original word."
type: docs
url: /python-net/groupdocs.search.dictionaries/englishwordformsprovider/get_word_forms/
is_root: false
weight: 1010
---


## get_word_forms {#word}

Returns the word forms for the specified word, excluding the original word.

```python
def get_word_forms(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word to suggest the word forms. |

**Returns:** list[str]: The word forms for the specified word or an empty list if the `IWordFormsProvider` does not provide word forms for the specified word.

### Aliases

These names call `get_word_forms` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_word_forms_file` | `get_word_forms_file(word)` |
| `get_word_forms_string` | `get_word_forms_string(word)` |

### See Also
* class [`EnglishWordFormsProvider`](/search/python-net/groupdocs.search.dictionaries/englishwordformsprovider/)
