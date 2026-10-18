---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för indexering av metadatafält."
type: docs
weight: 29
url: /sv/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Tillhandahåller alternativ för indexering av metadatafält.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Hämtar ett värde som indikerar om tomma fältvärden ska indexeras eller inte. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Ställer in ett värde som indikerar om tomma fältvärden ska indexeras eller inte. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Hämtar ett värde som indikerar om tomma fältnamn ska indexeras eller inte. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Ställer in ett värde som indikerar om tomma fältnamn ska indexeras eller inte. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Hämtar standardfältnamnet som används för att indexera tomma fältnamn. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Ställer in standardfältnamnet som används för att indexera tomma fältnamn. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Hämtar avgränsaren i det sammansatta namnet på ett fält. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Ställer in avgränsaren i det sammansatta namnet på ett fält. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Hämtar det maximala antalet värden i en array av typen byte för att indexera fältet. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Ställer in det maximala antalet värden i en array av typen byte för att indexera fältet. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Hämtar det maximala antalet värden i en array av typen int för att indexera fältet. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Ställer in det maximala antalet värden i en array av typen int för att indexera fältet. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Hämtar det maximala antalet värden i en array av typen long för att indexera fältet. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Ställer in det maximala antalet värden i en array av typen long för att indexera fältet. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Hämtar det maximala antalet värden i en array av typen double för att indexera fältet. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Ställer in det maximala antalet värden i en array av typen double för att indexera fältet. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Hämtar avgränsaren mellan värden i ett fält av typen array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Ställer in avgränsaren mellan värden i ett fält av typen array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Hämtar ett värde som indikerar om tomma fältvärden ska indexeras eller inte. Standardvärdet är  true .


**Returns:**
boolean - Ett värde som indikerar om tomma fältvärden ska indexeras eller inte.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Ställer in ett värde som indikerar om tomma fältvärden ska indexeras eller inte. Standardvärdet är  true .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om tomma fältvärden ska indexeras eller inte. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Hämtar ett värde som indikerar om tomma fältnamn ska indexeras eller inte. Standardvärdet är  true .


**Returns:**
boolean - Ett värde som indikerar om tomma fältnamn ska indexeras eller inte.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Ställer in ett värde som indikerar om tomma fältnamn ska indexeras eller inte. Standardvärdet är  true .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om tomma fältnamn ska indexeras eller inte. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Hämtar standardfältnamnet som används för att indexera tomma fältnamn. Standardvärdet är  \"unknown\" .


**Returns:**
java.lang.String - Standardfältnamnet som används för att indexera tomma fältnamn.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Ställer in standardfältnamnet som används för att indexera tomma fältnamn. Standardvärdet är  \"unknown\" .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Standardfältnamnet som används för att indexera tomma fältnamn. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Hämtar separatorn i det sammansatta namnet på ett fält. Standardvärdet är  \".\" .


**Returns:**
java.lang.String - Separatorn i det sammansatta namnet på ett fält.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Ställer in separatorn i det sammansatta namnet på ett fält. Standardvärdet är  \".\" .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Separatorn i det sammansatta namnet på ett fält. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Hämtar det maximala antalet värden i en array av typen byte för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Returns:**
int - Det maximala antalet värden i en array av typen byte för att indexera fältet.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Ställer in det maximala antalet värden i en array av typen byte för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet värden i en array av typen byte för att indexera fältet. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Hämtar det maximala antalet värden i en array av typen int för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Returns:**
int - Det maximala antalet värden i en array av typen int för att indexera fältet.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Ställer in det maximala antalet värden i en array av typen int för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet värden i en array av typen int för att indexera fältet. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Hämtar det maximala antalet värden i en array av typen long för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Returns:**
int - Det maximala antalet värden i en array av typen long för att indexera fältet.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Ställer in det maximala antalet värden i en array av typen long för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet värden i en array av typen long för att indexera fältet. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Hämtar det maximala antalet värden i en array av typen double för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Returns:**
int - Det maximala antalet värden i en array av typen double för att indexera fältet.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Ställer in det maximala antalet värden i en array av typen double för att indexera fältet. Standardvärdet är  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet värden i en array av typen double för att indexera fältet. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Hämtar separatorn mellan värden i ett fält av typen array. Standardvärdet är mellanslagstecknet.


**Returns:**
java.lang.String - Separatorn mellan värden i ett fält av typen array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Ställer in separatorn mellan värden i ett fält av typen array. Standardvärdet är mellanslagstecknet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Separatorn mellan värden i ett fält av typen array. |
|

