---
title: extract method
second_title: GroupDocs.Search for Python via .NET API References
description: "Extracts data from documents."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/extract/
is_root: false
weight: 1050
---


## extract {#documents-passwords-options}

Extracts data from documents.

The extract method of the [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/) class only extracts data from documents using the extraction services of the network, without indexing. The data extracted from each document are passed to the `data_extracted` event, and the completion of the operation is reported by the `extraction_completed` event.

```python
def extract(self, documents, passwords, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| documents | `List[Document]` | The documents to be extracted. |
| passwords | `List[str]` | The document passwords. |
| options | `IndexingOptions` | The extraction options. |

### Example

```python
import threading

from groupdocs.search.options import IndexingOptions

# `node` is the master node of a configured and started search network;
# `documents` and `passwords` are the lists Indexer.add takes
extracted_data = []
lock = threading.Lock()


def on_data_extracted(sender, args):
    with lock:  # raised on engine worker threads
        extracted_data.append(args.data)


node.events.data_extracted += on_data_extracted
node.events.extraction_completed += lambda sender, args: print("Extraction completed")

node.indexer.extract(documents, passwords, IndexingOptions())
```

### Aliases

These names call `extract` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `extract_ilist` | `extract_ilist(documents, passwords, options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
