---
title: IWordFormsProvider class
second_title: GroupDocs.Search for Python via .NET API References
description: "Defines interface of a word forms provider."
type: docs
url: /python-net/groupdocs.search.dictionaries/iwordformsprovider/
is_root: false
weight: 120
---


## IWordFormsProvider class

Defines interface of a word forms provider.

Learn more

- [Search for different word forms](https://docs.groupdocs.com/search/python-net/search-for-different-word-forms/)
- [Word forms provider](https://docs.groupdocs.com/search/python-net/word-forms-provider/)

The IWordFormsProvider type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [get_word_forms](/search/python-net/groupdocs.search.dictionaries/iwordformsprovider/get_word_forms/#word) | Gets the word forms for the specified word. |

### Example

```python
class SimpleWordFormsProvider:
    def get_word_forms(self, word):
        result = []
        lower_word = word.lower()

        # Assume the input word is plural, add singular forms
        if len(word) > 3 and lower_word.endswith("ies"):
            result.append(word[:-3] + "y")
        if len(word) > 2 and lower_word.endswith("es"):
            result.append(word[:-2])
        if len(word) > 1 and lower_word.endswith("s"):
            result.append(word[:-1])

        # Assume the input word is singular, add plural forms
        if len(word) > 1 and lower_word.endswith("y"):
            result.append(word[:-1] + "ies")
        elif lower_word.endswith(("s", "x", "ch", "sh")):
            result.append(word + "es")
        else:
            result.append(word + "s")

        return result
```

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
