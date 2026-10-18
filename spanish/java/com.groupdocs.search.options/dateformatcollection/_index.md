---
title: "DateFormatCollection"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una colección de objetos DateFormat."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Representa una colección de objetos DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Agrega un objeto de formato de fecha a la colección. |
|
|  | [clear()](#clear--) | Elimina todos los elementos de la colección. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Determina si la colección contiene un elemento específico. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Copia los elementos de la colección a un  Array , comenzando en un índice particular del  Array . |
|
|  | [size()](#size--) | Obtiene el número de elementos contenidos en la colección. |
|
|  | [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si la colección es de solo lectura. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Elimina la primera aparición de un elemento específico de la colección. |
|
|  | [iterator()](#iterator--) | Devuelve un enumerador que recorre la colección. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Agrega un objeto de formato de fecha a la colección.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | El objeto de formato de fecha que se añadirá a la colección. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todos los elementos de la colección.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Determina si la colección contiene un elemento específico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | El elemento a localizar en la colección. |
|

**Returns:**
boolean -  true  si el elemento se encuentra en la colección; de lo contrario,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Copia los elementos de la colección a un  Array , comenzando en un índice particular del  Array .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | El unidimensional  Array  que es el destino de los elementos copiados de la colección. |
|
|  | arrayIndex | int | El índice basado en cero en la matriz donde comienza la copia. |
|

### size() {#size--}
```
public abstract int size()
```


Obtiene el número de elementos contenidos en la colección.


**Returns:**
int - El número de elementos contenidos en la colección.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Obtiene un valor que indica si la colección es de solo lectura.


**Returns:**
boolean -  true  si la colección es de solo lectura; de lo contrario,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Elimina la primera aparición de un elemento específico de la colección.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | El elemento a eliminar de la colección. |
|

**Returns:**
boolean -  true  si el elemento se eliminó correctamente de la colección; de lo contrario,  false . Este método también devuelve  false  si el elemento no se encuentra en la colección.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Devuelve un enumerador que recorre la colección.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Un enumerador que puede usarse para recorrer la colección.

