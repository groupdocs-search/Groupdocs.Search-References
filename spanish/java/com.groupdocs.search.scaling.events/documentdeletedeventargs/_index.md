---
title: "DocumentDeletedEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de finalización de la eliminación de un documento."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

Representa los argumentos del evento de finalización de la eliminación de un documento.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Obtiene el índice del fragmento. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtiene la clave del documento. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Obtiene el índice del fragmento.


**Returns:**
int - El índice del fragmento.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtiene la clave del documento.


**Returns:**
java.lang.String - La clave del documento.

