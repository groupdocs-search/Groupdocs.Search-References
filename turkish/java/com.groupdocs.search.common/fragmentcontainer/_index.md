---
title: "FragmentContainer"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir belge alanının bulunan terimlerini vurgulayan metin parçacıkları için bir kapsayıcıyı temsil eder."
type: docs
weight: 22
url: /tr/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Bir belge alanının bulunan terimlerini vurgulayan metin parçacıkları için bir kapsayıcıyı temsil eder.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Belge alan adını alır. |
|
|  | [getCount()](#getCount--) | İçerilen metin parçacıklarının sayısını alır. |
|
|  | [getFragments()](#getFragments--) | İçerilen metin parçacıklarının bir dizisini alır. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Belge alan adını alır.


**Returns:**
java.lang.String - Belge alan adı.

### getCount() {#getCount--}
```
public abstract int getCount()
```


İçerilen metin parçacıklarının sayısını alır.


**Returns:**
int - İçerilen metin parçacıklarının sayısı.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


İçerilen metin parçacıklarının bir dizisini alır.


**Returns:**
java.lang.String[] - İçerilen metin parçacıklarının bir dizisi.

