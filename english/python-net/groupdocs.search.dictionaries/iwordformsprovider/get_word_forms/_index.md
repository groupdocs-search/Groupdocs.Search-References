---
title: get_word_forms method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the word forms for the specified word."
type: docs
url: /python-net/groupdocs.search.dictionaries/iwordformsprovider/get_word_forms/
is_root: false
weight: 1010
---


## get_word_forms {#word}

Gets the word forms for the specified word.

```python
def get_word_forms(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word to suggest the word forms. |

**Returns:** list[str]: The word forms for the specified word or an empty list if the `IWordFormsProvider` does not provide word forms for the specified word.

### Example

```python
    class SimpleWordFormsProvider:
        def get_word_forms(self, word):
            result = []
            lower_word = word.lower()

            # plural to singular
            if len(word) > 3 and lower_word.endswith("ies"):
                result.append(word[:-3] + "y")
            if len(word) > 2 and lower_word.endswith("es"):
                result.append(word[:-2])
            if len(word) > 1 and lower_word.endswith("s"):
                result.append(word[:-1])

            # singular to plural
            if len(word) > 1 and lower_word.endswith("y"):
                result.append(word[:-1] + "ies")
            elif lower_word.endswith(("s", "x", "ch", "sh")):
                result.append(word + "es")
            else:
                result.append(word + "s")

            return result

    provider = SimpleWordFormsProvider()
    forms = provider.get_word_forms("batteries")
    print(forms)  # ['battery', 'batteri', 'batteries', 'batteries']
    ```

### Aliases

These names call `get_word_forms` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_word_forms_file` | `get_word_forms_file(word)` |
| `get_word_forms_string` | `get_word_forms_string(word)` |

### See Also
* class [`IWordFormsProvider`](/search/python-net/groupdocs.search.dictionaries/iwordformsprovider/)
