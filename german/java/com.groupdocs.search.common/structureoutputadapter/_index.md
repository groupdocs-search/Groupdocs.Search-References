---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der die Ausgabe als Struktur sammelt, die jedes Feld separat enthält."
type: docs
weight: 33
url: /de/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Stellt einen Ausgabeadapter dar, der die Ausgabe als Struktur sammelt, die jedes Feld separat enthält.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialisiert eine neue Instanz der Klasse StructureOutputAdapter. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getResult()](#getResult--) | Liefert das resultierende Array von Feldern. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Initialisiert eine neue Instanz der Klasse StructureOutputAdapter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Das Ausgabeformat. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Liefert das resultierende Array von Feldern.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Das resultierende Array von Feldern.

