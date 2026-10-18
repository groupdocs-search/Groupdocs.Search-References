---
title: "DocumentFilter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Basisklasse für Dokumentfilter dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Stellt die Basisklasse für Dokumentfilter dar. Enthält Methoden zur Erstellung von Dokumentfilter-Instanzen.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [toString()](#toString--) | Gibt die String-Darstellung eines Dokumentfilters zurück. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum vor der unteren Grenze. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum nach der oberen Grenze. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum außerhalb des angegebenen Bereichs. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum vor der unteren Grenze. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum nach der oberen Grenze. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum außerhalb des angegebenen Bereichs. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge kleiner als die untere Grenze. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge größer als die obere Grenze. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Erstellt einen Filter zum Überspringen von Dokumenten außerhalb des angegebenen Dokumentlängenbereichs. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Erstellt einen Filter zum Überspringen von Dokumenten, die keine zulässige Erweiterung haben. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Erstellt eine logische Konjunktion der angegebenen Filter. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Erstellt eine logische Disjunktion der angegebenen Filter. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Gibt die String-Darstellung eines Dokumentfilters zurück.


**Returns:**
java.lang.String – String-Darstellung eines Dokumentfilters.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum vor der unteren Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Die untere Grenze der Dokumenterstellungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum nach der oberen Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | upperBound | java.util.Date | Die obere Grenze der Dokumenterstellungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Erstellungsdatum außerhalb des angegebenen Bereichs.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Die untere Grenze der Dokumenterstellungszeit. |
|
|  | upperBound | java.util.Date | Die obere Grenze der Dokumenterstellungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum vor der unteren Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Die untere Grenze der Dokumentenänderungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum nach der oberen Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | upperBound | java.util.Date | Die obere Grenze der Dokumentenänderungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit Änderungsdatum außerhalb des angegebenen Bereichs.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Die untere Grenze der Dokumentenänderungszeit. |
|
|  | upperBound | java.util.Date | Die obere Grenze der Dokumentenänderungszeit. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das Muster des regulären Ausdrucks. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Erstellt einen Filter, um Dokumente zu überspringen, die nicht einem regulären Ausdruck entsprechen. Der reguläre Ausdruck wird auf den vollständigen Pfad eines Dokuments angewendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pattern | java.lang.String | Das Muster des regulären Ausdrucks. |
|
|  | options | int | Die Optionen des regulären Ausdrucks. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge kleiner als die untere Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | long | Die untere Grenze der Dokumentlänge. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten mit einer Länge größer als die obere Grenze.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | upperBound | long | Die obere Grenze der Dokumentlänge. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Erstellt einen Filter zum Überspringen von Dokumenten außerhalb des angegebenen Dokumentlängenbereichs.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lowerBound | long | Die untere Grenze der Dokumentlänge. |
|
|  | upperBound | long | Die obere Grenze der Dokumentlänge. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Erstellt einen Filter zum Überspringen von Dokumenten, die keine zulässige Erweiterung haben.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Die Liste zulässiger Erweiterungen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Erstellt einen Filter, der eine inverse Logik in Bezug auf den angegebenen inneren Filter hat.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Der innere Dokumentfilter. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Erstellt eine logische Konjunktion der angegebenen Filter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Die Dokumentfilter. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Erstellt eine logische Disjunktion der angegebenen Filter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Die Dokumentfilter. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

