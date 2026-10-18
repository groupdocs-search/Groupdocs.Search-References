---
title: "MetadataIndexingOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para indexar campos de metadatos."
type: docs
weight: 29
url: /es/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Proporciona opciones para indexar campos de metadatos.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Obtiene un valor que indica si se deben indexar los valores de campos vacíos o no. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Establece un valor que indica si se deben indexar los valores de campos vacíos o no. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Obtiene un valor que indica si se deben indexar los nombres de campos vacíos o no. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Establece un valor que indica si se deben indexar los nombres de campos vacíos o no. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Obtiene el nombre de campo predeterminado utilizado para indexar nombres de campos vacíos. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Establece el nombre de campo predeterminado utilizado para indexar nombres de campos vacíos. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Obtiene el separador en el nombre compuesto de un campo. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Establece el separador en el nombre compuesto de un campo. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Obtiene el número máximo de valores en una matriz de tipo byte para indexar el campo. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Establece el número máximo de valores en una matriz de tipo byte para indexar el campo. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Obtiene el número máximo de valores en una matriz de tipo int para indexar el campo. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Establece el número máximo de valores en una matriz de tipo int para indexar el campo. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Obtiene el número máximo de valores en una matriz de tipo long para indexar el campo. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Establece el número máximo de valores en una matriz de tipo long para indexar el campo. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Obtiene el número máximo de valores en una matriz de tipo double para indexar el campo. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Establece el número máximo de valores en una matriz de tipo double para indexar el campo. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Obtiene el separador entre valores en un campo de tipo matriz. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Establece el separador entre valores en un campo de tipo matriz. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Obtiene un valor que indica si se deben indexar los valores de campos vacíos o no. El valor predeterminado es true.


**Returns:**
boolean - Un valor que indica si se deben indexar los valores de campos vacíos o no.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Establece un valor que indica si se deben indexar los valores de campo vacíos o no. El valor predeterminado es true.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se deben indexar los valores de campo vacíos o no. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Obtiene un valor que indica si se deben indexar los nombres de campo vacíos o no. El valor predeterminado es true.


**Returns:**
boolean - Un valor que indica si se deben indexar los nombres de campo vacíos o no.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Establece un valor que indica si se deben indexar los nombres de campo vacíos o no. El valor predeterminado es true.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se deben indexar los nombres de campo vacíos o no. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Obtiene el nombre de campo predeterminado utilizado para indexar nombres de campo vacíos. El valor predeterminado es "unknown".


**Returns:**
java.lang.String - El nombre de campo predeterminado utilizado para indexar nombres de campo vacíos.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Establece el nombre de campo predeterminado utilizado para indexar nombres de campo vacíos. El valor predeterminado es "unknown".


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El nombre de campo predeterminado utilizado para indexar nombres de campo vacíos. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Obtiene el separador en el nombre compuesto de un campo. El valor predeterminado es ".".


**Returns:**
java.lang.String - El separador en el nombre compuesto de un campo.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Establece el separador en el nombre compuesto de un campo. El valor predeterminado es ".".


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El separador en el nombre compuesto de un campo. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Obtiene el número máximo de valores en una matriz de tipo byte para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Returns:**
int - El número máximo de valores en una matriz de tipo byte para indexar el campo.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Establece el número máximo de valores en una matriz de tipo byte para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de valores en una matriz de tipo byte para indexar el campo. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Obtiene el número máximo de valores en una matriz de tipo int para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Returns:**
int - El número máximo de valores en una matriz de tipo int para indexar el campo.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Establece el número máximo de valores en una matriz de tipo int para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de valores en una matriz de tipo int para indexar el campo. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Obtiene el número máximo de valores en una matriz de tipo long para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Returns:**
int - El número máximo de valores en una matriz de tipo long para indexar el campo.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Establece el número máximo de valores en una matriz de tipo long para indexar el campo. El valor predeterminado es Integer.MAX_VALUE.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de valores en una matriz de tipo long para indexar el campo. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Obtiene el número máximo de valores en una matriz de tipo double para indexar el campo. El valor predeterminado es  Integer.MAX_VALUE .


**Returns:**
int - El número máximo de valores en una matriz de tipo double para indexar el campo.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Establece el número máximo de valores en una matriz de tipo double para indexar el campo. El valor predeterminado es  Integer.MAX_VALUE .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de valores en una matriz de tipo double para indexar el campo. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Obtiene el separador entre valores en un campo de tipo matriz. El valor predeterminado es el signo de espacio.


**Returns:**
java.lang.String - El separador entre valores en un campo de tipo matriz.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Establece el separador entre valores en un campo de tipo matriz. El valor predeterminado es el signo de espacio.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | El separador entre valores en un campo de tipo matriz. |
|

