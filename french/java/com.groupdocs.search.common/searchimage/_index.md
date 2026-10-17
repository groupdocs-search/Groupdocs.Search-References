---
title: "SearchImage"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une image à rechercher."
type: docs
weight: 29
url: /fr/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Représente une image à rechercher.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Crée une image à partir d'un fichier pour la recherche. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Crée une image à partir d'un fichier pour la recherche. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Crée une image à partir d'un flux pour la recherche. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Crée une image à partir d'un flux pour la recherche. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Crée une image à partir d'un fichier pour la recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier image. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Crée une image à partir d'un fichier pour la recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier image. |
|
|  | imageIndex | int | L'index de l'image dans les images multipages. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Crée une image à partir d'un flux pour la recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Le flux d'image. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Crée une image à partir d'un flux pour la recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Le flux d'image. |
|
|  | imageIndex | int | L'index de l'image dans les images multipages. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

