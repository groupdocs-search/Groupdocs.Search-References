---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento che si verifica quando un documento protetto da password è indicizzato."
type: docs
weight: 20
url: /it/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento che si verifica quando un documento protetto da password è indicizzato.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Restituisce il percorso completo del documento. |
|
|  | [getPassword()](#getPassword--) | Restituisce la password per aprire il documento. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Imposta la password per aprire il documento. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Restituisce il percorso completo del documento.


**Returns:**
java.lang.String - Il percorso completo del documento.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Restituisce la password per aprire il documento.


**Returns:**
java.lang.String - La password per aprire il documento.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Imposta la password per aprire il documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | La password per aprire il documento. |
|

