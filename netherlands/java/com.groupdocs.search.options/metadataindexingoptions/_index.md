---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor het indexeren van metagegevensvelden."
type: docs
weight: 29
url: /nl/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Biedt opties voor het indexeren van metagegevensvelden.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Haalt een waarde op die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Stelt een waarde in die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Haalt een waarde op die aangeeft of lege veldnamen moeten worden geïndexeerd of niet. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Stelt een waarde in die aangeeft of lege veldnamen moeten worden geïndexeerd of niet. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Haalt de standaard veldnaam op die wordt gebruikt om lege veldnamen te indexeren. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Stelt de standaard veldnaam in die wordt gebruikt om lege veldnamen te indexeren. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Haalt het scheidingsteken op in de samengestelde naam van een veld. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Stelt het scheidingsteken in in de samengestelde naam van een veld. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Haalt het maximale aantal waarden op in een array van het type byte om het veld te indexeren. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Stelt het maximale aantal waarden in in een array van het type byte om het veld te indexeren. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Haalt het maximale aantal waarden op in een array van het type int om het veld te indexeren. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Stelt het maximale aantal waarden in in een array van het type int om het veld te indexeren. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Haalt het maximale aantal waarden op in een array van het type long om het veld te indexeren. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Stelt het maximale aantal waarden in in een array van het type long om het veld te indexeren. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Haalt het maximale aantal waarden op in een array van het type double om het veld te indexeren. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Stelt het maximale aantal waarden in in een array van het type double om het veld te indexeren. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Haalt het scheidingsteken op tussen waarden in een veld van het type array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Stelt het scheidingsteken in tussen waarden in een veld van het type array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Haalt een waarde op die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet. De standaardwaarde is  true .


**Returns:**
boolean - Een waarde die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Stelt een waarde in die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet. De standaardwaarde is true.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of lege veldwaarden moeten worden geïndexeerd of niet. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Haalt een waarde op die aangeeft of lege veldnamen moeten worden geïndexeerd of niet. De standaardwaarde is true.


**Returns:**
boolean - Een waarde die aangeeft of lege veldnamen moeten worden geïndexeerd of niet.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Stelt een waarde in die aangeeft of lege veldnamen moeten worden geïndexeerd of niet. De standaardwaarde is true.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of lege veldnamen moeten worden geïndexeerd of niet. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Haalt de standaard veldnaam op die wordt gebruikt om lege veldnamen te indexeren. De standaardwaarde is "unknown".


**Returns:**
java.lang.String - De standaard veldnaam die wordt gebruikt om lege veldnamen te indexeren.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Stelt de standaard veldnaam in die wordt gebruikt om lege veldnamen te indexeren. De standaardwaarde is "unknown".


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De standaard veldnaam die wordt gebruikt om lege veldnamen te indexeren. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Haalt het scheidingsteken op in de samengestelde naam van een veld. De standaardwaarde is ".".


**Returns:**
java.lang.String - Het scheidingsteken in de samengestelde naam van een veld.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Stelt het scheidingsteken in de samengestelde naam van een veld in. De standaardwaarde is ".".


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Het scheidingsteken in de samengestelde naam van een veld. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Haalt het maximale aantal waarden op in een array van het type byte om het veld te indexeren. De standaardwaarde is Integer.MAX_VALUE.


**Returns:**
int - Het maximale aantal waarden in een array van het type byte om het veld te indexeren.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Stelt het maximale aantal waarden in een array van het type byte om het veld te indexeren in. De standaardwaarde is Integer.MAX_VALUE.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal waarden in een array van het type byte om het veld te indexeren. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Haalt het maximale aantal waarden op in een array van het type int om het veld te indexeren. De standaardwaarde is Integer.MAX_VALUE.


**Returns:**
int - Het maximale aantal waarden in een array van het type int om het veld te indexeren.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Stelt het maximale aantal waarden in een array van het type int om het veld te indexeren in. De standaardwaarde is Integer.MAX_VALUE.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal waarden in een array van het type int om het veld te indexeren. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Haalt het maximale aantal waarden op in een array van het type long om het veld te indexeren. De standaardwaarde is Integer.MAX_VALUE.


**Returns:**
int - Het maximale aantal waarden in een array van het type long om het veld te indexeren.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Stelt het maximale aantal waarden in een array van het type long om het veld te indexeren in. De standaardwaarde is Integer.MAX_VALUE.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximum aantal waarden in een array van het type long om het veld te indexeren. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Haalt het maximum aantal waarden op in een array van het type double om het veld te indexeren. De standaardwaarde is Integer.MAX_VALUE.


**Returns:**
int - Het maximum aantal waarden in een array van het type double om het veld te indexeren.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Stelt het maximum aantal waarden in een array van het type double om het veld te indexeren in. De standaardwaarde is Integer.MAX_VALUE.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximum aantal waarden in een array van het type double om het veld te indexeren. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Haalt de scheidingsteken tussen waarden op in een veld van het type array. De standaardwaarde is het spatie-teken.


**Returns:**
java.lang.String - De scheidingsteken tussen waarden in een veld van het type array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Stelt de scheidingsteken tussen waarden in een veld van het type array in. De standaardwaarde is het spatie-teken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De scheidingsteken tussen waarden in een veld van het type array. |
|

