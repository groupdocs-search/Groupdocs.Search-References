---
title: "PasswordRequiredEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento que ocurre cuando se indexa un documento protegido con contraseña."
type: docs
weight: 20
url: /es/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento que ocurre cuando se indexa un documento protegido con contraseña.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Obtiene la ruta completa del documento. |
|
|  | [getPassword()](#getPassword--) | Obtiene la contraseña para abrir el documento. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Establece la contraseña para abrir el documento. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Obtiene la ruta completa del documento.


**Returns:**
java.lang.String - La ruta completa del documento.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtiene la contraseña para abrir el documento.


**Returns:**
java.lang.String - La contraseña para abrir el documento.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Establece la contraseña para abrir el documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | La contraseña para abrir el documento. |
|

