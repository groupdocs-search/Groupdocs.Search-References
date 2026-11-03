---
title: Indexer class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a service that manages the distribution of indexed documents across shards of the search network."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/
is_root: false
weight: 10
---


## Indexer class

Represents a service that manages the distribution of indexed documents across shards of the search network.

The Indexer type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [add](/search/python-net/groupdocs.search.scaling/indexer/add/#documents-passwords-options) | Indexes documents from streams or structures. |
| [add](/search/python-net/groupdocs.search.scaling/indexer/add/#data-options) | Performs an indexing operation and adds the extracted data to the search network. |
| [change_attributes](/search/python-net/groupdocs.search.scaling/indexer/change_attributes/#batch-options) | Applies the specified batch of attribute changes to indexed documents without reindexing. |
| [delete](/search/python-net/groupdocs.search.scaling/indexer/delete/#document_keys-options) | Deletes indexed documents. |
| [delete_all_data](/search/python-net/groupdocs.search.scaling/indexer/delete_all_data/) | Deletes all indexed data from all shards of the search network. |
| [extract](/search/python-net/groupdocs.search.scaling/indexer/extract/#documents-passwords-options) | Extracts data from documents. |
| [get_alias_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_alias_dictionary/#shard_index) | Retrieves the alias dictionary. |
| [get_alphabet](/search/python-net/groupdocs.search.scaling/indexer/get_alphabet/#shard_index) | Gets the alphabet dictionary. |
| [get_attributes](/search/python-net/groupdocs.search.scaling/indexer/get_attributes/#document_key) | Gets all the attributes associated with the specified indexed document. |
| [get_character_replacement_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_character_replacement_dictionary/#shard_index) | Retrieves the character replacement dictionary. |
| [get_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_dictionary/#dictionary_type-shard_index) | Gets a dictionary from the specified shard. |
| [get_homophone_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_homophone_dictionary/#shard_index) | Gets the homophone dictionary. |
| [get_password_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_password_dictionary/#shard_index) | Gets the password dictionary. |
| [get_spelling_corrector](/search/python-net/groupdocs.search.scaling/indexer/get_spelling_corrector/#shard_index) | Gets the spelling corrector dictionary. |
| [get_stop_word_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_stop_word_dictionary/#shard_index) | Retrieves the stop word dictionary. |
| [get_synonym_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_synonym_dictionary/#shard_index) | Retrieves the synonym dictionary. |
| [get_tokenization_dictionary](/search/python-net/groupdocs.search.scaling/indexer/get_tokenization_dictionary/#shard_index) | Gets the tokenization dictionary. |
| [optimize](/search/python-net/groupdocs.search.scaling/indexer/optimize/#options) | Minimizes the number of index segments by merging them, improving search performance. |
| [set_dictionary](/search/python-net/groupdocs.search.scaling/indexer/set_dictionary/#dictionary-shard_index) | Sets a dictionary in the specified shard. |
| [set_dictionary](/search/python-net/groupdocs.search.scaling/indexer/set_dictionary/#dictionary) | Sets a dictionary in all shards. |
| [synchronize](/search/python-net/groupdocs.search.scaling/indexer/synchronize/#options) | Synchronizes the list of indexed documents with those on shards. |

### Properties
| Property | Description |
| :- | :- |
| [status](/search/python-net/groupdocs.search.scaling/indexer/status/) | The current search network status. |

### See Also
* module [`groupdocs.search.scaling`](/search/python-net/groupdocs.search.scaling/)
