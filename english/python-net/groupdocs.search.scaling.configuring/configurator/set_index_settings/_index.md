---
title: set_index_settings method
second_title: GroupDocs.Search for Python via .NET API References
description: "Starts configuring the index settings for each shard in the search network."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configurator/set_index_settings/
is_root: false
weight: 1040
---


## set_index_settings

Starts configuring the index settings for each shard in the search network.

```python
def set_index_settings(self):
    ...
```

**Returns:** IndexSettingsConfigurator: The index settings configurator.

### Example

```python
    from groupdocs.search.scaling.configuring import Configurator

    configurator = Configurator()
    index_settings = configurator.set_index_settings()
    index_settings.set_use_stop_words(True)
    ```

### See Also
* class [`Configurator`](/search/python-net/groupdocs.search.scaling.configuring/configurator/)
