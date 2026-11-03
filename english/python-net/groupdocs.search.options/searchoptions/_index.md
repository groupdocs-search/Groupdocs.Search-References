---
title: SearchOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for search operation."
type: docs
url: /python-net/groupdocs.search.options/searchoptions/
is_root: false
weight: 350
---


## SearchOptions class

Provides options for search operation.

Learn more

- https://docs.groupdocs.com/search/python-net/search-options/

The SearchOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/searchoptions/__init__/) | Initializes a new instance of the [`SearchOptions`](/search/python-net/groupdocs.search.options/searchoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [cancellation](/search/python-net/groupdocs.search.options/searchoptions/cancellation/) | The operation cancellation object, defaulting to None. |
| [date_formats](/search/python-net/groupdocs.search.options/searchoptions/date_formats/) | The collection of date formats for date range search. The default date formats are `'dd.MM.yyyy'`, `'MM/dd/yyyy'`, and `'yyyy-MM-dd'`. |
| [fuzzy_search](/search/python-net/groupdocs.search.options/searchoptions/fuzzy_search/) | The fuzzy search options. |
| [is_chunk_search](/search/python-net/groupdocs.search.options/searchoptions/is_chunk_search/) | The flag of search by chunks. The default value is False. |
| [keyboard_layout_corrector](/search/python-net/groupdocs.search.options/searchoptions/keyboard_layout_corrector/) | The keyboard layout corrector options. |
| [max_occurrence_count_per_term](/search/python-net/groupdocs.search.options/searchoptions/max_occurrence_count_per_term/) | The maximum number of occurrences of each term in a search query (default is 2000000000). |
| [max_total_occurrence_count](/search/python-net/groupdocs.search.options/searchoptions/max_total_occurrence_count/) | The maximum total number of occurrences of all terms in a search query (default is 2000000000). |
| [retrieve_attributes](/search/python-net/groupdocs.search.options/searchoptions/retrieve_attributes/) | The flag of retrieving attributes associated with found documents. |
| [search_document_filter](/search/python-net/groupdocs.search.options/searchoptions/search_document_filter/) | The search document filter. The default value is None, which means that all found documents will be returned. |
| [spelling_corrector](/search/python-net/groupdocs.search.options/searchoptions/spelling_corrector/) | The spelling corrector options. |
| [use_case_sensitive_search](/search/python-net/groupdocs.search.options/searchoptions/use_case_sensitive_search/) | The flag indicating whether the search is case‑sensitive. The default value is False. |
| [use_homophone_search](/search/python-net/groupdocs.search.options/searchoptions/use_homophone_search/) | The flag indicating whether homophones are used in search (default: False). |
| [use_synonym_search](/search/python-net/groupdocs.search.options/searchoptions/use_synonym_search/) | The flag of use synonyms in search; default is False. |
| [use_word_forms_search](/search/python-net/groupdocs.search.options/searchoptions/use_word_forms_search/) | The flag indicating whether to use different word forms in search. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions

with Index("./index") as index:
    index.add("./documents")

    options = SearchOptions()
    options.fuzzy_search.enabled = True  # Enable fuzzy search

    result = index.search("Einstein", options)
    print("Documents found:", result.document_count)
```

### Guides
Task guides that use `SearchOptions`:

* [Build search query](/search/python-net/guides/build-search-query/)
* [Work with search results](/search/python-net/guides/work-with-search-results/)
* [Search index events](/search/python-net/guides/search-index-events/)
* [Fuzzy search](/search/python-net/guides/fuzzy-search/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
