---
title: SearchResult class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search result matching a search query."
type: docs
url: /python-net/groupdocs.search.results/searchresult/
is_root: false
weight: 100
---


## SearchResult class

Represents a search result matching a search query.

Learn more

- Searching: https://docs.groupdocs.com/search/python-net/searching/
- Search results: https://docs.groupdocs.com/search/python-net/search-results/

The SearchResult type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [get_enumerator](/search/python-net/groupdocs.search.results/searchresult/get_enumerator/) | Returns an iterator that iterates through the collection of the documents found. |
| [get_found_document](/search/python-net/groupdocs.search.results/searchresult/get_found_document/#index) | Returns the found document at the specified index. |

### Properties
| Property | Description |
| :- | :- |
| [document_count](/search/python-net/groupdocs.search.results/searchresult/document_count/) | The number of documents found. |
| [end_time](/search/python-net/groupdocs.search.results/searchresult/end_time/) | The end time of the search. |
| [next_chunk_search_token](/search/python-net/groupdocs.search.results/searchresult/next_chunk_search_token/) | The chunk search token for searching the next chunk. |
| [occurrence_count](/search/python-net/groupdocs.search.results/searchresult/occurrence_count/) | The total number of occurrences found. |
| [search_duration](/search/python-net/groupdocs.search.results/searchresult/search_duration/) | The search duration. |
| [start_time](/search/python-net/groupdocs.search.results/searchresult/start_time/) | The start time of the search. |
| [truncated](/search/python-net/groupdocs.search.results/searchresult/truncated/) | The result is truncated. |
| [warnings](/search/python-net/groupdocs.search.results/searchresult/warnings/) | The warnings describing the result. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions, TableDiscreteFunction

index_folder = "./MyIndex"
document_folder = "./documents"

# Create an index and add documents
index = Index(index_folder)
index.add(document_folder)

# Configure search options (enable fuzzy search with max 3 differences)
options = SearchOptions()
options.fuzzy_search.enabled = True
options.fuzzy_search.fuzzy_algorithm = TableDiscreteFunction(3)

# Perform search
result = index.search('Einstein OR "Theory of Relativity"', options)

print(f"Documents: {result.document_count}")
print(f"Total occurrences: {result.occurrence_count}")

for i in range(result.document_count):
    doc = result.get_found_document(i)
    print(f"\tDocument: {doc.document_info.file_path}")
    print(f"\tOccurrences: {doc.occurrence_count}")
    for field in doc.found_fields:
        print(f"\t\tField: {field.field_name}")
        print(f"\t\tOccurrences: {doc.occurrence_count}")
        if field.terms:
            for term, occ in zip(field.terms, field.terms_occurrences):
                print(f"\t\t\t{term.ljust(20)}{occ}")
        if field.term_sequences:
            for seq, occ in zip(field.term_sequences, field.term_sequences_occurrences):
                sequence = " ".join(seq)
                print(f"\t\t\t{sequence.ljust(30)}{occ}")
```

### See Also
* module [`groupdocs.search.results`](/search/python-net/groupdocs.search.results/)
