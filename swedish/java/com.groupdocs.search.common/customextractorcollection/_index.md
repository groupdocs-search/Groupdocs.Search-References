---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search för Java API-referens"
description: "Innehåller en samling av anpassade extraherare."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Innehåller en samling av anpassade extraheringsverktyg. Om samlingen innehåller en extraherare för någon filändelse som täcks av inbyggda extraherare, kommer denna extraherare att användas istället för den inbyggda.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [size()](#size--) | Hämtar antalet extraherare som finns i samlingen. |
|
|  | [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om samlingen är skrivskyddad. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator för denna samling. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Lägger till en extraherare i samlingen. |
|
|  | [clear()](#clear--) | Tar bort alla extraherare från samlingen. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Avgör om samlingen innehåller en specifik extraktor. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Kopierar elementen i samlingen till en array, med start vid ett specifikt array-index. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Tar bort en extraktor från samlingen. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Hämtar antalet extraherare som finns i samlingen.


**Returns:**
int - Antalet extraktorer som finns i samlingen.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Hämtar ett värde som indikerar om samlingen är skrivskyddad.


**Returns:**
boolean - Ett värde som indikerar om samlingen är skrivskyddad.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Returnerar en iterator för denna samling.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Ett iterator-objekt som kan användas för att iterera genom samlingen.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Lägger till en extraherare i samlingen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Extraktorn att lägga till i samlingen. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla extraherare från samlingen.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Avgör om samlingen innehåller en specifik extraktor.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Extraktorn att söka efter i samlingen. |
|

**Returns:**
boolean -  true  om  objektet  hittas i samlingen; annars,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Kopierar elementen i samlingen till en array, med start vid ett specifikt array-index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Den endimensionella arrayen som är destinationen för elementen som kopierats från samlingen. Arrayen måste ha nollbaserad indexering. |
|
|  | arrayIndex | int | Det nollbaserade indexet i arrayen där kopieringen börjar. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Tar bort en extraktor från samlingen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Extraktorn att ta bort från samlingen. |
|

**Returns:**
boolean -  true  om  extraktorn  framgångsrikt togs bort från samlingen; annars,  false . Denna metod returnerar också  false  om  extraktorn  inte finns i den ursprungliga samlingen.

