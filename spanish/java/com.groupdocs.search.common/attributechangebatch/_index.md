---
title: "AttributeChangeBatch"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un contenedor para cambios de atributos."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Representa un contenedor para cambios de atributos.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Inicializa una nueva instancia de la  AttributeChangeBatch  clase. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Inicializa una nueva instancia de la  AttributeChangeBatch  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Agrega los atributos especificados al documento indexado especificado. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Agrega los atributos especificados a los documentos indexados especificados. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Agrega los atributos especificados a todos los documentos del índice. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Elimina los atributos especificados del documento indexado especificado. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Elimina los atributos especificados de los documentos indexados especificados. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Elimina todos los atributos del documento indexado especificado. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Elimina todos los atributos de los documentos indexados especificados. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Elimina los atributos especificados de todos los documentos del índice. |
|
|  | [clear()](#clear--) | Elimina todos los atributos de todos los documentos del índice. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Inicializa una nueva instancia de la  AttributeChangeBatch  clase.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Inicializa una nueva instancia de la  AttributeChangeBatch  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Agrega los atributos especificados al documento indexado especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta del documento. |
|
|  | atributos | java.lang.String[] | Los atributos a agregar. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Agrega los atributos especificados a los documentos indexados especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas de los documentos. |
|
|  | atributos | java.lang.String[] | Los atributos a agregar. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Agrega los atributos especificados a todos los documentos del índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | atributos | java.lang.String[] | Los atributos a agregar. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Elimina los atributos especificados del documento indexado especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta del documento. |
|
|  | atributos | java.lang.String[] | Los atributos a eliminar. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Elimina los atributos especificados de los documentos indexados especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas de los documentos. |
|
|  | atributos | java.lang.String[] | Los atributos a eliminar. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Elimina todos los atributos del documento indexado especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta del documento. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Elimina todos los atributos de los documentos indexados especificados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | paths | java.lang.String[] | Las rutas de los documentos. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Elimina los atributos especificados de todos los documentos del índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | atributos | java.lang.String[] | Los atributos a eliminar. |
|

### clear() {#clear--}
```
public void clear()
```


Elimina todos los atributos de todos los documentos del índice.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
