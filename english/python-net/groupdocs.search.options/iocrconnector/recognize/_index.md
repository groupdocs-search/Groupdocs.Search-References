---
title: recognize method
second_title: GroupDocs.Search for Python via .NET API References
description: "Performs OCR processing on an image."
type: docs
url: /python-net/groupdocs.search.options/iocrconnector/recognize/
is_root: false
weight: 1010
---


## recognize {#context}

Performs OCR processing on an image.

```python
def recognize(self, context):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| context | `OcrContext` | The OCR processing context. |

**Returns:** The recognized text.

### Example

```python
import io

from groupdocs.search.options import IndexingOptions

try:
    import pytesseract  # pip install pytesseract
    from PIL import Image  # pip install pillow
except ImportError:
    pytesseract = None


class TesseractOcrConnector(object):
    def recognize(self, context):
        image = context.image_stream.read()  # Read the whole image stream
        if pytesseract is None:
            print("pytesseract is not installed: an image of %d bytes is not recognized" % len(image))
            return None
        with Image.open(io.BytesIO(image)) as picture:
            return pytesseract.image_to_string(picture)


options = IndexingOptions()
options.ocr_indexing_options.enabled_for_separate_images = True
options.ocr_indexing_options.ocr_connector = TesseractOcrConnector()
```

### Aliases

These names call `recognize` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `recognize_ocr_context` | `recognize_ocr_context(context)` |

### See Also
* class [`IOcrConnector`](/search/python-net/groupdocs.search.options/iocrconnector/)
