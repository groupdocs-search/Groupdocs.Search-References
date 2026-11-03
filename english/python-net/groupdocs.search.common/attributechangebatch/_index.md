---
title: AttributeChangeBatch class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a container for attribute changes."
type: docs
url: /python-net/groupdocs.search.common/attributechangebatch/
is_root: false
weight: 10
---


## AttributeChangeBatch class

Represents a container for attribute changes.

Learn more
- Document attributes: https://docs.groupdocs.com/search/python-net/document-attributes/
- Document filtering in search result: https://docs.groupdocs.com/search/python-net/document-filtering-in-search-result/

The AttributeChangeBatch type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/attributechangebatch/__init__/) | Initializes a new instance of the [`AttributeChangeBatch`](/search/python-net/groupdocs.search.common/attributechangebatch/) class. |

### Methods
| Method | Description |
| :- | :- |
| [add](/search/python-net/groupdocs.search.common/attributechangebatch/add/#path-attributes) | Adds the specified attributes to the specified indexed document. |
| [add](/search/python-net/groupdocs.search.common/attributechangebatch/add/#paths-attributes) | Adds the specified attributes to the specified indexed documents. |
| [add_to_all](/search/python-net/groupdocs.search.common/attributechangebatch/add_to_all/#attributes) | Adds the specified attributes to all documents in the index. |
| [clear](/search/python-net/groupdocs.search.common/attributechangebatch/clear/) | Removes all attributes from all documents in the index. |
| [remove](/search/python-net/groupdocs.search.common/attributechangebatch/remove/#path-attributes) | Removes the specified attributes from the specified indexed document. |
| [remove](/search/python-net/groupdocs.search.common/attributechangebatch/remove/#paths-attributes) | Removes the specified attributes from the specified indexed documents. |
| [remove_all](/search/python-net/groupdocs.search.common/attributechangebatch/remove_all/#path) | Removes all attributes from the specified indexed document. |
| [remove_all](/search/python-net/groupdocs.search.common/attributechangebatch/remove_all/#paths) | Removes all attributes from the specified indexed documents. |
| [remove_from_all](/search/python-net/groupdocs.search.common/attributechangebatch/remove_from_all/#attributes) | Removes the specified attributes from all documents in the index. |

### Example

```python
import os
from groupdocs.search.common import AttributeChangeBatch

# Create a batch of attribute changes
batch = AttributeChangeBatch()
batch.add(os.path.abspath("./documents/relativity-lecture.pdf"), ["main"])
batch.add(os.path.abspath("./documents/einstein-biography.txt"), ["main", "biography"])

# Apply the changes to the index
index.change_attributes(batch)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
