---
title: "DocumentFilter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar basklassen för dokumentfilter."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Representerar basklassen för dokumentfilter. Innehåller metoder för att skapa instanser av dokumentfilter.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [toString()](#toString--) | Returnerar en strängrepresentation av ett dokumentfilter. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Skapar ett filter för att hoppa över dokument med skapelsedatum tidigare än den nedre gränsen. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Skapar ett filter för att hoppa över dokument med skapelsedatum senare än den övre gränsen. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Skapar ett filter för att hoppa över dokument med skapelsedatum utanför det angivna intervallet. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Skapar ett filter för att hoppa över dokument med ändringsdatum tidigare än den nedre gränsen. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Skapar ett filter för att hoppa över dokument med ändringsdatum senare än den övre gränsen. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Skapar ett filter för att hoppa över dokument med ändringsdatum utanför det angivna intervallet. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Skapar ett filter för att hoppa över dokument med längden mindre än den nedre gränsen. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Skapar ett filter för att hoppa över dokument med längden större än den övre gränsen. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Skapar ett filter för att hoppa över dokument utanför det angivna längdintervallet. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Skapar ett filter för att hoppa över dokument som inte har en tillåten filändelse. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Skapar ett filter som har omvänd logik i förhållande till det angivna inre filtret. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Skapar en logisk konjunktion av de angivna filtren. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Skapar en logisk disjunktion av de angivna filtren. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en strängrepresentation av ett dokumentfilter.


**Returns:**
java.lang.String - Strängrepresentation av ett dokumentfilter.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Skapar ett filter för att hoppa över dokument med skapelsedatum tidigare än den nedre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Den nedre gränsen för dokumentets skapandetid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Skapar ett filter för att hoppa över dokument med skapelsedatum senare än den övre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | upperBound | java.util.Date | Det övre gränsvärdet för dokumentets skapandetid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Skapar ett filter för att hoppa över dokument med skapelsedatum utanför det angivna intervallet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Den nedre gränsen för dokumentets skapandetid. |
|
|  | upperBound | java.util.Date | Det övre gränsvärdet för dokumentets skapandetid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Skapar ett filter för att hoppa över dokument med ändringsdatum tidigare än den nedre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Det nedre gränsvärdet för dokumentets ändringstid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Skapar ett filter för att hoppa över dokument med ändringsdatum senare än den övre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | upperBound | java.util.Date | Det övre gränsvärdet för dokumentets ändringstid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Skapar ett filter för att hoppa över dokument med ändringsdatum utanför det angivna intervallet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Det nedre gränsvärdet för dokumentets ändringstid. |
|
|  | upperBound | java.util.Date | Det övre gränsvärdet för dokumentets ändringstid. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på dokumentets fullständiga sökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Skapar ett filter för att hoppa över dokument som inte matchar ett reguljärt uttryck. Det reguljära uttrycket tillämpas på dokumentets fullständiga sökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pattern | java.lang.String | Det reguljära uttrycksmönstret. |
|
|  | options | int | Alternativen för det reguljära uttrycket. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Skapar ett filter för att hoppa över dokument med längden mindre än den nedre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | long | Det nedre gränsvärdet för dokumentets längd. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Skapar ett filter för att hoppa över dokument med längden större än den övre gränsen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | upperBound | long | Det övre gränsvärdet för dokumentets längd. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Skapar ett filter för att hoppa över dokument utanför det angivna längdintervallet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lowerBound | long | Det nedre gränsvärdet för dokumentets längd. |
|
|  | upperBound | long | Det övre gränsvärdet för dokumentets längd. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Skapar ett filter för att hoppa över dokument som inte har en tillåten filändelse.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filändelser | java.lang.String[] | Listan över tillåtna filändelser. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Skapar ett filter som har omvänd logik i förhållande till det angivna inre filtret.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Det inre dokumentfiltret. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Skapar en logisk konjunktion av de angivna filtren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Dokumentfiltren. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Skapar en logisk disjunktion av de angivna filtren.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Dokumentfiltren. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

