---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für das Indexieren von Metadatenfeldern bereit."
type: docs
weight: 29
url: /de/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Stellt Optionen für das Indexieren von Metadatenfeldern bereit.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Gibt einen Wert zurück, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Setzt einen Wert, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Gibt einen Wert zurück, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Setzt einen Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Gibt den Standardfeldnamen zurück, der zum Indizieren leerer Feldnamen verwendet wird. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Setzt den Standardfeldnamen, der zum Indizieren leerer Feldnamen verwendet wird. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Gibt das Trennzeichen im zusammengesetzten Namen eines Feldes zurück. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Setzt das Trennzeichen im zusammengesetzten Namen eines Feldes. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Gibt die maximale Anzahl von Werten in einem Array vom Typ byte zurück, um das Feld zu indizieren. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Setzt die maximale Anzahl von Werten in einem Array vom Typ byte, um das Feld zu indizieren. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Gibt die maximale Anzahl von Werten in einem Array vom Typ int zurück, um das Feld zu indizieren. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Setzt die maximale Anzahl von Werten in einem Array vom Typ int, um das Feld zu indizieren. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Gibt die maximale Anzahl von Werten in einem Array vom Typ long zurück, um das Feld zu indizieren. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Setzt die maximale Anzahl von Werten in einem Array vom Typ long, um das Feld zu indizieren. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Gibt die maximale Anzahl von Werten in einem Array vom Typ double zurück, um das Feld zu indizieren. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Setzt die maximale Anzahl von Werten in einem Array vom Typ double, um das Feld zu indizieren. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Gibt das Trennzeichen zwischen Werten in einem Feld vom Typ array zurück. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Setzt das Trennzeichen zwischen Werten in einem Feld vom Typ array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Gibt einen Wert zurück, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. Der Standardwert ist true.


**Returns:**
boolean - Ein Wert, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Setzt einen Wert, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. Der Standardwert ist  true .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob leere Feldwerte indiziert werden sollen oder nicht. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Liefert einen Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. Der Standardwert ist  true .


**Returns:**
boolean - Ein Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Setzt einen Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. Der Standardwert ist  true .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob leere Feldnamen indiziert werden sollen oder nicht. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Liefert den Standardfeldnamen, der zum Indizieren leerer Feldnamen verwendet wird. Der Standardwert ist  \"unknown\" .


**Returns:**
java.lang.String - Der Standardfeldname, der zum Indizieren leerer Feldnamen verwendet wird.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Setzt den Standardfeldnamen, der zum Indizieren leerer Feldnamen verwendet wird. Der Standardwert ist  \"unknown\" .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Der Standardfeldname, der zum Indizieren leerer Feldnamen verwendet wird. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Liefert das Trennzeichen im zusammengesetzten Namen eines Feldes. Der Standardwert ist  \".\" .


**Returns:**
java.lang.String - Das Trennzeichen im zusammengesetzten Namen eines Feldes.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Setzt das Trennzeichen im zusammengesetzten Namen eines Feldes. Der Standardwert ist  \".\" .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Das Trennzeichen im zusammengesetzten Namen eines Feldes. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Liefert die maximale Anzahl von Werten in einem Array vom Typ byte, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Returns:**
int - Die maximale Anzahl von Werten in einem Array vom Typ byte, um das Feld zu indizieren.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Setzt die maximale Anzahl von Werten in einem Array vom Typ byte, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Werten in einem Array vom Typ byte, um das Feld zu indizieren. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Liefert die maximale Anzahl von Werten in einem Array vom Typ int, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Returns:**
int - Die maximale Anzahl von Werten in einem Array vom Typ int, um das Feld zu indizieren.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Setzt die maximale Anzahl von Werten in einem Array vom Typ int, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Werten in einem Array vom Typ int, um das Feld zu indizieren. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Liefert die maximale Anzahl von Werten in einem Array vom Typ long, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Returns:**
int - Die maximale Anzahl von Werten in einem Array vom Typ long, um das Feld zu indizieren.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Setzt die maximale Anzahl von Werten in einem Array vom Typ long, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Werten in einem Array vom Typ long, um das Feld zu indizieren. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Liest die maximale Anzahl von Werten in einem Array vom Typ double, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Returns:**
int - Die maximale Anzahl von Werten in einem Array vom Typ double, um das Feld zu indizieren.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Setzt die maximale Anzahl von Werten in einem Array vom Typ double, um das Feld zu indizieren. Der Standardwert ist  Integer.MAX_VALUE .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Werten in einem Array vom Typ double, um das Feld zu indizieren. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Liest das Trennzeichen zwischen Werten in einem Feld vom Typ Array. Der Standardwert ist das Leerzeichen.


**Returns:**
java.lang.String - Das Trennzeichen zwischen Werten in einem Feld vom Typ Array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Setzt das Trennzeichen zwischen Werten in einem Feld vom Typ Array. Der Standardwert ist das Leerzeichen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Das Trennzeichen zwischen Werten in einem Feld vom Typ Array. |
|

