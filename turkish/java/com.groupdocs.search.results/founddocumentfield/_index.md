---
title: "FoundDocumentField"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulunan bir belge alanını temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Bulunan bir belge alanını temsil eder.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Alan adını alır. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Bulunan oluşum sayısını alır. |
|
|  | [getTerms()](#getTerms--) | Bulunan terimleri alır. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Bulunan terimlerin oluşumlarını alır. |
|
|  | [getTermSequences()](#getTermSequences--) | Bulunan terim dizilerini alır. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Bulunan terim dizilerinin oluşumlarını alır. |
|
|  | [toString()](#toString--) | Bulunan belge alanının dize temsili döndürür. |
|
|  | [serialize()](#serialize--) | Geçerli örneği bir bayt dizisine serileştirir. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Bir örneği bayt dizisinden seriden çıkarır. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Alan adını alır.


**Returns:**
java.lang.String - Alan adı.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Bulunan oluşum sayısını alır.


**Returns:**
int - Bulunan oluşum sayısı.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Bulunan terimleri alır.


**Returns:**
java.lang.String[] - Bulunan terimler.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Bulunan terimlerin oluşumlarını alır.


**Returns:**
int[] - Bulunan terimlerin oluşumları.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Bulunan terim dizilerini alır.


**Returns:**
java.lang.String[][] - Bulunan terim dizileri.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Bulunan terim dizilerinin oluşumlarını alır.


**Returns:**
int[] - Bulunan terim dizilerinin oluşumları.

### toString() {#toString--}
```
public abstract String toString()
```


Bulunan belge alanının dize temsili döndürür.


**Returns:**
java.lang.String - Bulunan belge alanını temsil eden bir dize.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Geçerli örneği bir bayt dizisine serileştirir.


**Returns:**
byte[] - Geçerli örneği temsil eden bir bayt dizisi.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Bir örneği bayt dizisinden seriden çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dizi | byte[] | Serileştirilecek bir bayt dizisi. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

