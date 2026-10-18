---
title: "DateFormatCollection"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een verzameling van DateFormat-objecten voor."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Stelt een collectie van DateFormat-objecten voor.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Voegt een datumformaatobject toe aan de verzameling. |
|
|  | [clear()](#clear--) | Verwijdert alle elementen uit de verzameling. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Bepaalt of de verzameling een specifiek item bevat. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Kopieert de elementen van de verzameling naar een  Array , beginnend bij een bepaalde  Array  index. |
|
|  | [size()](#size--) | Haalt het aantal elementen op dat in de verzameling zit. |
|
|  | [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of de verzameling alleen-lezen is. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Verwijdert de eerste voorkoming van een specifiek element uit de collectie. |
|
|  | [iterator()](#iterator--) | Retourneert een enumerator die door de collectie iterereert. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Voegt een datumformaatobject toe aan de verzameling.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Het datumformaatobject om toe te voegen aan de collectie. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle elementen uit de verzameling.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Bepaalt of de verzameling een specifiek item bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Het item om te lokaliseren in de collectie. |
|

**Returns:**
boolean -  true  als het item wordt gevonden in de collectie; anders,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Kopieert de elementen van de verzameling naar een  Array , beginnend bij een bepaalde  Array  index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | De eendimensionale  Array  die de bestemming is van de elementen die uit de collectie zijn gekopieerd. |
|
|  | arrayIndex | int | De nulgebaseerde index in de array waarop het kopiëren begint. |
|

### size() {#size--}
```
public abstract int size()
```


Haalt het aantal elementen op dat in de verzameling zit.


**Returns:**
int - Het aantal elementen dat in de collectie zit.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Haalt een waarde op die aangeeft of de verzameling alleen-lezen is.


**Returns:**
boolean -  true  als de collectie alleen-lezen is; anders,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Verwijdert de eerste voorkoming van een specifiek element uit de collectie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Het item om te verwijderen uit de collectie. |
|

**Returns:**
boolean -  true  als het item succesvol is verwijderd uit de collectie; anders,  false . Deze methode retourneert ook  false  als het item niet wordt gevonden in de collectie.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Retourneert een enumerator die door de collectie iterereert.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Een enumerator die kan worden gebruikt om door de collectie te itereren.

