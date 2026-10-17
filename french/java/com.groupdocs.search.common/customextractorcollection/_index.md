---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Contient une collection d'extracteurs personnalisés."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Contient une collection d'extracteurs personnalisés. Si la collection contient un extracteur pour une extension de fichier qui est déjà prise en charge par les extracteurs intégrés, alors cet extracteur sera utilisé à la place de celui intégré.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [size()](#size--) | Obtient le nombre d'extracteurs contenus dans la collection. |
|
|  | [isReadOnly()](#isReadOnly--) | Obtient une valeur indiquant si la collection est en lecture seule. |
|
|  | [iterator()](#iterator--) | Renvoie un itérateur pour cette collection. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Ajoute un extracteur à la collection. |
|
|  | [clear()](#clear--) | Supprime tous les extracteurs de la collection. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Détermine si la collection contient un extracteur spécifique. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Copie les éléments de la collection dans un tableau, en commençant à un indice de tableau particulier. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Supprime un extracteur de la collection. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Obtient le nombre d'extracteurs contenus dans la collection.


**Returns:**
int - Le nombre d'extracteurs contenus dans la collection.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Obtient une valeur indiquant si la collection est en lecture seule.


**Returns:**
boolean - Une valeur indiquant si la collection est en lecture seule.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Renvoie un itérateur pour cette collection.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Un objet itérateur qui peut être utilisé pour parcourir la collection.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Ajoute un extracteur à la collection.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur à ajouter à la collection. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les extracteurs de la collection.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Détermine si la collection contient un extracteur spécifique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur à localiser dans la collection. |
|

**Returns:**
boolean -  true  si  item  est trouvé dans la collection ; sinon,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Copie les éléments de la collection dans un tableau, en commençant à un indice de tableau particulier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Le tableau unidimensionnel qui est la destination des éléments copiés depuis la collection. Le tableau doit être indexé à partir de zéro. |
|
|  | arrayIndex | int | L'index basé sur zéro dans le tableau où la copie commence. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Supprime un extracteur de la collection.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur à supprimer de la collection. |
|

**Returns:**
boolean -  true  si  extractor  a été supprimé avec succès de la collection ; sinon,  false . Cette méthode renvoie également  false  si  extractor  n'est pas trouvé dans la collection originale.

