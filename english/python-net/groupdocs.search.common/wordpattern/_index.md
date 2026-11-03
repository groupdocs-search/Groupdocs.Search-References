---
title: WordPattern class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a word pattern for the wildcard search."
type: docs
url: /python-net/groupdocs.search.common/wordpattern/
is_root: false
weight: 350
---


## WordPattern class

Represents a word pattern for the wildcard search.

A pattern is a sequence of values, each of them either a character or a wildcard. A wildcard carries the flag that puts it above `System.Char.MaxValue`, together with the least and the greatest number of characters it stands for, therefore a character of the pattern is anything that fits into a UTF-16 code unit.

The WordPattern type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/wordpattern/__init__/) | Initializes a new instance of the [`WordPattern`](/search/python-net/groupdocs.search.common/wordpattern/) class. |

### Methods
| Method | Description |
| :- | :- |
| [append_character](/search/python-net/groupdocs.search.common/wordpattern/append_character/#character) | Appends a character to the word pattern. |
| [append_one_character_wildcard](/search/python-net/groupdocs.search.common/wordpattern/append_one_character_wildcard/) | Appends a wildcard for exactly one character to the word pattern. |
| [append_one_or_more_characters_wildcard](/search/python-net/groupdocs.search.common/wordpattern/append_one_or_more_characters_wildcard/) | Appends a wildcard that matches one or more characters to the word pattern. |
| [append_string](/search/python-net/groupdocs.search.common/wordpattern/append_string/#text) | Appends a string to the word pattern. |
| [append_wildcard](/search/python-net/groupdocs.search.common/wordpattern/append_wildcard/#min-max) | Appends a wildcard to the word pattern. |
| [append_zero_or_more_characters_wildcard](/search/python-net/groupdocs.search.common/wordpattern/append_zero_or_more_characters_wildcard/) | Appends a wildcard that matches zero to 255 characters to the word pattern. |
| [append_zero_or_one_character_wildcard](/search/python-net/groupdocs.search.common/wordpattern/append_zero_or_one_character_wildcard/) | Appends a zero-or-one character wildcard to the word pattern. |
| [to_string](/search/python-net/groupdocs.search.common/wordpattern/to_string/) | Returns a string that represents the current WordPattern. |

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.common import WordPattern

# Create a pattern that matches words like "merry" or "marry"
pattern = WordPattern()
pattern.append_string("m")
pattern.append_one_character_wildcard()
pattern.append_string("rry")
query = SearchQuery.create_word_pattern_query(pattern)
result = index.search(query)

# Create a pattern that matches words like "cardiff", "cardinal", "cardio", "cards"
pattern2 = WordPattern()
pattern2.append_string("card")
pattern2.append_wildcard(1, 6)  # matches between 1 and 6 characters
query2 = SearchQuery.create_word_pattern_query(pattern2)
result2 = index.search(query2)
```

### Guides
Task guides that use `WordPattern`:

* [Phrase search](/search/python-net/guides/phrase-search/)
* [Wildcard search](/search/python-net/guides/wildcard-search/)

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
