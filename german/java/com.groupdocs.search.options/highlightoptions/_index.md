---
title: "HighlightOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Bietet Optionen zum Hervorheben gefundener Begriffe."
type: docs
weight: 22
url: /de/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Bietet Optionen zum Hervorheben gefundener Begriffe.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialisiert eine neue Instanz der  HighlightOptions  Klasse. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Initialisiert eine neue Instanz der  TextOptions  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Liefert die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Legt die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort fest. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Liefert die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Legt die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort fest. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Liefert die maximale Anzahl von Wörtern in einem Textausschnitt. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Legt die maximale Anzahl von Wörtern in einem Textausschnitt fest. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Liefert einen Wert, der angibt, ob Inline-Stile verwendet werden, um Vorkommen hervorzuheben. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Legt einen Wert fest, der angibt, ob Inline-Stile verwendet werden, um Vorkommen hervorzuheben. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Liefert eine Farbe, die zum Hervorheben von Vorkommen verwendet wird. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Legt eine Farbe fest, die zum Hervorheben von Vorkommen verwendet wird. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Liest das Start-Tag der Hervorhebung des gefundenen Wortes. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Legt das Start-Tag der Hervorhebung des gefundenen Wortes fest. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Liest das End-Tag der Hervorhebung des gefundenen Wortes. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Legt das End-Tag der Hervorhebung des gefundenen Wortes fest. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialisiert eine neue Instanz der  HighlightOptions  Klasse.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Initialisiert eine neue Instanz der  TextOptions  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Liest die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 7.


**Returns:**
int – Die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Legt die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort fest. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 7.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Wörtern in einem Textausschnitt vor dem hervorgehobenen Wort. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Liest die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 7.


**Returns:**
int – Die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Legt die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort fest. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 7.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Wörtern in einem Textausschnitt nach dem hervorgehobenen Wort. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Liest die maximale Anzahl von Wörtern in einem Textausschnitt. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 21.


**Returns:**
int – Die maximale Anzahl von Wörtern in einem Textausschnitt.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Legt die maximale Anzahl von Wörtern in einem Textausschnitt fest. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist 21.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Wörtern in einem Textausschnitt. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Liest einen Wert, der angibt, ob Inline-Stile zum Hervorheben von Vorkommen verwendet werden. Der Standardwert ist true.


**Returns:**
boolean – Ein Wert, der angibt, ob Inline-Stile zum Hervorheben von Vorkommen verwendet werden.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Legt einen Wert fest, der angibt, ob Inline-Stile zum Hervorheben von Vorkommen verwendet werden. Der Standardwert ist true.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Inline-Stile zum Hervorheben von Vorkommen verwendet werden. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Liest eine Farbe, die zum Hervorheben von Vorkommen verwendet wird. Der Standardwert ist #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Legt eine Farbe fest, die zum Hervorheben von Vorkommen verwendet wird. Der Standardwert ist #FFD800.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Eine Farbe, die verwendet wird, um Vorkommen hervorzuheben. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Liest das Start-Tag der Hervorhebung des gefundenen Wortes. Dieses Tag wird nur beim Hervorheben im Nur-Text verwendet. Der Standardwert ist ein leerer String.


**Returns:**
java.lang.String – Das Start-Tag der Hervorhebung des gefundenen Wortes.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Setzt das Start-Tag der Hervorhebung des gefundenen Wortes. Dieses Tag wird nur beim Hervorheben im Nur-Text verwendet. Der Standardwert ist ein leerer String.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Das Start-Tag der Hervorhebung des gefundenen Wortes. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Liest das End-Tag der Hervorhebung des gefundenen Wortes. Dieses Tag wird nur beim Hervorheben im Nur-Text verwendet. Der Standardwert ist ein leerer String.


**Returns:**
java.lang.String – Das End-Tag der Hervorhebung des gefundenen Wortes.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Setzt das End-Tag der Hervorhebung des gefundenen Wortes. Dieses Tag wird nur beim Hervorheben im Nur-Text verwendet. Der Standardwert ist ein leerer String.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Das End-Tag der Hervorhebung des gefundenen Wortes. |
|

