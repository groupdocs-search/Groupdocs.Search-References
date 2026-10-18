---
title: "SpellingCorrectorOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para el corrector ortográfico."
type: docs
weight: 36
url: /es/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Proporciona opciones para el corrector ortográfico.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtiene un valor que indica si el corrector ortográfico está habilitado. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Establece un valor que indica si el corrector ortográfico está habilitado. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Obtiene el número máximo de errores. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Establece el número máximo de errores. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Obtiene un valor que indica si solo se devolverán los mejores resultados. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Establece un valor que indica si solo se devolverán los mejores resultados. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Obtiene el exceso máximo del número mínimo de errores que se encuentran. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Establece el exceso máximo del número mínimo de errores que se encuentran. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Obtiene un valor que indica si el algoritmo debe considerar la transposición de dos caracteres adyacentes como un solo error. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Establece un valor que indica si el algoritmo debe considerar la transposición de dos caracteres adyacentes como un solo error. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Obtiene un valor que indica si el corrector ortográfico está habilitado. El valor predeterminado es false.


**Returns:**
boolean - Un valor que indica si el corrector ortográfico está habilitado.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Establece un valor que indica si el corrector ortográfico está habilitado. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si el corrector ortográfico está habilitado. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Obtiene el número máximo de errores. El valor predeterminado es 2.


**Returns:**
int - El número máximo de errores.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Establece el número máximo de errores. El valor predeterminado es  2 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de errores. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Obtiene un valor que indica si solo se devolverán los mejores resultados. El valor predeterminado es  false .


**Returns:**
boolean -  true  si solo se devolverán los mejores resultados; de lo contrario  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Establece un valor que indica si solo se devolverán los mejores resultados. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | true  si solo se devolverán los mejores resultados; de lo contrario  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Obtiene el exceso máximo del número mínimo de errores que se encuentran. El valor predeterminado es  0 .


**Returns:**
byte - El exceso máximo del número mínimo de errores encontrados.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Establece el exceso máximo del número mínimo de errores que se encuentran. El valor predeterminado es  0 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | byte | El exceso máximo del número mínimo de errores encontrados. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Obtiene un valor que indica si el algoritmo debe considerar la transposición de dos caracteres adyacentes como un solo error. El valor predeterminado es  true .


**Returns:**
boolean -  true  si el algoritmo corrector ortográfico considera transposiciones; de lo contrario  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Establece un valor que indica si el algoritmo debe considerar la transposición de dos caracteres adyacentes como un solo error. El valor predeterminado es  true .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | true  si el algoritmo corrector ortográfico considera transposiciones; de lo contrario  false . |
|

