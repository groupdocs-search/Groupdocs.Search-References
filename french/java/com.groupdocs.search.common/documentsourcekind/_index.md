---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit les types de sources de documents."
type: docs
weight: 39
url: /fr/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Définit les types de sources de documents.

## Fields

| Field | Description |
| --- | --- |
|  | [File](#File) | La source de document fichier. |
|
|  | [Stream](#Stream) | La source de document flux. |
|
|  | [Structure](#Structure) | La source de document structure. |
|
|  | [ExtractedData](#ExtractedData) | La source de document des données précédemment extraites. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


La source de document fichier.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


La source de document flux.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


La source de document structure.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


La source de document des données précédemment extraites.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
