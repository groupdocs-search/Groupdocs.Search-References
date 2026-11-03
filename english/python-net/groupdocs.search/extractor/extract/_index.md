---
title: extract method
second_title: GroupDocs.Search for Python via .NET API References
description: "Extracts data from a document."
type: docs
url: /python-net/groupdocs.search/extractor/extract/
is_root: false
weight: 1010
---


## extract {#document-extraction_options}

Extracts data from a document.

```python
def extract(self, document, extraction_options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `Document` | The document from file system, stream or structure. |
| extraction_options | `ExtractionOptions` | The extraction options. |

**Returns:** The extracted data of the document.

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

### Aliases

These names call `extract` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `extract_document` | `extract_document(document, extraction_options)` |

### See Also
* class [`Extractor`](/search/python-net/groupdocs.search/extractor/)
