---
title: "DateFormatCollection"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt eine Sammlung von DateFormat-Objekten dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Stellt eine Sammlung von DateFormat‑Objekten dar.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Fügt der Sammlung ein DateFormat-Objekt hinzu. |
|
|  | [clear()](#clear--) | Entfernt alle Elemente aus der Sammlung. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Bestimmt, ob die Sammlung ein bestimmtes Element enthält. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Kopiert die Elemente der Sammlung in ein Array, beginnend bei einem bestimmten Array-Index. |
|
|  | [size()](#size--) | Gibt die Anzahl der in der Sammlung enthaltenen Elemente zurück. |
|
|  | [isReadOnly()](#isReadOnly--) | Gibt einen Wert zurück, der angibt, ob die Sammlung schreibgeschützt ist. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Entfernt das erste Vorkommen eines bestimmten Elements aus der Sammlung. |
|
|  | [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Fügt der Sammlung ein DateFormat-Objekt hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Das Datumsformat-Objekt, das zur Sammlung hinzugefügt werden soll. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Elemente aus der Sammlung.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Bestimmt, ob die Sammlung ein bestimmtes Element enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Das Element, das in der Sammlung gefunden werden soll. |
|

**Returns:**
boolean - true, wenn das Element in der Sammlung gefunden wird; andernfalls false.

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Kopiert die Elemente der Sammlung in ein Array, beginnend bei einem bestimmten Array-Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Das eindimensionale Array, das das Ziel der aus der Sammlung kopierten Elemente ist. |
|
|  | arrayIndex | int | Der nullbasierte Index im Array, an dem das Kopieren beginnt. |
|

### size() {#size--}
```
public abstract int size()
```


Gibt die Anzahl der in der Sammlung enthaltenen Elemente zurück.


**Returns:**
int - Die Anzahl der im Sammlung enthaltenen Elemente.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Gibt einen Wert zurück, der angibt, ob die Sammlung schreibgeschützt ist.


**Returns:**
boolean - true, wenn die Sammlung schreibgeschützt ist; andernfalls false.

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Entfernt das erste Vorkommen eines bestimmten Elements aus der Sammlung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Das Element, das aus der Sammlung entfernt werden soll. |
|

**Returns:**
boolean - true, wenn das Element erfolgreich aus der Sammlung entfernt wurde; andernfalls false. Diese Methode gibt ebenfalls false zurück, wenn das Element in der Sammlung nicht gefunden wird.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Gibt einen Enumerator zurück, der die Sammlung durchläuft.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Ein Enumerator, der verwendet werden kann, um die Sammlung zu durchlaufen.

