---
title: "PasswordDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de contraseñas de documentos."
type: docs
weight: 20
url: /es/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Define la interfaz de un diccionario de contraseñas de documentos.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de elementos contenidos en el diccionario. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Obtiene la contraseña del archivo. |
|
|  | [clear()](#clear--) | Elimina todas las contraseñas de este  PasswordDictionary  objeto. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Determina si el diccionario contiene una contraseña para el documento especificado. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Agrega una contraseña para un documento al diccionario. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Elimina una contraseña del documento especificado del diccionario. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de elementos contenidos en el diccionario.


**Returns:**
int - El número de elementos contenidos en el diccionario.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Obtiene la contraseña del archivo.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo. |
|

**Returns:**
java.lang.String - La contraseña del archivo.

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todas las contraseñas de este  PasswordDictionary  objeto.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Determina si el diccionario contiene una contraseña para el documento especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo del documento. |
|

**Returns:**
boolean -  true  si el diccionario contiene una contraseña para el documento; de lo contrario,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Agrega una contraseña para un documento al diccionario.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo del documento. |
|
|  | contraseña | java.lang.String | La contraseña del documento. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Elimina una contraseña del documento especificado del diccionario.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo del documento. |
|

**Returns:**
boolean -  true  si la contraseña se eliminó correctamente; de lo contrario,  false . Este método también devuelve  false  si  filePath  no se encontró en el diccionario.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.String> - Un iterador que puede usarse para iterar a través de la colección.

