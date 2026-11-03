---
title: Index class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the main class for indexing documents and searching through them."
type: docs
url: /python-net/groupdocs.search/index/
is_root: false
weight: 40
---


## Index class

Represents the main class for indexing documents and searching through them.

Learn more:
- Creating an index: https://docs.groupdocs.com/search/python-net/creating-an-index/
- Indexing: https://docs.groupdocs.com/search/python-net/indexing/
- Searching: https://docs.groupdocs.com/search/python-net/searching/

The Index type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search/index/__init__/) | Initializes a new in-memory [`Index`](/search/python-net/groupdocs.search/index/) instance. |
| [__init__](/search/python-net/groupdocs.search/index/__init__/#settings) | Initializes a new Index instance in memory with the specified index settings. |
| [__init__](/search/python-net/groupdocs.search/index/__init__/#index_folder) | Initializes a new Index, creating a new or opening an existing index on disk. |
| [__init__](/search/python-net/groupdocs.search/index/__init__/#index_folder-settings) | Initializes a new Index with the specified folder and settings. |
| [__init__](/search/python-net/groupdocs.search/index/__init__/#index_folder-overwrite_if_exists) | Initializes a new Index instance. |
| [__init__](/search/python-net/groupdocs.search/index/__init__/#index_folder-settings-overwrite_if_exists) | Initializes a new [`Index`](/search/python-net/groupdocs.search/index/) instance. Loads an existing index from disk if `overwrite_if_exists` is `False`; otherwise creates a new index on disk with the specified index settings. |

### Methods
| Method | Description |
| :- | :- |
| [add](/search/python-net/groupdocs.search/index/add/#path) | Performs indexing operation by adding a file or folder specified by an absolute or relative path; documents in all subfolders are indexed. |
| [add](/search/python-net/groupdocs.search/index/add/#path-options) | Adds a file or folder by an absolute or relative path, indexing documents from all subfolders. |
| [add](/search/python-net/groupdocs.search/index/add/#paths) | Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed. |
| [add](/search/python-net/groupdocs.search/index/add/#paths-options) | Adds files or folders by an absolute or relative path, indexing documents from all subfolders. |
| [add](/search/python-net/groupdocs.search/index/add/#documents-options) | Indexes documents from the file system, a stream, or a structured source. |
| [add](/search/python-net/groupdocs.search/index/add/#data-options) | Performs an indexing operation and adds the extracted data to the index. |
| [change_attributes](/search/python-net/groupdocs.search/index/change_attributes/#batch) | Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation. |
| [check_segments](/search/python-net/groupdocs.search/index/check_segments/#fix_index_functionality) | Checks the index for damaged segment files on the disk and optionally fixes index functionality if `fix_index_functionality` is True. |
| [delete](/search/python-net/groupdocs.search/index/delete/#paths-options) | Deletes indexed files or folders from the index and updates the index without the deleted paths. |
| [delete](/search/python-net/groupdocs.search/index/delete/#options-document_keys) | Deletes documents indexed from streams or structures and updates the index without the deleted documents. |
| [dispose](/search/python-net/groupdocs.search/index/dispose/) | Releases all resources used by the [`Index`](/search/python-net/groupdocs.search/index/). |
| [get_attributes](/search/python-net/groupdocs.search/index/get_attributes/#path) | Gets all the attributes associated with the specified indexed document. |
| [get_document_text](/search/python-net/groupdocs.search/index/get_document_text/#document_info-adapter) | Generates the text of an indexed document and passes it through an output adapter. |
| [get_document_text](/search/python-net/groupdocs.search/index/get_document_text/#document_info-adapter-options) | Generates HTML formatted text for an indexed document and transfers it through the output adapter. |
| [get_indexed_document](/search/python-net/groupdocs.search/index/get_indexed_document/#document_key) | Gets an indexed document by document key. |
| [get_indexed_document_items](/search/python-net/groupdocs.search/index/get_indexed_document_items/#document_info) | Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST). |
| [get_indexed_documents](/search/python-net/groupdocs.search/index/get_indexed_documents/) | Gets an array of all indexed documents. |
| [get_indexed_paths](/search/python-net/groupdocs.search/index/get_indexed_paths/) | Returns a list of indexed paths – documents or folders. |
| [get_indexing_reports](/search/python-net/groupdocs.search/index/get_indexing_reports/) | Gets the reports on indexing operations. |
| [get_search_reports](/search/python-net/groupdocs.search/index/get_search_reports/) | Retrieves the reports on search operations. |
| [highlight](/search/python-net/groupdocs.search/index/highlight/#document-highlighter) | Generates HTML formatted text with highlighted found terms. |
| [highlight](/search/python-net/groupdocs.search/index/highlight/#document-highlighter-options) | Generates HTML formatted text with highlighted found terms. |
| [load_into_memory_completely](/search/python-net/groupdocs.search/index/load_into_memory_completely/#index_folder) | Loads the entire index into memory. |
| [load_into_memory_completely](/search/python-net/groupdocs.search/index/load_into_memory_completely/#index_folder-settings) | Loads the entire index into memory. |
| [merge](/search/python-net/groupdocs.search/index/merge/#index-options) | Merges the specified index into the current index. |
| [merge](/search/python-net/groupdocs.search/index/merge/#repository-options) | Merges indexes from the specified index repository into the current index. |
| [notify](/search/python-net/groupdocs.search/index/notify/#notification) | Passes the specified notification object to the index to perform the notification. |
| [optimize](/search/python-net/groupdocs.search/index/optimize/) | Minimizes the number of index segments by merging them, improving search performance. |
| [optimize](/search/python-net/groupdocs.search/index/optimize/#options) | Minimizes the number of index segments by merging them, improving search performance. |
| [save_to](/search/python-net/groupdocs.search/index/save_to/#index_folder) | Saves the in‑memory or regular index to a specified folder on disk without changing its settings. |
| [search](/search/python-net/groupdocs.search/index/search/#query) | Searches in index. |
| [search](/search/python-net/groupdocs.search/index/search/#query-options) | Searches in the index. |
| [search](/search/python-net/groupdocs.search/index/search/#query) | Searches in index. |
| [search](/search/python-net/groupdocs.search/index/search/#query-options) | Searches in index. |
| [search](/search/python-net/groupdocs.search/index/search/#image-options) | Performs a reverse image search in the index. |
| [search_next](/search/python-net/groupdocs.search/index/search_next/#chunk_search_token) | Continues the chunk search started with method Search. |
| [search_next](/search/python-net/groupdocs.search/index/search_next/#chunk_search_token-cancellation) | Continues the chunk search started with [`Index.search`](/search/python-net/groupdocs.search/index/search/). |
| [update](/search/python-net/groupdocs.search/index/update/) | Re-indexes documents that have been changed or deleted since the last update and adds new files that have been added to the indexed folders. |
| [update](/search/python-net/groupdocs.search/index/update/#options) | Re-indexes documents that have been changed or deleted since the last update and adds new files that have been added to the indexed folders. |

### Properties
| Property | Description |
| :- | :- |
| [dictionaries](/search/python-net/groupdocs.search/index/dictionaries/) | The dictionary repository. |
| [events](/search/python-net/groupdocs.search/index/events/) | The event hub for subscribing to events. |
| [index_info](/search/python-net/groupdocs.search/index/index_info/) | The basic information on the index. |
| [index_settings](/search/python-net/groupdocs.search/index/index_settings/) | The index settings. |
| [repository](/search/python-net/groupdocs.search/index/repository/) | The index repository object if the index is contained in it. |

### Example

```python
from groupdocs.search import Index

def on_file_indexing(sender, args):
    print("Indexing:", args.document_full_path)

with Index("./index") as index:
    index.events.file_indexing += on_file_indexing
    index.add("./documents")
```

### Guides
Task guides that use `Index`:

* [Hello, World!](/search/python-net/guides/hello-world/)
* [Build your first search solution](/search/python-net/guides/build-your-first-search-solution/)
* [Build search query](/search/python-net/guides/build-search-query/)
* [Work with search results](/search/python-net/guides/work-with-search-results/)
* [Search index events](/search/python-net/guides/search-index-events/)
* [Phrase search](/search/python-net/guides/phrase-search/)
* [Wildcard search](/search/python-net/guides/wildcard-search/)
* [Fuzzy search](/search/python-net/guides/fuzzy-search/)
* [Regular expression search](/search/python-net/guides/regular-expression-search/)
* [Boolean search](/search/python-net/guides/boolean-search/)
* [Faceted search](/search/python-net/guides/faceted-search/)
* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)
* [Custom text extractors](/search/python-net/guides/custom-text-extractors/)

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
