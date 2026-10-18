---
title: "PasswordDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge şifreleri sözlüğünün arabirimini tanımlar."
type: docs
weight: 20
url: /tr/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Belge şifreleri sözlüğünün arabirimini tanımlar.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Sözlükte bulunan öğelerin sayısını alır. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Dosyanın şifresini alır. |
|
|  | [clear()](#clear--) | Bu  PasswordDictionary  nesnesinden tüm şifreleri kaldırır. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Sözlüğün belirtilen belge için bir şifre içerip içermediğini belirler. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Bir belge için şifreyi sözlüğe ekler. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Belirtilen belgenin şifresini sözlükten kaldırır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Sözlükte bulunan öğelerin sayısını alır.


**Returns:**
int - Sözlükte bulunan öğelerin sayısı.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Dosyanın şifresini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosya yolu. |
|

**Returns:**
java.lang.String - Dosyanın şifresi.

### clear() {#clear--}
```
public abstract void clear()
```


Bu  PasswordDictionary  nesnesinden tüm şifreleri kaldırır.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Sözlüğün belirtilen belge için bir şifre içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Belgenin dosya yolu. |
|

**Returns:**
boolean -  true  sözlüğün belge için bir şifre içeriyorsa; aksi takdirde,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Bir belge için şifreyi sözlüğe ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Belgenin dosya yolu. |
|
|  | password | java.lang.String | Belge şifresi. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Belirtilen belgenin şifresini sözlükten kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Belgenin dosya yolu. |
|

**Returns:**
boolean -  true  şifre başarıyla kaldırıldıysa; aksi takdirde,  false . Bu yöntem ayrıca  filePath  sözlükte bulunamazsa  false  döndürür.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.String> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

