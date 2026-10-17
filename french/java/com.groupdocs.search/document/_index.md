---
title: "Document"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente la classe de base pour les documents ajoutés à un index à partir d'un flux du système de fichiers ou d'une structure."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Représente la classe de base pour les documents ajoutés à un index à partir du système de fichiers, d'un flux ou d'une structure. Contient des méthodes statiques pour créer des documents à partir de différents types de sources.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Obtient le type de source du document. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtient la clé du document utilisée pour identifier le document dans un index. |
|
|  | [isLazy()](#isLazy--) | Obtient une valeur indiquant si le document est chargé à la demande ou non. |
|
|  | [getModificationDate()](#getModificationDate--) | Obtient la date de dernière modification du document. |
|
|  | [getExtension()](#getExtension--) | Obtient l'extension utilisée pour ce type de document. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtient les champs supplémentaires du document. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Définit les champs supplémentaires du document. |
|
|  | [getAttributes()](#getAttributes--) | Obtient les attributs du document. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Définit les attributs du document. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Crée un document à partir d'un fichier. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Crée un document à partir d'un flux. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Crée un document à partir d'une structure qui est un tableau de champs texte. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Crée un document chargé paresseusement. |
|
|  | [toString()](#toString--) | Renvoie un  java.lang.String  qui représente le  Document  actuel. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Obtient le type de source du document.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Obtient la clé du document utilisée pour identifier le document dans un index.


**Returns:**
java.lang.String - La clé du document utilisée pour identifier le document dans un index.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Obtient une valeur indiquant si le document est chargé à la demande ou non.


**Returns:**
boolean - Une valeur indiquant si le document est chargé à la demande ou non.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Obtient la date de dernière modification du document.


**Returns:**
java.util.Date - La date de dernière modification du document.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Obtient l'extension utilisée pour ce type de document.


**Returns:**
java.lang.String - L'extension utilisée pour ce type de document.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Obtient les champs supplémentaires du document.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Les champs supplémentaires du document.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Définit les champs supplémentaires du document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Les champs supplémentaires pour le document. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Obtient les attributs du document.


**Returns:**
java.lang.String[] - Les attributs du document.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Définit les attributs du document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String[] | Les attributs du document. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Crée un document à partir d'un fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier du document. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Crée un document à partir d'un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clé du document. |
|
|  | modificationDate | java.util.Date | La date de modification du document. |
|
|  | extension | java.lang.String | L'extension du document. |
|
|  | stream | java.io.InputStream | Le flux du document. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Crée un document à partir d'une structure qui est un tableau de champs texte.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clé du document. |
|
|  | modificationDate | java.util.Date | La date de modification du document. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Les champs du document. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Crée un document chargé paresseusement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Le type de source du document. Cette valeur doit correspondre au type du document chargé. |
|
|  | documentKey | java.lang.String | La clé du document. Cette valeur doit correspondre à la clé du document chargé. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Le chargeur de document. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Renvoie un  java.lang.String  qui représente le  Document  actuel.


**Returns:**
java.lang.String - Un  java.lang.String  qui représente le  Document actuel .

