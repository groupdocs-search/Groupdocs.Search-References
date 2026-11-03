---
title: DictionaryRepository class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a repository of all dictionaries in the System.Index."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionaryrepository/
is_root: false
weight: 80
---


## DictionaryRepository class

Represents a repository of all dictionaries in the [`System.Index`](/search/python-net/groupdocs.search/index/).

The dictionaries [`DictionaryRepository.alphabet`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/alphabet/),
[`DictionaryRepository.tokenization_dictionary`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/tokenization_dictionary/),
[`DictionaryRepository.character_replacements`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/character_replacements/) and
[`DictionaryRepository.stop_word_dictionary`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/stop_word_dictionary/) define how the text of documents is divided into terms.
Therefore they can be changed only while the index contains no documents and its status is `IndexStatus.ready`. The other dictionaries can be changed at any time.

The DictionaryRepository type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [alias_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/alias_dictionary/) | The dictionary of aliases. |
| [alphabet](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/alphabet/) | The dictionary of characters used by the internal tokenization mechanism to split text into words. |
| [character_replacements](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/character_replacements/) | The dictionary of character replacements. |
| [document_passwords](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/document_passwords/) | The dictionary of document passwords. |
| [homophone_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/homophone_dictionary/) | The dictionary of homophones. |
| [spelling_corrector](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/spelling_corrector/) | The spelling corrector. |
| [stop_word_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/stop_word_dictionary/) | The dictionary of stop words. |
| [synonym_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/synonym_dictionary/) | The dictionary of synonyms. |
| [tokenization_dictionary](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/tokenization_dictionary/) | The dictionary of characters that defines whether a token is considered as a valid word or a separator when using external tokenization tools. |
| [word_forms_provider](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/word_forms_provider/) | The word forms provider. |

### Example

```python
# Obtain the dictionary repository from an index instance
repo = index.dictionaries

# Access a specific dictionary, e.g., the stop‑word dictionary
stop_words = repo.StopWordDictionary
print(stop_words)
```

### See Also
* module [`groupdocs.search.dictionaries`](/search/python-net/groupdocs.search.dictionaries/)
