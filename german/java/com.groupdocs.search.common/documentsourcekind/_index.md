---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Arten von Dokumentquellen."
type: docs
weight: 39
url: /de/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Definiert die Arten von Dokumentquellen.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [File](#File) | Die Dateidokumentquelle. |
|
|  | [Stream](#Stream) | Die Stream-Dokumentquelle. |
|
|  | [Structure](#Structure) | Die Struktur-Dokumentquelle. |
|
|  | [ExtractedData](#ExtractedData) | Die Dokumentquelle zuvor extrahierter Daten. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


Die Dateidokumentquelle.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


Die Stream-Dokumentquelle.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


Die Struktur-Dokumentquelle.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


Die Dokumentquelle zuvor extrahierter Daten.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
