---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'indicizzazione dei campi dei metadati."
type: docs
weight: 29
url: /it/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Fornisce opzioni per l'indicizzazione dei campi dei metadati.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Restituisce un valore che indica se indicizzare i valori dei campi vuoti o meno. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Imposta un valore che indica se indicizzare i valori dei campi vuoti o meno. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Restituisce un valore che indica se indicizzare i nomi dei campi vuoti o meno. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Imposta un valore che indica se indicizzare i nomi dei campi vuoti o meno. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Restituisce il nome di campo predefinito utilizzato per indicizzare i nomi dei campi vuoti. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Imposta il nome di campo predefinito utilizzato per indicizzare i nomi dei campi vuoti. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Restituisce il separatore nel nome composto di un campo. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Imposta il separatore nel nome composto di un campo. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Restituisce il numero massimo di valori in un array di tipo byte da indicizzare nel campo. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Imposta il numero massimo di valori in un array di tipo byte da indicizzare nel campo. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Restituisce il numero massimo di valori in un array di tipo int da indicizzare nel campo. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Imposta il numero massimo di valori in un array di tipo int da indicizzare nel campo. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Restituisce il numero massimo di valori in un array di tipo long da indicizzare nel campo. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Imposta il numero massimo di valori in un array di tipo long da indicizzare nel campo. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Restituisce il numero massimo di valori in un array di tipo double da indicizzare nel campo. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Imposta il numero massimo di valori in un array di tipo double da indicizzare nel campo. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Restituisce il separatore tra i valori in un campo di tipo array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Imposta il separatore tra i valori in un campo di tipo array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Restituisce un valore che indica se indicizzare i valori dei campi vuoti o meno. Il valore predefinito è true.


**Returns:**
boolean - Un valore che indica se indicizzare i valori dei campi vuoti o meno.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Imposta un valore che indica se indicizzare i valori dei campi vuoti o meno. Il valore predefinito è  true .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se indicizzare i valori dei campi vuoti o meno. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Ottiene un valore che indica se indicizzare i nomi dei campi vuoti o meno. Il valore predefinito è  true .


**Returns:**
boolean - Un valore che indica se indicizzare i nomi dei campi vuoti o meno.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Imposta un valore che indica se indicizzare i nomi dei campi vuoti o meno. Il valore predefinito è  true .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se indicizzare i nomi dei campi vuoti o meno. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Ottiene il nome del campo predefinito usato per indicizzare i nomi dei campi vuoti. Il valore predefinito è  \"unknown\" .


**Returns:**
java.lang.String - Il nome del campo predefinito usato per indicizzare i nomi dei campi vuoti.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Imposta il nome del campo predefinito usato per indicizzare i nomi dei campi vuoti. Il valore predefinito è  \"unknown\" .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il nome del campo predefinito usato per indicizzare i nomi dei campi vuoti. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Ottiene il separatore nel nome composto di un campo. Il valore predefinito è  \".\" .


**Returns:**
java.lang.String - Il separatore nel nome composto di un campo.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Imposta il separatore nel nome composto di un campo. Il valore predefinito è  \".\" .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il separatore nel nome composto di un campo. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Ottiene il numero massimo di valori in un array di tipo byte da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Returns:**
int - Il numero massimo di valori in un array di tipo byte da indicizzare nel campo.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Imposta il numero massimo di valori in un array di tipo byte da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di valori in un array di tipo byte da indicizzare nel campo. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Ottiene il numero massimo di valori in un array di tipo int da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Returns:**
int - Il numero massimo di valori in un array di tipo int da indicizzare nel campo.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Imposta il numero massimo di valori in un array di tipo int da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di valori in un array di tipo int da indicizzare nel campo. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Ottiene il numero massimo di valori in un array di tipo long da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Returns:**
int - Il numero massimo di valori in un array di tipo long da indicizzare nel campo.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Imposta il numero massimo di valori in un array di tipo long da indicizzare nel campo. Il valore predefinito è  Integer.MAX_VALUE .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di valori in un array di tipo long da indicizzare nel campo. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Ottiene il numero massimo di valori in un array di tipo double da indicizzare nel campo. Il valore predefinito è Integer.MAX_VALUE.


**Returns:**
int - Il numero massimo di valori in un array di tipo double da indicizzare nel campo.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Imposta il numero massimo di valori in un array di tipo double da indicizzare nel campo. Il valore predefinito è Integer.MAX_VALUE.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di valori in un array di tipo double da indicizzare nel campo. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Ottiene il separatore tra i valori in un campo di tipo array. Il valore predefinito è il segno di spazio.


**Returns:**
java.lang.String - Il separatore tra i valori in un campo di tipo array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Imposta il separatore tra i valori in un campo di tipo array. Il valore predefinito è il segno di spazio.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il separatore tra i valori in un campo di tipo array. |
|

