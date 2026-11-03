---
title: SearchQuery class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search query in object form."
type: docs
url: /python-net/groupdocs.search/searchquery/
is_root: false
weight: 110
---


## SearchQuery class

Represents a search query in object form.

Learn more:
- https://docs.groupdocs.com/search/python-net/searching/
- https://docs.groupdocs.com/search/python-net/queries-in-text-and-object-form/
- https://docs.groupdocs.com/search/python-net/nesting-search-queries-in-object-form/

The SearchQuery type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [create_and_query](/search/python-net/groupdocs.search/searchquery/create_and_query/#left_query-right_query) | Creates a combined query that will find only documents which will be found for each original query. |
| [create_and_query](/search/python-net/groupdocs.search/searchquery/create_and_query/#queries) | Creates a combined query that will find only documents which will be found for each original query. |
| [create_date_range_query](/search/python-net/groupdocs.search/searchquery/create_date_range_query/#start-end) | Creates a date range query. |
| [create_field_query](/search/python-net/groupdocs.search/searchquery/create_field_query/#field_name-query) | Adds a field to the specified query. |
| [create_not_query](/search/python-net/groupdocs.search/searchquery/create_not_query/#query) | Creates an inverted query that matches all documents not matching the specified query. |
| [create_numeric_range_query](/search/python-net/groupdocs.search/searchquery/create_numeric_range_query/#start-end) | Creates a numeric range query. |
| [create_or_query](/search/python-net/groupdocs.search/searchquery/create_or_query/#left_query-right_query) | Creates a combined query that will find all the documents which will be found at least for one of the original queries. |
| [create_or_query](/search/python-net/groupdocs.search/searchquery/create_or_query/#queries) | Creates a combined query that finds documents matching at least one of the original queries. |
| [create_phrase_search_query](/search/python-net/groupdocs.search/searchquery/create_phrase_search_query/#queries) | Creates a phrase search query. |
| [create_regex_query](/search/python-net/groupdocs.search/searchquery/create_regex_query/#pattern) | Creates a regular expression query. |
| [create_regex_query](/search/python-net/groupdocs.search/searchquery/create_regex_query/#pattern-options) | Creates a regular expression query. |
| [create_wildcard_query](/search/python-net/groupdocs.search/searchquery/create_wildcard_query/#count) | Creates a wildcard for the phrase search. |
| [create_wildcard_query](/search/python-net/groupdocs.search/searchquery/create_wildcard_query/#min_count-max_count) | Creates a wildcard for the phrase search. |
| [create_word_pattern_query](/search/python-net/groupdocs.search/searchquery/create_word_pattern_query/#pattern) | Creates a word pattern query. |
| [create_word_query](/search/python-net/groupdocs.search/searchquery/create_word_query/#term) | Creates a simple word query. |
| [get_child](/search/python-net/groupdocs.search/searchquery/get_child/#index) | Gets a child query by its index. |
| [to_string](/search/python-net/groupdocs.search/searchquery/to_string/) | Returns a str that represents the current SearchQuery instance. |

### Properties
| Property | Description |
| :- | :- |
| [child_count](/search/python-net/groupdocs.search/searchquery/child_count/) | The number of child queries. |
| [field_name](/search/python-net/groupdocs.search/searchquery/field_name/) | The field name. |
| [first_child](/search/python-net/groupdocs.search/searchquery/first_child/) | The first child query. |
| [search_options](/search/python-net/groupdocs.search/searchquery/search_options/) | The search options of this search query. |
| [second_child](/search/python-net/groupdocs.search/searchquery/second_child/) | The second child query. |

### Example

```python
import datetime
from groupdocs.search import Index, SearchQuery
from groupdocs.search.options import SearchOptions, TableDiscreteFunction

# Create an index and add documents
index_folder = "./MyIndex"
documents_folder = "./documents"
index = Index(index_folder)
index.add(documents_folder)

# Create subqueries
subquery1 = SearchQuery.create_date_range_query(
    datetime.datetime(2011, 6, 17), datetime.datetime(2013, 1, 1)
)
subquery2 = SearchQuery.create_wildcard_query(0, 2)
subquery3 = SearchQuery.create_word_query("birth")
subquery3.search_options = SearchOptions()
subquery3.search_options.fuzzy_search.enabled = True
subquery3.search_options.fuzzy_search.fuzzy_algorithm = TableDiscreteFunction(1)

# Combine subqueries into a phrase search query
query = SearchQuery.create_phrase_search_query(subquery1, subquery2, subquery3)

# Set overall search options
options = SearchOptions()
options.max_occurrence_count_per_term = 1_000_000
options.max_total_occurrence_count = 10_000_000

# Execute the search
result = index.search(query, options)
```

### Guides
Task guides that use `SearchQuery`:

* [Phrase search](/search/python-net/guides/phrase-search/)
* [Wildcard search](/search/python-net/guides/wildcard-search/)
* [Regular expression search](/search/python-net/guides/regular-expression-search/)
* [Boolean search](/search/python-net/guides/boolean-search/)
* [Faceted search](/search/python-net/guides/faceted-search/)

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
