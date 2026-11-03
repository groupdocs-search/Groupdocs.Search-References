---
title: MetadataIndexingOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for indexing metadata fields."
type: docs
url: /python-net/groupdocs.search.options/metadataindexingoptions/
is_root: false
weight: 270
---


## MetadataIndexingOptions class

Provides options for indexing metadata fields.

Learn more

- Indexing options: https://docs.groupdocs.com/search/python-net/indexing-options/
- MetadataIndexingOptions are used when retrieving document text from an index: https://docs.groupdocs.com/search/python-net/getting-indexed-documents/
- MetadataIndexingOptions are used when highlighting search results: https://docs.groupdocs.com/search/python-net/highlighting-search-results/

The MetadataIndexingOptions type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [default_field_name](/search/python-net/groupdocs.search.options/metadataindexingoptions/default_field_name/) | The default field name used to index empty field names. The default value is `"unknown"`. |
| [indexing_empty_names](/search/python-net/groupdocs.search.options/metadataindexingoptions/indexing_empty_names/) | The indexing_empty_names property indicates whether to index empty field names. |
| [indexing_empty_values](/search/python-net/groupdocs.search.options/metadataindexingoptions/indexing_empty_values/) | The value indicating whether to index empty field values. The default is True. |
| [max_bytes_to_index_field](/search/python-net/groupdocs.search.options/metadataindexingoptions/max_bytes_to_index_field/) | The maximum number of values in an array of type byte to index the field. The default value is int.MaxValue. |
| [max_doubles_to_index_field](/search/python-net/groupdocs.search.options/metadataindexingoptions/max_doubles_to_index_field/) | The maximum number of values in an array of type double to index the field. The default value is `int.MaxValue`. |
| [max_ints_to_index_field](/search/python-net/groupdocs.search.options/metadataindexingoptions/max_ints_to_index_field/) | The maximum number of integer values in an array to index the field. The default value is `int.MaxValue`. |
| [max_longs_to_index_field](/search/python-net/groupdocs.search.options/metadataindexingoptions/max_longs_to_index_field/) | The maximum number of values in an array of type long to index the field. |
| [separator_between_values](/search/python-net/groupdocs.search.options/metadataindexingoptions/separator_between_values/) | The separator between values in a field of type array. The default value is a space character. |
| [separator_in_compound_name](/search/python-net/groupdocs.search.options/metadataindexingoptions/separator_in_compound_name/) | The separator in the compound name of a field. The default value is ".". |

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
