---
title: split method
second_title: GroupDocs.Search for Python via .NET API References
description: "Splits the input string into individual words."
type: docs
url: /python-net/groupdocs.search.common/iwordsplitter/split/
is_root: false
weight: 1010
---


## split {#text}

Splits the input string into individual words.

```python
def split(self, text):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| text | `str` | The input text to be split. |

**Returns:** Iterable[str]: An enumeration of words extracted from the input text.

### Example

```python
    class WhiteSpaceWordSplitter:
        def split(self, text):
            return text.split()

    splitter = WhiteSpaceWordSplitter()
    words = splitter.split("Hello world")
    print(list(words))  # ['Hello', 'world']
    ```

### Aliases

These names call `split` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `split_file` | `split_file(text)` |
| `split_string` | `split_string(text)` |

### See Also
* class [`IWordSplitter`](/search/python-net/groupdocs.search.common/iwordsplitter/)
