---
title: "PasswordDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en ordbok med dokumentlösenord."
type: docs
weight: 20
url: /sv/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Definierar gränssnittet för en ordbok med dokumentlösenord.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet element som finns i ordboken. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Hämtar lösenordet för filen. |
|
|  | [clear()](#clear--) | Tar bort alla lösenord från detta  PasswordDictionary  -objekt. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Avgör om ordboken innehåller ett lösenord för det angivna dokumentet. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Lägger till ett lösenord för ett dokument i ordboken. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Tar bort ett lösenord för det angivna dokumentet från ordboken. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet element som finns i ordboken.


**Returns:**
int - Antalet element som finns i ordboken.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Hämtar lösenordet för filen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Filens sökväg. |
|

**Returns:**
java.lang.String - Lösenordet för filen.

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla lösenord från detta  PasswordDictionary  -objekt.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Avgör om ordboken innehåller ett lösenord för det angivna dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Dokumentets filsökväg. |
|

**Returns:**
boolean -  true  om ordboken innehåller ett lösenord för dokumentet; annars  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Lägger till ett lösenord för ett dokument i ordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Dokumentets filsökväg. |
|
|  | lösenord | java.lang.String | Dokumentets lösenord. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Tar bort ett lösenord för det angivna dokumentet från ordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Dokumentets filsökväg. |
|

**Returns:**
boolean -  true  om lösenordet togs bort framgångsrikt; annars  false . Denna metod returnerar också  false  om  filePath  inte hittades i ordboken.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.String> - En iterator som kan användas för att iterera genom samlingen.

