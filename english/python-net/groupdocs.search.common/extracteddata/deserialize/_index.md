---
title: deserialize method
second_title: GroupDocs.Search for Python via .NET API References
description: "Deserializes an instance from a byte array."
type: docs
url: /python-net/groupdocs.search.common/extracteddata/deserialize/
is_root: false
weight: 1010
---


## deserialize {#array}

Deserializes an instance from a byte array.

```python
def deserialize(cls, array):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| array | `list[int]` | A byte array to deserialize from. |

**Returns:** An instance deserialized from a byte array.

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
* class [`ExtractedData`](/search/python-net/groupdocs.search.common/extracteddata/)
