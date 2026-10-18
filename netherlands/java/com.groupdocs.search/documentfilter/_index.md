---
title: "DocumentFilter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de basisklasse voor documentfilters voor."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Vertegenwoordigt de basisklasse voor documentfilters. Bevat methoden voor het maken van documentfilterinstanties.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van een documentfilter. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Maakt een filter om documenten over te slaan met een creatiedatum eerder dan de ondergrens. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Maakt een filter om documenten over te slaan met een creatiedatum later dan de bovengrens. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Maakt een filter om documenten over te slaan met een creatiedatum buiten het opgegeven bereik. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Maakt een filter om documenten over te slaan met een wijzigingsdatum eerder dan de ondergrens. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Maakt een filter om documenten over te slaan met een wijzigingsdatum later dan de bovengrens. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Maakt een filter om documenten over te slaan met een wijzigingsdatum buiten het opgegeven bereik. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Maakt een filter om documenten over te slaan met een lengte kleiner dan de ondergrens. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Maakt een filter om documenten over te slaan met een lengte groter dan de bovengrens. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Maakt een filter om documenten over te slaan buiten het opgegeven documentlengtebereik. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Maakt een filter om documenten over te slaan die geen toegestane extensie hebben. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Maakt een filter dat een omgekeerde logica heeft ten opzichte van het opgegeven interne filter. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Maakt een logische conjunctie van de opgegeven filters. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Maakt een logische disjunctie van de opgegeven filters. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Retourneert de tekenreeksrepresentatie van een documentfilter.


**Returns:**
java.lang.String - Tekenreeksrepresentatie van een documentfilter.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Maakt een filter om documenten over te slaan met een creatiedatum eerder dan de ondergrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | java.util.Date | De ondergrens van de creatietijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Maakt een filter om documenten over te slaan met een creatiedatum later dan de bovengrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | upperBound | java.util.Date | De bovengrens van de creatietijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Maakt een filter om documenten over te slaan met een creatiedatum buiten het opgegeven bereik.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | java.util.Date | De ondergrens van de creatietijd van het document. |
|
|  | upperBound | java.util.Date | De bovengrens van de creatietijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Maakt een filter om documenten over te slaan met een wijzigingsdatum eerder dan de ondergrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | java.util.Date | De ondergrens van de wijzigingstijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Maakt een filter om documenten over te slaan met een wijzigingsdatum later dan de bovengrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | upperBound | java.util.Date | De bovengrens van de wijzigingstijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Maakt een filter om documenten over te slaan met een wijzigingsdatum buiten het opgegeven bereik.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | java.util.Date | De ondergrens van de wijzigingstijd van het document. |
|
|  | upperBound | java.util.Date | De bovengrens van de wijzigingstijd van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. De reguliere expressie wordt toegepast op het volledige pad van een document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het patroon van de reguliere expressie. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Maakt een filter om documenten over te slaan die niet overeenkomen met een reguliere expressie. De reguliere expressie wordt toegepast op het volledige pad van een document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pattern | java.lang.String | Het patroon van de reguliere expressie. |
|
|  | options | int | De opties van de reguliere expressie. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Maakt een filter om documenten over te slaan met een lengte kleiner dan de ondergrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | long | De ondergrens van de lengte van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Maakt een filter om documenten over te slaan met een lengte groter dan de bovengrens.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | upperBound | long | De bovengrens van de lengte van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Maakt een filter om documenten over te slaan buiten het opgegeven documentlengtebereik.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lowerBound | long | De ondergrens van de lengte van het document. |
|
|  | upperBound | long | De bovengrens van de lengte van het document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Maakt een filter om documenten over te slaan die geen toegestane extensie hebben.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | extensions | java.lang.String[] | De lijst met toegestane extensies. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Maakt een filter dat een omgekeerde logica heeft ten opzichte van het opgegeven interne filter.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | De interne documentfilter. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Maakt een logische conjunctie van de opgegeven filters.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | De documentfilters. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Maakt een logische disjunctie van de opgegeven filters.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | De documentfilters. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

