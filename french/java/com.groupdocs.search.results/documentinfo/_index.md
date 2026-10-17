---
title: "DocumentInfo"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un descripteur pour un document indexé."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Représente un descripteur pour un document indexé.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [toString()](#toString--) | Renvoie une  System.String  qui représente le  DocumentInfo  actuel. |
|
|  | [getFilePath()](#getFilePath--) | Obtient le chemin du fichier indexé à partir d'un fichier ou la clé du document indexé à partir d'un flux ou d'une structure. |
|
|  | [getFileType()](#getFileType--) | Obtient le type de fichier. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Obtient la famille de formats de document. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtient le chemin interne pour l'élément de document conteneur. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Obtient les parties du chemin interne pour l'élément de document conteneur. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Obtient le type de source du document. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Obtient l'indicateur d'erreur d'indexation. |
|
|  | [serialize()](#serialize--) | Sérialise l'instance actuelle en un tableau d'octets. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Désérialise une instance à partir d'un tableau d'octets. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Renvoie une  System.String  qui représente le  DocumentInfo  actuel.


**Returns:**
java.lang.String - Une  System.String  qui représente le  DocumentInfo  actuel.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Obtient le chemin du fichier indexé à partir d'un fichier ou la clé du document indexé à partir d'un flux ou d'une structure.


**Returns:**
java.lang.String - Le chemin du fichier ou la clé du document.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Obtient le type de fichier.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Obtient la famille de formats de document.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Obtient le chemin interne pour l'élément de document conteneur.


**Returns:**
java.lang.String - Le chemin interne.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Obtient les parties du chemin interne pour l'élément de document conteneur.


**Returns:**
java.lang.String[] - Les parties du chemin interne.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Obtient le type de source du document.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Obtient l'indicateur d'erreur d'indexation.


**Returns:**
boolean - L'indicateur d'erreur d'indexation.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Sérialise l'instance actuelle en un tableau d'octets.


**Returns:**
byte[] - Un tableau d'octets représentant l'instance actuelle.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Désérialise une instance à partir d'un tableau d'octets.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | tableau | byte[] | Un tableau d'octets à désérialiser. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

