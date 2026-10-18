---
title: "HighlightOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para resaltar los términos encontrados."
type: docs
weight: 22
url: /es/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Proporciona opciones para resaltar los términos encontrados.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Inicializa una nueva instancia de la clase  HighlightOptions . |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Inicializa una nueva instancia de la clase  TextOptions . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Obtiene el número máximo de palabras en un fragmento de texto antes de la palabra resaltada. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Establece el número máximo de palabras en un fragmento de texto antes de la palabra resaltada. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Obtiene el número máximo de palabras en un fragmento de texto después de la palabra resaltada. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Establece el número máximo de palabras en un fragmento de texto después de la palabra resaltada. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Obtiene el número máximo de palabras en un fragmento de texto. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Establece el número máximo de palabras en un fragmento de texto. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Obtiene un valor que indica si se utilizan estilos en línea para resaltar ocurrencias. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Establece un valor que indica si se utilizan estilos en línea para resaltar ocurrencias. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Obtiene un color que se utiliza para resaltar ocurrencias. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Establece un color que se usa para resaltar ocurrencias. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Obtiene la etiqueta de inicio del resaltado de la palabra encontrada. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Establece la etiqueta de inicio del resaltado de la palabra encontrada. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Obtiene la etiqueta de fin del resaltado de la palabra encontrada. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Establece la etiqueta de fin del resaltado de la palabra encontrada. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Inicializa una nueva instancia de la clase  HighlightOptions .


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Inicializa una nueva instancia de la clase  TextOptions .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Obtiene el número máximo de palabras en un fragmento de texto antes de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 7.


**Returns:**
int - El número máximo de palabras en un fragmento de texto antes de la palabra resaltada.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Establece el número máximo de palabras en un fragmento de texto antes de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 7.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de palabras en un fragmento de texto antes de la palabra resaltada. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Obtiene el número máximo de palabras en un fragmento de texto después de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 7.


**Returns:**
int - El número máximo de palabras en un fragmento de texto después de la palabra resaltada.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Establece el número máximo de palabras en un fragmento de texto después de la palabra resaltada. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 7.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de palabras en un fragmento de texto después de la palabra resaltada. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Obtiene el número máximo de palabras en un fragmento de texto. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 21.


**Returns:**
int - El número máximo de palabras en un fragmento de texto.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Establece el número máximo de palabras en un fragmento de texto. El valor debe estar en el rango de 0 a 10000. El valor predeterminado es 21.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número máximo de palabras en un fragmento de texto. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Obtiene un valor que indica si se usan estilos en línea para resaltar ocurrencias. El valor predeterminado es true.


**Returns:**
boolean - Un valor que indica si se usan estilos en línea para resaltar ocurrencias.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Establece un valor que indica si se usan estilos en línea para resaltar ocurrencias. El valor predeterminado es true.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se usan estilos en línea para resaltar ocurrencias. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Obtiene un color que se usa para resaltar ocurrencias. El valor predeterminado es #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Establece un color que se usa para resaltar ocurrencias. El valor predeterminado es #FFD800.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Un color que se usa para resaltar ocurrencias. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Obtiene la etiqueta de inicio del resaltado de la palabra encontrada. Esta etiqueta se usa solo cuando se resalta en texto plano. El valor predeterminado es una cadena vacía.


**Returns:**
java.lang.String - La etiqueta de inicio del resaltado de la palabra encontrada.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Establece la etiqueta de inicio del resaltado de la palabra encontrada. Esta etiqueta se usa solo cuando se resalta en texto plano. El valor predeterminado es una cadena vacía.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | La etiqueta de inicio del resaltado de la palabra encontrada. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Obtiene la etiqueta de fin del resaltado de la palabra encontrada. Esta etiqueta se usa solo cuando se resalta en texto plano. El valor predeterminado es una cadena vacía.


**Returns:**
java.lang.String - La etiqueta de fin del resaltado de la palabra encontrada.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Establece la etiqueta de fin del resaltado de la palabra encontrada. Esta etiqueta se usa solo cuando se resalta en texto plano. El valor predeterminado es una cadena vacía.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | La etiqueta de fin del resaltado de la palabra encontrada. |
|

