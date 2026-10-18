---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar typerna av dokumentkällor."
type: docs
weight: 39
url: /sv/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Definierar typerna av dokumentkällor.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [File](#File) | Filens dokumentkälla. |
|
|  | [Stream](#Stream) | Strömmens dokumentkälla. |
|
|  | [Structure](#Structure) | Strukturens dokumentkälla. |
|
|  | [ExtractedData](#ExtractedData) | Dokumentkällan för tidigare extraherade data. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


Filens dokumentkälla.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


Strömmens dokumentkälla.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


Strukturens dokumentkälla.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


Dokumentkällan för tidigare extraherade data.


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
