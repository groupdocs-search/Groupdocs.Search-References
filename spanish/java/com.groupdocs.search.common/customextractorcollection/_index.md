---
title: "CustomExtractorCollection"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Contiene una colección de extractores personalizados."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Contiene una colección de extractores personalizados. Si la colección contiene un extractor para alguna extensión de archivo que está cubierta por los extractores incorporados, entonces este extractor se usará en lugar del incorporado.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [size()](#size--) | Obtiene el número de extractores contenidos en la colección. |
|
|  | [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si la colección es de solo lectura. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador para esta colección. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Añade un extractor a la colección. |
|
|  | [clear()](#clear--) | Elimina todos los extractores de la colección. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Determina si la colección contiene un extractor específico. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Copia los elementos de la colección a un arreglo, comenzando en un índice de arreglo específico. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Elimina un extractor de la colección. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Obtiene el número de extractores contenidos en la colección.


**Returns:**
int - El número de extractores contenidos en la colección.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Obtiene un valor que indica si la colección es de solo lectura.


**Returns:**
boolean - Un valor que indica si la colección es de solo lectura.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Devuelve un iterador para esta colección.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Un objeto iterador que puede usarse para iterar a través de la colección.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Añade un extractor a la colección.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor a agregar a la colección. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todos los extractores de la colección.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Determina si la colección contiene un extractor específico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor a localizar en la colección. |
|

**Returns:**
boolean -  true  si  el elemento  se encuentra en la colección; de lo contrario,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Copia los elementos de la colección a un arreglo, comenzando en un índice de arreglo específico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | El arreglo unidimensional que es el destino de los elementos copiados de la colección. El arreglo debe tener indexación basada en cero. |
|
|  | arrayIndex | int | El índice basado en cero en la matriz donde comienza la copia. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Elimina un extractor de la colección.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor a eliminar de la colección. |
|

**Returns:**
boolean -  true  si  el extractor  se eliminó correctamente de la colección; de lo contrario,  false . Este método también devuelve  false  si  el extractor  no se encuentra en la colección original.

