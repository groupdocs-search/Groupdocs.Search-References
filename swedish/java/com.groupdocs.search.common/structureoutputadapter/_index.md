---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en utdataadapter som samlar utdata som en struktur som innehåller varje fält separat."
type: docs
weight: 33
url: /sv/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Representerar en utdataadapter som samlar utdata som en struktur som innehåller varje fält separat.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initierar en ny instans av klassen StructureOutputAdapter. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getResult()](#getResult--) | Hämtar den resulterande arrayen av fält. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Initierar en ny instans av klassen StructureOutputAdapter.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Utdataformatet. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Hämtar den resulterande arrayen av fält.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Den resulterande arrayen av fält.

