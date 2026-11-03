---
title: FuzzySearchOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options of the fuzzy search."
type: docs
url: /python-net/groupdocs.search.options/fuzzysearchoptions/
is_root: false
weight: 150
---


## FuzzySearchOptions class

Provides options of the fuzzy search.

- [Fuzzy search](https://docs.groupdocs.com/search/python-net/fuzzy-search/)
- [Search options](https://docs.groupdocs.com/search/python-net/search-options/)

The FuzzySearchOptions type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [consider_transpositions](/search/python-net/groupdocs.search.options/fuzzysearchoptions/consider_transpositions/) | The property indicates whether the fuzzy search algorithm treats a transposition of two adjacent characters as a single mistake. |
| [enabled](/search/python-net/groupdocs.search.options/fuzzysearchoptions/enabled/) | The fuzzy search feature is enabled when True, otherwise disabled; defaults to False. |
| [fuzzy_algorithm](/search/python-net/groupdocs.search.options/fuzzysearchoptions/fuzzy_algorithm/) | The fuzzy search algorithm. The currently available fuzzy search algorithms are [`SimilarityLevel`](/search/python-net/groupdocs.search.options/similaritylevel/) and [`TableDiscreteFunction`](/search/python-net/groupdocs.search.options/tablediscretefunction/). The default value is an instance of [`SimilarityLevel`](/search/python-net/groupdocs.search.options/similaritylevel/) with a similarity level value of 0.5. |
| [only_best_results](/search/python-net/groupdocs.search.options/fuzzysearchoptions/only_best_results/) | The property indicating whether only the best results will be returned. The default value is False. |
| [only_best_results_range](/search/python-net/groupdocs.search.options/fuzzysearchoptions/only_best_results_range/) | The maximum exceeding of the minimum number of mistakes found. The default value is 0. |

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
