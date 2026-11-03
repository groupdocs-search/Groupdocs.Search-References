---
title: Extractor class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a tool for preliminary data extraction from documents for separating the stage of subsequent fast indexing."
type: docs
url: /python-net/groupdocs.search/extractor/
is_root: false
weight: 20
---


## Extractor class

Represents a tool for preliminary data extraction from documents for separating the stage of subsequent fast indexing.

The Extractor type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search/extractor/__init__/) | Initializes a new instance of the Extractor class. |

### Methods
| Method | Description |
| :- | :- |
| [extract](/search/python-net/groupdocs.search/extractor/extract/#document-extraction_options) | Extracts data from a document. |

### Properties
| Property | Description |
| :- | :- |
| [settings](/search/python-net/groupdocs.search/extractor/settings/) | The extractor settings. |

### Events
| Event | Description |
| :- | :- |
| [error_occurred](/search/python-net/groupdocs.search/extractor/error_occurred/) | Occurs when an error happens during an extractor operation. |
| [image_preparing](/search/python-net/groupdocs.search/extractor/image_preparing/) | Occurs when an image is going to be prepared for indexing. |
| [password_required](/search/python-net/groupdocs.search/extractor/password_required/) | Occurs when a document requires password for opening. |

### Example

```python
from groupdocs.search import Extractor
from groupdocs.search.common import Document
from groupdocs.search.options import ExtractionOptions

extractor = Extractor()
extractor.error_occurred += lambda sender, args: print(args.message)

document = Document.create_from_file("./documents/lecture.txt")

extraction_options = ExtractionOptions()
extraction_options.use_raw_text_extraction = False

extracted_data = extractor.extract(document, extraction_options)
```

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
