---
title: get_result method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns an array of resulting fragment containers."
type: docs
url: /python-net/groupdocs.search.highlighters/fragmenthighlighter/get_result/
is_root: false
weight: 1010
---


## get_result

Returns an array of resulting fragment containers.

```python
def get_result(self):
    ...
```

**Returns:** list: A list of fragment containers.

### Example

```python
    from groupdocs.search.highlighters import FragmentHighlighter
    from groupdocs.search.options import OutputFormat

    fh = FragmentHighlighter(OutputFormat.HTML)
    index.highlight(found, fh)
    for container in fh.get_result():
        print(container.field_name, container.count)
    ```

### See Also
* class [`FragmentHighlighter`](/search/python-net/groupdocs.search.highlighters/fragmenthighlighter/)
