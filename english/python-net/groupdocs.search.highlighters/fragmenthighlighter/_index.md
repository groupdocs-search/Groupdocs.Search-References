---
title: FragmentHighlighter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search result highlighter that highlights search results in text fragments."
type: docs
url: /python-net/groupdocs.search.highlighters/fragmenthighlighter/
is_root: false
weight: 20
---


## FragmentHighlighter class

Represents a search result highlighter that highlights search results in text fragments.

Learn more:
- Highlighting search results (https://docs.groupdocs.com/search/python-net/highlighting-search-results/)

The FragmentHighlighter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.highlighters/fragmenthighlighter/__init__/#output_format) | Initializes a new instance of the [`FragmentHighlighter`](/search/python-net/groupdocs.search.highlighters/fragmenthighlighter/) class. |

### Methods
| Method | Description |
| :- | :- |
| [get_result](/search/python-net/groupdocs.search.highlighters/fragmenthighlighter/get_result/) | Returns an array of resulting fragment containers. |

### Properties
| Property | Description |
| :- | :- |
| [output_format](/search/python-net/groupdocs.search.common/resultbuilderfactory/output_format/) | The output format. (inherited from [`ResultBuilderFactory`](/search/python-net/groupdocs.search.common/resultbuilderfactory/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.highlighters import FragmentHighlighter
from groupdocs.search.options import HighlightOptions, OutputFormat

index_folder = "./MyIndex"
documents_folder = "./documents"

# Create an index and add documents
index = Index(index_folder)
index.add(documents_folder)

# Search for a term
result = index.search("Einstein")

# Configure highlight options
options = HighlightOptions()
options.terms_before = 5
options.terms_after = 5
options.terms_total = 15

# Highlight the first found document
document = result.get_found_document(0)
highlighter = FragmentHighlighter(OutputFormat.HTML)
index.highlight(document, highlighter, options)

# Retrieve and print highlighted fragments
for container in highlighter.get_result():
    fragments = container.get_fragments()
    if fragments:
        print(container.field_name)
        for fragment in fragments:
            print(fragment)
```

### Guides
Task guides that use `FragmentHighlighter`:

* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)

### See Also
* module [`groupdocs.search.highlighters`](/search/python-net/groupdocs.search.highlighters/)
