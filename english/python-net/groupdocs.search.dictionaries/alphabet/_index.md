---
title: Alphabet class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a dictionary of characters that is used during indexing to detect character type."
type: docs
url: /python-net/groupdocs.search.dictionaries/alphabet/
is_root: false
weight: 30
---


## Alphabet class

Represents a dictionary of characters that is used during indexing to detect character type.

The dictionary defines how the text of documents is divided into terms. Therefore the dictionary of an index can be changed only while the index contains no documents and its status is `IndexStatus.ready`; otherwise a method that changes the dictionary throws a `RuntimeError`. A call that does not change the content of the dictionary is always allowed. To use another content with documents that are already indexed, create a new index and index the documents again.

A change of the dictionary of an index is saved in the index at once. If it cannot be saved, the method throws the exception that describes the failure, and the dictionary stays unchanged.

- Character types (https://docs.groupdocs.com/search/python-net/character-types/)
- Managing alphabet (https://docs.groupdocs.com/search/python-net/alphabet/)

The Alphabet type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [clear](/search/python-net/groupdocs.search.dictionaries/alphabet/clear/) | Sets the Separator type for all characters in this Alphabet. |
| [get_character_type](/search/python-net/groupdocs.search.dictionaries/alphabet/get_character_type/#character) | Gets the type of a character. |
| [get_character_type](/search/python-net/groupdocs.search.dictionaries/alphabet/get_character_type/#code_point) | Gets the type of a Unicode code point. |
| [get_character_type](/search/python-net/groupdocs.search.dictionaries/alphabet/get_character_type/#character) | Gets the type of a character. |
| [get_enumerator](/search/python-net/groupdocs.search.dictionaries/alphabet/get_enumerator/) | Returns an enumerator that iterates through the collection. |
| [set_range](/search/python-net/groupdocs.search.dictionaries/alphabet/set_range/#characters-type) | Sets the character type for each character in the specified collection. |
| [set_range](/search/python-net/groupdocs.search.dictionaries/alphabet/set_range/#characters-type) | Sets the type for each character in the specified collection for this Alphabet instance. |
| [set_range](/search/python-net/groupdocs.search.dictionaries/alphabet/set_range/#code_points-type) | Sets the character type for each Unicode code point in the given collection. |
| [export_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/export_dictionary/) | Exports the dictionary to a file with the specified name. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |
| [import_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/import_dictionary/) | Imports a dictionary from the specified file. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |

### Properties
| Property | Description |
| :- | :- |
| [count](/search/python-net/groupdocs.search.dictionaries/alphabet/count/) | The number of characters contained in the Alphabet dictionary. |
| [dictionary_type](/search/python-net/groupdocs.search.dictionaries/alphabet/dictionary_type/) | The dictionary type. |

### Example

```python
# Export the alphabet to a file
alphabet.export_dictionary("./Alphabet.dat")

# Import the alphabet into another index and inspect it
new_index.dictionaries.alphabet.import_dictionary("./Alphabet.dat")
print("Characters that are not separators:", new_index.dictionaries.alphabet.count)
```

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
