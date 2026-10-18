---
title: "DocumentSourceKind"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define los tipos de fuentes de documentos."
type: docs
weight: 39
url: /es/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Define los tipos de fuentes de documentos.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [File](#File) | La fuente de documento de archivo. |
|
|  | [Stream](#Stream) | La fuente de documento de flujo. |
|
|  | [Structure](#Structure) | La fuente de documento estructurado. |
|
|  | [ExtractedData](#ExtractedData) | La fuente de documento de datos extraídos previamente. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


La fuente de documento de archivo.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


La fuente de documento de flujo.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


La fuente de documento estructurado.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


La fuente de documento de datos extraídos previamente.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
