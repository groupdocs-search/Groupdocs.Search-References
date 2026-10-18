---
title: "FoundDocument"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulunan bir belgeyi temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Bulunan bir belgeyi temsil eder.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Belge bilgilerini alır. |
|
|  | [getRelevance()](#getRelevance--) | Arama sonucunun alaka düzeyini alır. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Bulunan oluşum sayısını alır. |
|
|  | [getFoundFields()](#getFoundFields--) | Bulunan belge alanlarını alır. |
|
|  | [getTerms()](#getTerms--) | Bulunan terimleri alır. |
|
|  | [getTermSequences()](#getTermSequences--) | Bulunan terim dizilerini alır. |
|
|  | [getAttributes()](#getAttributes--) | Bulunan belgeyle ilişkili öznitelikleri alır. |
|
|  | [toString()](#toString--) | Bulunan belgenin dize temsili döndürür. |
|
|  | [serialize()](#serialize--) | Geçerli örneği bir bayt dizisine serileştirir. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Bir örneği bayt dizisinden seriden çıkarır. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Belge bilgilerini alır.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Arama sonucunun alaka düzeyini alır.


**Returns:**
double - Arama sonucunun alaka düzeyi.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Bulunan oluşum sayısını alır.


**Returns:**
int - Bulunan oluşum sayısı.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Bulunan belge alanlarını alır.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Bulunan belge alanları.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Bulunan terimleri alır. Değer, özelliğe her erişildiğinde değerlendirilir.


**Returns:**
java.lang.String[] - Bulunan terimler.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Bulunan terim dizilerini alır.


**Returns:**
java.lang.String[][] - Bulunan terim dizileri.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Bulunan belgeyle ilişkili öznitelikleri alır. Öznitelikleri almak için ilgili seçeneğin arama seçeneklerinde etkinleştirilmiş olması gerekir.


**Returns:**
java.lang.String[] - Bulunan belgeyle ilişkili öznitelikler.

### toString() {#toString--}
```
public abstract String toString()
```


Bulunan belgenin dize temsili döndürür.


**Returns:**
java.lang.String - Bulunan belgeyi temsil eden bir dize.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Geçerli örneği bir bayt dizisine serileştirir.


**Returns:**
byte[] - Geçerli örneği temsil eden bir bayt dizisi.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Bir örneği bayt dizisinden seriden çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dizi | byte[] | Serileştirilecek bir bayt dizisi. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

