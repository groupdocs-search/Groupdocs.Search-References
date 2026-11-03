---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new in-memory Index instance."
type: docs
url: /python-net/groupdocs.search/index/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new in-memory [`Index`](/search/python-net/groupdocs.search/index/) instance.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.search import Index

index = Index()
```

## __init__ {#settings}

Initializes a new Index instance in memory with the specified index settings.

```python
def __init__(self, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| settings | `IndexSettings` | The index settings object. |

### Example

```python
from groupdocs.search import Index, IndexSettings
from groupdocs.search.options import IndexType

settings = IndexSettings()
settings.index_type = IndexType.COMPACT_INDEX
index = Index(settings)
```

## __init__ {#index_folder}

Initializes a new Index, creating a new or opening an existing index on disk.

```python
def __init__(self, index_folder):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |

### Example

```python
from groupdocs.search import Index

# Create or open an index located at "./index"
index = Index("./index")
```

## __init__ {#index_folder-settings}

Initializes a new Index with the specified folder and settings.

```python
def __init__(self, index_folder, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |
| settings | `IndexSettings` | The index settings object. |

### Example

```python
from groupdocs.search import Index, IndexSettings
from groupdocs.search.options import IndexType

settings = IndexSettings()
settings.index_type = IndexType.COMPACT_INDEX
index = Index("./MyIndex", settings)
```

## __init__ {#index_folder-overwrite_if_exists}

Initializes a new Index instance.

Loads an existing index from disk if `overwrite_if_exists` is False; otherwise creates a new index on disk.

```python
def __init__(self, index_folder, overwrite_if_exists):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |
| overwrite_if_exists | `bool` | The flag of overwriting the index folder. |

### Example

```python
from groupdocs.search import Index

# Create a new index, overwriting any existing index in the folder
index = Index("./MyIndex", overwrite_if_exists=True)
```

## __init__ {#index_folder-settings-overwrite_if_exists}

Initializes a new [`Index`](/search/python-net/groupdocs.search/index/) instance. Loads an existing index from disk if `overwrite_if_exists` is `False`; otherwise creates a new index on disk with the specified index settings.

```python
def __init__(self, index_folder, settings, overwrite_if_exists):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |
| settings | `IndexSettings` | The index settings object. |
| overwrite_if_exists | `bool` | Flag indicating whether to overwrite the index folder. |

### Example

```python
from groupdocs.search import Index, IndexSettings
from groupdocs.search.options import IndexType

index_folder = "./MyIndex"
settings = IndexSettings()
settings.index_type = IndexType.COMPACT_INDEX
index = Index(index_folder, settings, overwrite_if_exists=True)
```

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
