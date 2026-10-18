---
title: "HighlightOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för att markera hittade termer."
type: docs
weight: 22
url: /sv/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Tillhandahåller alternativ för att markera hittade termer.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initierar en ny instans av klassen  HighlightOptions . |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Initierar en ny instans av klassen  TextOptions . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Hämtar det maximala antalet ord i ett textutdrag före det markerade ordet. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Ställer in det maximala antalet ord i ett textutdrag före det markerade ordet. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Hämtar det maximala antalet ord i ett textutdrag efter det markerade ordet. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Ställer in det maximala antalet ord i ett textutdrag efter det markerade ordet. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Hämtar det maximala antalet ord i ett textutdrag. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Ställer in det maximala antalet ord i ett textutdrag. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Hämtar ett värde som indikerar om inline‑stilar används för att markera förekomster. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Ställer in ett värde som indikerar om inline‑stilar används för att markera förekomster. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Hämtar en färg som används för att markera förekomster. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Ställer in en färg som används för att markera förekomster. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Hämtar starttaggen för markeringen av det hittade ordet. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Ställer in starttaggen för markeringen av det hittade ordet. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Hämtar sluttaggen för markeringen av det hittade ordet. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Ställer in sluttaggen för markeringen av det hittade ordet. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initierar en ny instans av klassen  HighlightOptions .


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Initierar en ny instans av klassen  TextOptions .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Hämtar det maximala antalet ord i ett textutdrag före det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 7.


**Returns:**
int - Det maximala antalet ord i ett textutdrag före det markerade ordet.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Ställer in det maximala antalet ord i ett textutdrag före det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 7.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet ord i ett textutdrag före det markerade ordet. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Hämtar det maximala antalet ord i ett textutdrag efter det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 7.


**Returns:**
int - Det maximala antalet ord i ett textutdrag efter det markerade ordet.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Ställer in det maximala antalet ord i ett textutdrag efter det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 7.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet ord i ett textutdrag efter det markerade ordet. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Hämtar det maximala antalet ord i ett textutdrag. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 21.


**Returns:**
int - Det maximala antalet ord i ett textutdrag.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Ställer in det maximala antalet ord i ett textutdrag. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är 21.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet ord i ett textutdrag. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Hämtar ett värde som indikerar om inbäddade stilar används för att markera förekomster. Standardvärdet är true.


**Returns:**
boolean - Ett värde som indikerar om inbäddade stilar används för att markera förekomster.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Ställer in ett värde som indikerar om inbäddade stilar används för att markera förekomster. Standardvärdet är true.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om inbäddade stilar används för att markera förekomster. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Hämtar en färg som används för att markera förekomster. Standardvärdet är #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Ställer in en färg som används för att markera förekomster. Standardvärdet är #FFD800.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | En färg som används för att markera förekomster. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Hämtar starttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng.


**Returns:**
java.lang.String - Starttaggen för markeringen av det hittade ordet.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Ställer in starttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Starttaggen för markeringen av det hittade ordet. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Hämtar sluttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng.


**Returns:**
java.lang.String - Sluttaggen för markeringen av det hittade ordet.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Ställer in sluttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Sluttaggen för markeringen av det hittade ordet. |
|

