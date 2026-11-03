---
title: StopWordDictionary class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a dictionary of stop words."
type: docs
url: /python-net/groupdocs.search.dictionaries/stopworddictionary/
is_root: false
weight: 150
---


## StopWordDictionary class

Represents a dictionary of stop words.

The dictionary defines how the text of documents is divided into terms. Therefore the dictionary of an index can be changed only while the index contains no documents and its status is `IndexStatus.ready`; otherwise a method that changes the dictionary throws `RuntimeError`. A call that does not change the content of the dictionary is always allowed. To use another content with documents that are indexed already, create a new index and index the documents again.

A change of the dictionary of an index is saved in the index at once. If it cannot be saved, the method throws the exception that describes the failure, and the dictionary stays unchanged.

- [Indexing with stop words](https://docs.groupdocs.com/search/python-net/indexing-with-stop-words/)
- [Managing stop word dictionary](https://docs.groupdocs.com/search/python-net/stop-word-dictionary/)

The StopWordDictionary type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [add_range](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/add_range/#words) | Adds the specified collection of words to this StopWordDictionary. |
| [add_range](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/add_range/#words) | Adds the specified collection of words to the StopWordDictionary instance. |
| [clear](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/clear/) | Removes all words from the StopWordDictionary. |
| [contains](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/contains/#word) | Determines whether the StopWordDictionary contains the specified word. |
| [get_enumerator](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/get_enumerator/) | Returns an iterator that iterates through the collection. |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/remove_range/#words) | Removes the specified collection of words from this StopWordDictionary. |
| [remove_range](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/remove_range/#words) | Removes the specified collection of words from this StopWordDictionary. |
| [export_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/export_dictionary/) | Exports the dictionary to a file with the specified name. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |
| [import_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionarybase/import_dictionary/) | Imports a dictionary from the specified file. (inherited from [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)) |

### Properties
| Property | Description |
| :- | :- |
| [count](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/count/) | The number of stop words contained in the [`StopWordDictionary`](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/). |
| [dictionary_type](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/dictionary_type/) | The dictionary type. |

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
