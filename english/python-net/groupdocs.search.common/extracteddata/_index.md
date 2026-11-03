---
title: ExtractedData class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents data retrieved from a document and prepared for indexing."
type: docs
url: /python-net/groupdocs.search.common/extracteddata/
is_root: false
weight: 110
---


## ExtractedData class

Represents data retrieved from a document and prepared for indexing.

The ExtractedData type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [deserialize](/search/python-net/groupdocs.search.common/extracteddata/deserialize/#array) | Deserializes an instance from a byte array. |
| [serialize](/search/python-net/groupdocs.search.common/extracteddata/serialize/) | Serializes the current instance to a byte array. |

### Properties
| Property | Description |
| :- | :- |
| [is_extraction_successful](/search/python-net/groupdocs.search.common/extracteddata/is_extraction_successful/) | The property indicates whether the data extraction process completed successfully. |

### Example

```python
from groupdocs.search import Extractor
from groupdocs.search.common import Document, ExtractedData
from groupdocs.search.options import ExtractionOptions

extractor = Extractor()
extractor.error_occurred += lambda sender, args: print(args.message)

document = Document.create_from_file("./documents/lecture.txt")

extraction_options = ExtractionOptions()
extraction_options.use_raw_text_extraction = False

extracted_data = extractor.extract(document, extraction_options)

# Serialized data can be stored or sent, then read back
array = extracted_data.serialize()
deserialized_data = ExtractedData.deserialize(array)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
