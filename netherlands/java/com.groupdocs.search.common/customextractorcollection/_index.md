---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Bevat een verzameling van aangepaste extractors."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Bevat een collectie van aangepaste extractors. Als de collectie een extractor bevat voor een bestandsextensie die wordt gedekt door ingebouwde extractors, dan wordt deze extractor in plaats van de ingebouwde gebruikt.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [size()](#size--) | Haalt het aantal extractors op dat in de collectie zit. |
|
|  | [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of de verzameling alleen-lezen is. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator voor deze collectie. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Voegt een extractor toe aan de collectie. |
|
|  | [clear()](#clear--) | Verwijdert alle extractors uit de collectie. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Bepaalt of de collectie een specifieke extractor bevat. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Kopieert de elementen van de collectie naar een array, beginnend op een bepaalde array-index. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Verwijdert een extractor uit de collectie. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Haalt het aantal extractors op dat in de collectie zit.


**Returns:**
int - Het aantal extractors dat in de collectie zit.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Haalt een waarde op die aangeeft of de verzameling alleen-lezen is.


**Returns:**
boolean - Een waarde die aangeeft of de collectie alleen-lezen is.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Retourneert een iterator voor deze collectie.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Een iterator-object dat kan worden gebruikt om door de collectie te itereren.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Voegt een extractor toe aan de collectie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De extractor die aan de collectie moet worden toegevoegd. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle extractors uit de collectie.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Bepaalt of de collectie een specifieke extractor bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De extractor die in de collectie moet worden gevonden. |
|

**Returns:**
boolean -  true  als  item  in de collectie wordt gevonden; anders,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Kopieert de elementen van de collectie naar een array, beginnend op een bepaalde array-index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | De eendimensionale array die de bestemming is van de gekopieerde elementen uit de collectie. De array moet nulgebaseerde indexering hebben. |
|
|  | arrayIndex | int | De nulgebaseerde index in de array waarop het kopiëren begint. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Verwijdert een extractor uit de collectie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De extractor die uit de collectie moet worden verwijderd. |
|

**Returns:**
boolean -  true  als  extractor  succesvol uit de collectie is verwijderd; anders,  false . Deze methode geeft ook  false  terug als  extractor  niet wordt gevonden in de oorspronkelijke collectie.

