---
title: "AliasDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de alias."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Define la interfaz de un diccionario de alias.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de alias contenidos en el  AliasDictionary . |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Agrega la colección especificada de pares alias/reemplazo a esta instancia del  AliasDictionary . |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Agrega la colección especificada de pares alias/reemplazo a esta instancia del  AliasDictionary . |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Agrega el par especificado de alias y texto asociado a esta instancia del  AliasDictionary . |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Elimina el alias especificado de un objeto  AliasDictionary  . |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Determina si un objeto  AliasDictionary  contiene el alias especificado. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Obtiene un texto que está asociado con el alias especificado. |
|
|  | [clear()](#clear--) | Elimina todos los alias de un objeto  AliasDictionary  . |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de alias contenidos en el  AliasDictionary .


**Returns:**
int - El número de alias contenidos en el  AliasDictionary .

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Agrega la colección especificada de pares alias/reemplazo a esta instancia del  AliasDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pares | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | La colección de pares alias/reemplazo para agregar al diccionario. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Agrega la colección especificada de pares alias/reemplazo a esta instancia del  AliasDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | La colección de pares alias/reemplazo para agregar al diccionario. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Agrega el par especificado de alias y texto asociado a esta instancia del  AliasDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | alias | java.lang.String | El alias para agregar al diccionario. |
|
|  | texto | java.lang.String | El texto que se asociará con el alias. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Elimina el alias especificado de un objeto  AliasDictionary  .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | alias | java.lang.String | El alias a eliminar. |
|

**Returns:**
boolean - Este método devuelve  true  si el alias se encuentra y elimina correctamente. Este método devuelve  false  si el alias no se encuentra en el  AliasDictionary  objeto.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Determina si un objeto  AliasDictionary  contiene el alias especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | alias | java.lang.String | El alias a localizar en el  AliasDictionary  objeto. |
|

**Returns:**
boolean -  true  si el objeto  AliasDictionary  contiene el alias especificado; de lo contrario,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Obtiene un texto que está asociado con el alias especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | alias | java.lang.String | El alias a localizar en el  AliasDictionary  objeto. |
|

**Returns:**
java.lang.String - Un texto asociado con el alias especificado o  null .

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todos los alias de un objeto  AliasDictionary  .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.String> - Un iterador que puede usarse para iterar a través de la colección.

