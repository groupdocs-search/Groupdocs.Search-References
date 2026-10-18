---
title: "DateFormatCollection"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en samling av DateFormat-objekt."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Representerar en samling av DateFormat-objekt.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Lägger till ett DateFormat-objekt i samlingen. |
|
|  | [clear()](#clear--) | Tar bort alla element från samlingen. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Bestämmer om samlingen innehåller ett specifikt objekt. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Kopierar elementen i samlingen till en  Array , med start vid ett specifikt  Array  index. |
|
|  | [size()](#size--) | Hämtar antalet element som finns i samlingen. |
|
|  | [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om samlingen är skrivskyddad. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Tar bort den första förekomsten av ett specifikt element från samlingen. |
|
|  | [iterator()](#iterator--) | Returnerar en enumerator som itererar genom samlingen. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Lägger till ett DateFormat-objekt i samlingen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Datumformatobjektet att lägga till i samlingen. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla element från samlingen.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Bestämmer om samlingen innehåller ett specifikt objekt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Objektet att hitta i samlingen. |
|

**Returns:**
boolean -  true  om objektet hittas i samlingen; annars,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Kopierar elementen i samlingen till en  Array , med start vid ett specifikt  Array  index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Den endimensionella  Array  som är destinationen för elementen som kopierats från samlingen. |
|
|  | arrayIndex | int | Det nollbaserade indexet i arrayen där kopieringen börjar. |
|

### size() {#size--}
```
public abstract int size()
```


Hämtar antalet element som finns i samlingen.


**Returns:**
int - Antalet element som finns i samlingen.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Hämtar ett värde som indikerar om samlingen är skrivskyddad.


**Returns:**
boolean -  true  om samlingen är skrivskyddad; annars,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Tar bort den första förekomsten av ett specifikt element från samlingen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Objektet att ta bort från samlingen. |
|

**Returns:**
boolean -  true  om objektet framgångsrikt togs bort från samlingen; annars,  false . Denna metod returnerar också  false  om objektet inte hittas i samlingen.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Returnerar en enumerator som itererar genom samlingen.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - En enumerator som kan användas för att iterera genom samlingen.

