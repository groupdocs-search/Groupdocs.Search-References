---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Özellik değişiklikleri için bir kapsayıcıyı temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Özellik değişiklikleri için bir kapsayıcıyı temsil eder.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | AttributeChangeBatch sınıfının yeni bir örneğini başlatır. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | AttributeChangeBatch sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Belirtilen nitelikleri belirtilen indekslenmiş belgeye ekler. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Belirtilen nitelikleri belirtilen indekslenmiş belgelere ekler. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Belirtilen nitelikleri indeksdeki tüm belgelere ekler. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Belirtilen nitelikleri belirtilen indekslenmiş belgeden kaldırır. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Belirtilen nitelikleri belirtilen indekslenmiş belgelere kaldırır. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Belirtilen indekslenmiş belgeden tüm nitelikleri kaldırır. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Belirtilen indekslenmiş belgelerden tüm öznitelikleri kaldırır. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | İndeksteki tüm belgelerden belirtilen öznitelikleri kaldırır. |
|
|  | [clear()](#clear--) | İndeksteki tüm belgelerden tüm öznitelikleri kaldırır. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


AttributeChangeBatch sınıfının yeni bir örneğini başlatır.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


AttributeChangeBatch sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Belirtilen nitelikleri belirtilen indekslenmiş belgeye ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Belge yolu. |
|
|  | attributes | java.lang.String[] | Eklenecek öznitelikler. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Belirtilen nitelikleri belirtilen indekslenmiş belgelere ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | Belge yolları. |
|
|  | attributes | java.lang.String[] | Eklenecek öznitelikler. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Belirtilen nitelikleri indeksdeki tüm belgelere ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | attributes | java.lang.String[] | Eklenecek öznitelikler. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Belirtilen nitelikleri belirtilen indekslenmiş belgeden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Belge yolu. |
|
|  | attributes | java.lang.String[] | Kaldırılacak öznitelikler. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Belirtilen nitelikleri belirtilen indekslenmiş belgelere kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | Belge yolları. |
|
|  | attributes | java.lang.String[] | Kaldırılacak öznitelikler. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Belirtilen indekslenmiş belgeden tüm nitelikleri kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | path | java.lang.String | Belge yolu. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Belirtilen indekslenmiş belgelerden tüm öznitelikleri kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | yollar | java.lang.String[] | Belge yolları. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


İndeksteki tüm belgelerden belirtilen öznitelikleri kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | attributes | java.lang.String[] | Kaldırılacak öznitelikler. |
|

### clear() {#clear--}
```
public void clear()
```


İndeksteki tüm belgelerden tüm öznitelikleri kaldırır.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
