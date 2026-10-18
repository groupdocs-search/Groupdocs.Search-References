---
title: "DocumentFilter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge filtreleri için temel sınıfı temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Belge filtreleri için temel sınıfı temsil eder. Belge filtresi örnekleri oluşturmak için yöntemler içerir.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [toString()](#toString--) | Bir belge filtresinin dize temsilini döndürür. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Alt sınırdan daha erken oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Üst sınırdan daha geç oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Belirtilen aralık dışında oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Alt sınırdan daha erken değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Üst sınırdan daha geç değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Belirtilen aralık dışında değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Alt sınırdan daha kısa uzunluğa sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Üst sınırdan daha uzun uzunluğa sahip belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Belirtilen belge uzunluğu aralığı dışında kalan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | İzin verilen uzantıya sahip olmayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Belirtilen iç filtreyle ilişkili ters mantığa sahip bir filtre oluşturur. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Belirtilen filtrelerin mantıksal birleşimini oluşturur. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Belirtilen filtrelerin mantıksal ayrımını oluşturur. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Bir belge filtresinin dize temsilini döndürür.


**Returns:**
java.lang.String - Bir belge filtresinin dize temsili.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Alt sınırdan daha erken oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Belge oluşturma zamanının alt sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Üst sınırdan daha geç oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | upperBound | java.util.Date | Belge oluşturma zamanının üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Belirtilen aralık dışında oluşturulma tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Belge oluşturma zamanının alt sınırı. |
|
|  | upperBound | java.util.Date | Belge oluşturma zamanının üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Alt sınırdan daha erken değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Belge değiştirme zamanının alt sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Üst sınırdan daha geç değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | upperBound | java.util.Date | Belge değiştirme zamanının üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Belirtilen aralık dışında değiştirilme tarihine sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Belge değiştirme zamanının alt sınırı. |
|
|  | upperBound | java.util.Date | Belge değiştirme zamanının üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. Düzenli ifade, bir belgenin tam yoluna uygulanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Düzenli ifade deseni. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. Düzenli ifade, bir belgenin tam yoluna uygulanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Düzenli ifade deseni. |
|
|  | options | int | Düzenli ifade seçenekleri. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Alt sınırdan daha kısa uzunluğa sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | uzun | Belge uzunluğunun alt sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Üst sınırdan daha uzun uzunluğa sahip belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | upperBound | uzun | Belge uzunluğunun üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Belirtilen belge uzunluğu aralığı dışında kalan belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lowerBound | uzun | Belge uzunluğunun alt sınırı. |
|
|  | upperBound | uzun | Belge uzunluğunun üst sınırı. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


İzin verilen uzantıya sahip olmayan belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | extensions | java.lang.String[] | İzin verilen uzantıların listesi. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Belirtilen iç filtreyle ilişkili ters mantığa sahip bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | İç belge filtresi. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Belirtilen filtrelerin mantıksal birleşimini oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Belge filtreleri. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Belirtilen filtrelerin mantıksal ayrımını oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Belge filtreleri. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

