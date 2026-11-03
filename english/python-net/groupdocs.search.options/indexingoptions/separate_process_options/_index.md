---
title: separate_process_options property
second_title: GroupDocs.Search for Python via .NET API References
description: "The options for extracting data in a separate process."
type: docs
url: /python-net/groupdocs.search.options/indexingoptions/separate_process_options/
is_root: false
weight: 2030
---


## separate_process_options property

The options for extracting data in a separate process.

Provides a [`SeparateProcessOptions`](/search/python-net/groupdocs.search.options/separateprocessoptions/) object that configures extraction in a separate process. Use this property to enable extraction in a separate process, specify the launcher assembly path, set a timeout, and control whether the process is started with the `dotnet` command.

- `extract_in_separate_process` – Enables extraction in a separate process. The default value is `False`. In this mode data are extracted in only one thread; the `threads` option is ignored.
- `assembly_path` – Path to the extraction service assembly or launcher script.
- `timeout` – Maximum time to wait for the result of data extraction from one document. The default value is 10 minutes.
- `use_dotnet_to_start_process` – Determines whether the process is started with the `dotnet` command. The default value is `True`. Set to `False` to start an executable file directly; in this case `assembly_path` must point to the executable.

### Definition:
```python
@property
def separate_process_options(self):
    ...
```

### See Also
* class [`IndexingOptions`](/search/python-net/groupdocs.search.options/indexingoptions/)
