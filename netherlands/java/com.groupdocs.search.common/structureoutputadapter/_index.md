---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een outputadapter voor die output verzamelt als een structuur die elk veld afzonderlijk bevat."
type: docs
weight: 33
url: /nl/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Stelt een outputadapter voor die output verzamelt als een structuur die elk veld afzonderlijk bevat.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialiseert een nieuw exemplaar van de StructureOutputAdapter-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getResult()](#getResult--) | Haalt de resulterende array van velden op. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Initialiseert een nieuw exemplaar van de StructureOutputAdapter-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Het uitvoerformaat. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Haalt de resulterende array van velden op.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De resulterende array van velden.

