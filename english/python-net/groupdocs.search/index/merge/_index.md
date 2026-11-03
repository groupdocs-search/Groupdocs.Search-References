---
title: merge method
second_title: GroupDocs.Search for Python via .NET API References
description: "Merges the specified index into the current index."
type: docs
url: /python-net/groupdocs.search/index/merge/
is_root: false
weight: 1160
---


## merge {#index-options}

Merges the specified index into the current index.

If the other index has a previous version, it must be updated before merging with [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/).

The indexes must divide the text of documents into terms in the same way; a search finds a document reliably only if the document was indexed with the dictionaries and settings that the index uses. The operation compares the current index with the other index if it contains documents: the settings [`IndexSettings.use_stop_words`](/search/python-net/groupdocs.search/indexsettings/use_stop_words/), [`IndexSettings.use_character_replacements`](/search/python-net/groupdocs.search/indexsettings/use_character_replacements/), [`IndexSettings.replace_unpaired_surrogates`](/search/python-net/groupdocs.search/indexsettings/replace_unpaired_surrogates/) and [`IndexSettings.skip_blended_only_terms`](/search/python-net/groupdocs.search/indexsettings/skip_blended_only_terms/), the alphabet, the tokenization dictionary, the stop word dictionary if the indexes use stop words, and the character replacement dictionary if the indexes use character replacements. If a difference is found, the operation throws a `RuntimeError` and no index is changed.

The alphabet, the tokenization dictionary, the stop word dictionary and the character replacement dictionary of the current index are not changed by the operation. The other dictionaries of the other index are merged into the dictionaries of the current index.

```python
def merge(self, index, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index | `Index` | The index to merge into. |
| options | `MergeOptions` | The merge options. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The other index contains documents and divides their text into terms differently from the current index. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import MergeOptions
from groupdocs.search.common import Cancellation

index1 = Index("./index1")
index1.add("./documents")

index2 = Index("./index2")
index2.add("./documents2")

options = MergeOptions()
options.cancellation = Cancellation()

try:
    index1.merge(index2, options)
except RuntimeError as exc:
    print(exc)

print("Documents in index1:", len(index1.get_indexed_documents()))
```

## merge {#repository-options}

Merges indexes from the specified index repository into the current index.

If other indexes have a previous version, they must be updated before merging with [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/).

The indexes have to divide the text of documents into terms in the same way: a search finds a document reliably only if the document was indexed with the dictionaries and settings that the index uses. The operation compares the current index with every index of the repository that contains documents: the settings [`IndexSettings.use_stop_words`](/search/python-net/groupdocs.search/indexsettings/use_stop_words/), [`IndexSettings.use_character_replacements`](/search/python-net/groupdocs.search/indexsettings/use_character_replacements/), [`IndexSettings.replace_unpaired_surrogates`](/search/python-net/groupdocs.search/indexsettings/replace_unpaired_surrogates/) and [`IndexSettings.skip_blended_only_terms`](/search/python-net/groupdocs.search/indexsettings/skip_blended_only_terms/), the alphabet, the tokenization dictionary, the stop word dictionary if the indexes use stop words, and the character replacement dictionary if the indexes use character replacements. If a difference is found, the operation throws a `RuntimeError` and no index is changed.

The alphabet, the tokenization dictionary, the stop word dictionary and the character replacement dictionary of the current index are not changed by the operation. The other dictionaries of the other indexes are merged into the dictionaries of the current index.

```python
def merge(self, repository, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| repository | `IndexRepository` | The index repository to merge into. |
| options | `MergeOptions` | The merge options. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | An index of the repository contains documents and divides their text into terms differently from the current index. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import MergeOptions
from groupdocs.search.common import Cancellation

index1 = Index("./index1")          # Creating index1
index1.add("./documents")           # Indexing documents

index2 = Index("./index2")          # Creating index2
index2.add("./documents2")          # Indexing documents

options = MergeOptions()
options.cancellation = Cancellation()  # Create cancellation object

try:
    # Merge index2 into index1; index2 files remain unchanged
    index1.merge(index2, options)
except RuntimeError as e:
    print(e)

print("Documents in index1:", len(index1.get_indexed_documents()))
```

### Aliases

These names call `merge` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `merge_index` | `merge_index(index, options)` |
| `merge_index_repository` | `merge_index_repository(repository, options)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
