---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un conteneur pour les modifications d'attributs."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Représente un conteneur pour les modifications d'attributs.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Initialise une nouvelle instance de la classe AttributeChangeBatch. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Initialise une nouvelle instance de la classe AttributeChangeBatch. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Ajoute les attributs spécifiés au document indexé spécifié. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Ajoute les attributs spécifiés aux documents indexés spécifiés. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Ajoute les attributs spécifiés à tous les documents de l'index. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Supprime les attributs spécifiés du document indexé spécifié. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Supprime les attributs spécifiés des documents indexés spécifiés. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Supprime tous les attributs du document indexé spécifié. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Supprime tous les attributs des documents indexés spécifiés. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Supprime les attributs spécifiés de tous les documents de l'index. |
|
|  | [clear()](#clear--) | Supprime tous les attributs de tous les documents de l'index. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Initialise une nouvelle instance de la classe AttributeChangeBatch.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Initialise une nouvelle instance de la classe AttributeChangeBatch.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Ajoute les attributs spécifiés au document indexé spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin du document. |
|
|  | attributs | java.lang.String[] | Les attributs à ajouter. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Ajoute les attributs spécifiés aux documents indexés spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins des documents. |
|
|  | attributs | java.lang.String[] | Les attributs à ajouter. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Ajoute les attributs spécifiés à tous les documents de l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | attributs | java.lang.String[] | Les attributs à ajouter. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Supprime les attributs spécifiés du document indexé spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin du document. |
|
|  | attributs | java.lang.String[] | Les attributs à supprimer. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Supprime les attributs spécifiés des documents indexés spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins des documents. |
|
|  | attributs | java.lang.String[] | Les attributs à supprimer. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Supprime tous les attributs du document indexé spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemin | java.lang.String | Le chemin du document. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Supprime tous les attributs des documents indexés spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | chemins | java.lang.String[] | Les chemins des documents. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Supprime les attributs spécifiés de tous les documents de l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | attributs | java.lang.String[] | Les attributs à supprimer. |
|

### clear() {#clear--}
```
public void clear()
```


Supprime tous les attributs de tous les documents de l'index.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
