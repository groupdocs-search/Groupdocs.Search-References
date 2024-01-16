---
title: StructureOutputAdapter
second_title: GroupDocs.Search for Java API Reference
description: Represents an output adapter that collects output as a structure containing each field separately.
type: docs
weight: 33
url: /java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Represents an output adapter that collects output as a structure containing each field separately.
## Constructors

| Constructor | Description |
| --- | --- |
| [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initializes a new instance of the  StructureOutputAdapter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getResult()](#getResult--) | Gets the resulting array of fields. |
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Initializes a new instance of the  StructureOutputAdapter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | The output format. |

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Gets the resulting array of fields.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The resulting array of fields.
