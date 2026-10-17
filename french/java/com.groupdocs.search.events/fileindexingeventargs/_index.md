---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de démarrage de l'indexation d'un document."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement de démarrage de l'indexation d'un document.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocument()](#getDocument--) | Obtient le document. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Obtient le chemin complet du document. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtient la clé du document. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Obtient une valeur indiquant que l'indexation du document doit être ignorée. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Définit une valeur indiquant que l'indexation du document doit être ignorée. |
|
|  | [getEncoding()](#getEncoding--) | Obtient l'encodage du document. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Définit l'encodage du document. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtient l'extracteur de texte personnalisé. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Définit l'extracteur de texte personnalisé. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtient les champs supplémentaires du document. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Définit les champs supplémentaires du document. |
|
|  | [getAttributes()](#getAttributes--) | Obtient les attributs du document. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Définit les attributs du document. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Obtient le document.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Obtient le chemin complet du document.


**Returns:**
java.lang.String - Le chemin complet du document.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtient la clé du document.


**Returns:**
java.lang.String - La clé du document.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Obtient une valeur indiquant que l'indexation du document doit être ignorée.


**Returns:**
boolean - Une valeur indiquant que l'indexation du document doit être ignorée.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Définit une valeur indiquant que l'indexation du document doit être ignorée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant que l'indexation du document doit être ignorée. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Obtient l'encodage du document.


**Returns:**
java.lang.String - L'encodage du document.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Définit l'encodage du document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | L'encodage du document. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Obtient l'extracteur de texte personnalisé.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Définit l'extracteur de texte personnalisé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur de texte personnalisé. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Obtient les champs supplémentaires du document.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Les champs supplémentaires du document.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Définit les champs supplémentaires du document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Les champs supplémentaires pour le document. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Obtient les attributs du document.


**Returns:**
java.lang.String[] - Les attributs du document.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Définit les attributs du document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String[] | Les attributs du document. |
|

