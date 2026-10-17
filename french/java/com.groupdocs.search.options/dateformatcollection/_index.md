---
title: "DateFormatCollection"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une collection d'objets DateFormat."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Représente une collection d'objets DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Ajoute un objet de format de date à la collection. |
|
|  | [clear()](#clear--) | Supprime tous les éléments de la collection. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Détermine si la collection contient un élément spécifique. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Copie les éléments de la collection dans un  Array , en commençant à un indice particulier du  Array . |
|
|  | [size()](#size--) | Obtient le nombre d'éléments contenus dans la collection. |
|
|  | [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si la collection est en lecture seule. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Supprime la première occurrence d'un élément spécifique de la collection. |
|
|  | [iterator()](#iterator--) | Renvoie un itérateur qui parcourt la collection. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Ajoute un objet de format de date à la collection.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'objet de format de date à ajouter à la collection. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les éléments de la collection.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Détermine si la collection contient un élément spécifique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'élément à localiser dans la collection. |
|

**Returns:**
boolean -  true  si l'élément est trouvé dans la collection ; sinon,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Copie les éléments de la collection dans un  Array , en commençant à un indice particulier du  Array .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Le tableau unidimensionnel  Array  qui est la destination des éléments copiés depuis la collection. |
|
|  | arrayIndex | int | L'index basé sur zéro dans le tableau où la copie commence. |
|

### size() {#size--}
```
public abstract int size()
```


Obtient le nombre d'éléments contenus dans la collection.


**Returns:**
int - Le nombre d'éléments contenus dans la collection.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Obtient une valeur indiquant si la collection est en lecture seule.


**Returns:**
boolean -  true  si la collection est en lecture seule ; sinon,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Supprime la première occurrence d'un élément spécifique de la collection.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'élément à supprimer de la collection. |
|

**Returns:**
boolean -  true  si l'élément a été supprimé avec succès de la collection ; sinon,  false . Cette méthode renvoie également  false  si l'élément n'est pas trouvé dans la collection.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Renvoie un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Un itérateur qui peut être utilisé pour parcourir la collection.

