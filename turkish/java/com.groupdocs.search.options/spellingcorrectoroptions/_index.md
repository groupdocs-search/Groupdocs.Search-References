---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Yazım düzelticisi için seçenekler sağlar."
type: docs
weight: 36
url: /tr/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Yazım düzelticisi için seçenekler sağlar.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Yazım düzelticisinin etkin olup olmadığını gösteren bir değeri alır. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Yazım düzelticisinin etkin olup olmadığını gösteren bir değeri ayarlar. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Maksimum hata sayısını alır. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Maksimum hata sayısını ayarlar. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri alır. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri ayarlar. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Bulunan minimum hata sayısının üstündeki maksimum aşımı alır. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Bulunan minimum hata sayısının üstündeki maksimum aşımı ayarlar. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Algoritmanın iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değeri alır. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Algoritmanın iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değeri ayarlar. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Yazım düzelticisinin etkin olup olmadığını gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - Yazım düzelticisinin etkin olup olmadığını gösteren bir değer.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Yazım düzelticisinin etkin olup olmadığını gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Yazım düzelticisinin etkin olup olmadığını gösteren bir değer. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Maksimum hata sayısını alır. Varsayılan değer 2.


**Returns:**
int - Maksimum hata sayısı.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Maksimum hata sayısını ayarlar. Varsayılan değer 2.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Maksimum hata sayısı. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri alır. Varsayılan değer false.


**Returns:**
boolean - true if only the best results will be returned; otherwise false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Yalnızca en iyi sonuçların döndürüleceğini gösteren bir değeri ayarlar. Varsayılan değer false.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | yalnızca en iyi sonuçların döndürüleceği durumda true; aksi takdirde false. |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Bulunan en az hata sayısının maksimum aşımını alır. Varsayılan değer 0'dır.


**Returns:**
byte - Bulunan en az hata sayısının maksimum aşımı.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Bulunan en az hata sayısının maksimum aşımını ayarlar. Varsayılan değer 0'dır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | byte | Bulunan en az hata sayısının maksimum aşımı. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Algoritmanın iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değer alır. Varsayılan değer true'dur.


**Returns:**
boolean - transpozisyonları dikkate alıyorsa true; aksi takdirde false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Algoritmanın iki yan yana karakterin yer değiştirmesini tek bir hata olarak değerlendirmesi gerekip gerekmediğini gösteren bir değer ayarlar. Varsayılan değer true'dur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | transpozisyonları dikkate alıyorsa true; aksi takdirde false. |
|

