---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'indexation des champs de métadonnées."
type: docs
weight: 29
url: /fr/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Fournit des options pour l'indexation des champs de métadonnées.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Obtient une valeur indiquant s'il faut indexer les valeurs de champ vides ou non. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Définit une valeur indiquant s'il faut indexer les valeurs de champ vides ou non. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Obtient une valeur indiquant s'il faut indexer les noms de champ vides ou non. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Définit une valeur indiquant s'il faut indexer les noms de champ vides ou non. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Obtient le nom de champ par défaut utilisé pour indexer les noms de champ vides. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Définit le nom de champ par défaut utilisé pour indexer les noms de champ vides. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Obtient le séparateur dans le nom composé d'un champ. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Définit le séparateur dans le nom composé d'un champ. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Obtient le nombre maximal de valeurs dans un tableau de type byte à indexer pour le champ. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Définit le nombre maximal de valeurs dans un tableau de type byte à indexer pour le champ. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Obtient le nombre maximal de valeurs dans un tableau de type int à indexer pour le champ. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Définit le nombre maximal de valeurs dans un tableau de type int à indexer pour le champ. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Obtient le nombre maximal de valeurs dans un tableau de type long à indexer pour le champ. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Définit le nombre maximal de valeurs dans un tableau de type long à indexer pour le champ. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Obtient le nombre maximal de valeurs dans un tableau de type double à indexer pour le champ. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Définit le nombre maximal de valeurs dans un tableau de type double à indexer pour le champ. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Obtient le séparateur entre les valeurs dans un champ de type tableau. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Définit le séparateur entre les valeurs dans un champ de type tableau. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Obtient une valeur indiquant s'il faut indexer les valeurs de champ vides ou non. La valeur par défaut est true.


**Returns:**
booléen - Une valeur indiquant s'il faut indexer les valeurs de champ vides ou non.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Définit une valeur indiquant s'il faut indexer les valeurs de champ vides ou non. La valeur par défaut est true.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut indexer les valeurs de champ vides ou non. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Obtient une valeur indiquant s'il faut indexer les noms de champ vides ou non. La valeur par défaut est true.


**Returns:**
boolean - Une valeur indiquant s'il faut indexer les noms de champ vides ou non.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Définit une valeur indiquant s'il faut indexer les noms de champ vides ou non. La valeur par défaut est true.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut indexer les noms de champ vides ou non. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Obtient le nom de champ par défaut utilisé pour indexer les noms de champ vides. La valeur par défaut est "unknown".


**Returns:**
java.lang.String - Le nom de champ par défaut utilisé pour indexer les noms de champ vides.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Définit le nom de champ par défaut utilisé pour indexer les noms de champ vides. La valeur par défaut est "unknown".


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le nom de champ par défaut utilisé pour indexer les noms de champ vides. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Obtient le séparateur dans le nom composé d'un champ. La valeur par défaut est ".".


**Returns:**
java.lang.String - Le séparateur dans le nom composé d'un champ.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Définit le séparateur dans le nom composé d'un champ. La valeur par défaut est ".".


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le séparateur dans le nom composé d'un champ. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Obtient le nombre maximal de valeurs dans un tableau de type byte à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Returns:**
int - Le nombre maximal de valeurs dans un tableau de type byte à indexer le champ.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Définit le nombre maximal de valeurs dans un tableau de type byte à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de valeurs dans un tableau de type byte à indexer le champ. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Obtient le nombre maximal de valeurs dans un tableau de type int à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Returns:**
int - Le nombre maximal de valeurs dans un tableau de type int à indexer le champ.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Définit le nombre maximal de valeurs dans un tableau de type int à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de valeurs dans un tableau de type int à indexer le champ. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Obtient le nombre maximal de valeurs dans un tableau de type long à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Returns:**
int - Le nombre maximal de valeurs dans un tableau de type long à indexer le champ.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Définit le nombre maximal de valeurs dans un tableau de type long à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de valeurs dans un tableau de type long à indexer le champ. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Obtient le nombre maximal de valeurs dans un tableau de type double à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Returns:**
int - Le nombre maximal de valeurs dans un tableau de type double à indexer le champ.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Définit le nombre maximal de valeurs dans un tableau de type double à indexer le champ. La valeur par défaut est Integer.MAX_VALUE.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de valeurs dans un tableau de type double à indexer le champ. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Obtient le séparateur entre les valeurs dans un champ de type tableau. La valeur par défaut est le signe espace.


**Returns:**
java.lang.String - Le séparateur entre les valeurs dans un champ de type tableau.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Définit le séparateur entre les valeurs dans un champ de type tableau. La valeur par défaut est le signe espace.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le séparateur entre les valeurs dans un champ de type tableau. |
|

