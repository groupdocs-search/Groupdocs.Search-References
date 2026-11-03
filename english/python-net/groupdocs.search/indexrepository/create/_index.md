---
title: create method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a new index in memory."
type: docs
url: /python-net/groupdocs.search/indexrepository/create/
is_root: false
weight: 1020
---


## create

Creates a new index in memory.

```python
def create(self):
    ...
```

**Returns:** Index: The created index.

### Example

```python
    from groupdocs.search import IndexRepository

    index_repository = IndexRepository()
    index = index_repository.create()
    ```

## create {#settings}

Creates a new index in memory.

```python
def create(self, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| settings | `IndexSettings` | The index settings. |

**Returns:** The created index.

### Example

```python
from groupdocs.search import IndexRepository, IndexSettings

index_repository = IndexRepository()
settings = IndexSettings()
settings.use_stop_words = False  # Disable stop words during indexing

index = index_repository.create(settings)
```

## create {#index_folder}

Creates a new index on disk, cleaning the index folder before creation.

```python
def create(self, index_folder):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder. |

**Returns:** Index: The created index.

### Example

```python
from groupdocs.search import IndexRepository

index_folder = "./MyIndex"
index_repository = IndexRepository()
index = index_repository.create(index_folder)
```

## create {#index_folder-settings}

Creates a new index on disk. The index folder will be cleaned before the index creation.

```python
def create(self, index_folder, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder. |
| settings | `IndexSettings` | The index settings. |

**Returns:** Index: The created index.

### Example

```python
from groupdocs.search import IndexRepository, IndexSettings

index_folder = "./MyIndex"
settings = IndexSettings()
settings.use_stop_words = False  # Disable stop words during indexing

index_repository = IndexRepository()
index = index_repository.create(index_folder, settings)
```

### Aliases

These names call `create` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_file` | `create_file(index_folder, settings)`<br>`create_file(index_folder)` |
| `create_string` | `create_string(index_folder, settings)`<br>`create_string(index_folder)` |
| `create_index_settings` | `create_index_settings(settings)` |

### See Also
* class [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/)
