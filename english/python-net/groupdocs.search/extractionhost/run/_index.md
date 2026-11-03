---
title: run method
second_title: GroupDocs.Search for Python via .NET API References
description: "Starts the service for extracting data from documents."
type: docs
url: /python-net/groupdocs.search/extractionhost/run/
is_root: false
weight: 1020
---


## run

Starts the service for extracting data from documents.

Processes extraction requests until the main process stops the service. The license set in the main process is automatically passed to the extraction process, and the service forwards document password requests and extraction errors back to the main process. Custom text extractors must be added to the host's `custom_extractors` collection before invoking this method.

```python
def run(self):
    ...
```

### Example

```python
import sys
from groupdocs.search import ExtractionHost

# The index starts this script and passes the communication channel name.
with ExtractionHost(sys.argv[1:]) as host:
    # host.custom_extractors.add(MyExtractor())  # optional custom extractor
    host.run()
```

### See Also
* class [`ExtractionHost`](/search/python-net/groupdocs.search/extractionhost/)
