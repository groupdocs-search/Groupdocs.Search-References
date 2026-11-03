---
title: CharacterReplacementDictionary class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a character replacement dictionary used during indexing, allowing character replacement such as removing accents or enabling case‑insensitive indexing."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/
is_root: false
weight: 40
---


## CharacterReplacementDictionary class

Represents a character replacement dictionary used during indexing, allowing character replacement such as removing accents or enabling case‑insensitive indexing.

The dictionary defines how the text of documents is divided into terms. It can be changed only while the index contains no documents and its status is `IndexStatus.ready`; otherwise a method that changes the dictionary raises `RuntimeError`. Calls that do not modify the dictionary content are always allowed. To apply a different dictionary to documents that are already indexed, create a new index and re‑index the documents.

A change to the dictionary is saved to the index immediately. If the change cannot be saved, the method raises the exception that describes the failure, and the dictionary remains unchanged.

Learn more
- https://docs.groupdocs.com/search/python-net/character-replacement-during-indexing/
- https://docs.groupdocs.com/search/python-net/character-replacements/

The CharacterReplacementDictionary type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [add_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/add_range/#character_replacements) | Adds the specified collection of character replacements to this [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [add_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/add_range/#character_replacements) | Adds the specified collection of Unicode code point replacements to this instance of the CharacterReplacementDictionary. |
| [add_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/add_range/#character_replacements) | Adds the specified collection of character replacements to this instance of the CharacterReplacementDictionary. |
| [add_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/add_range/#character_replacements) | Adds the specified collection of character replacements to this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [clear](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/clear/) | Removes all character replacements from the dictionary. |
| [contains](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/contains/#code_point) | Determines whether a [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/) object contains a replacement for the specified Unicode code point. |
| [get_enumerator](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/get_enumerator/) | Returns an enumerator that iterates through the collection. |
| [get_replacement](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/get_replacement/#code_point) | Returns the replacement for the specified Unicode code point. |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/remove_range/#characters) | Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/remove_range/#code_points) | Removes the specified collection of Unicode code point replacements from this [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/remove_range/#characters) | Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/remove_range/#code_points) | Removes the specified collection of Unicode code points replacements from this instance of the CharacterReplacementDictionary. |
| [export_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/export_dictionary/) | Exports the dictionary to a file with the specified name. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |
| [import_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/import_dictionary/) | Imports a dictionary from the specified file. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |

### Properties
| Property | Description |
| :- | :- |
| [count](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/count/) | The number of Unicode code points contained in this [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/). |
| [dictionary_type](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/dictionary_type/) | The dictionary type. |

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
