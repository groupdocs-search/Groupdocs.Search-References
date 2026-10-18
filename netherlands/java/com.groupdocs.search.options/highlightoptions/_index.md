---
title: "HighlightOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor het markeren van gevonden termen."
type: docs
weight: 22
url: /nl/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Biedt opties voor het markeren van gevonden termen.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialiseert een nieuwe instantie van de  HighlightOptions  klasse. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Initialiseert een nieuwe instantie van de  TextOptions  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Haalt het maximale aantal woorden op in een tekstfragment vóór het gemarkeerde woord. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Stelt het maximale aantal woorden in een tekstfragment vóór het gemarkeerde woord in. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Haalt het maximale aantal woorden op in een tekstfragment na het gemarkeerde woord. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Stelt het maximale aantal woorden in een tekstfragment na het gemarkeerde woord in. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Haalt het maximale aantal woorden op in een tekstfragment. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Stelt het maximale aantal woorden in een tekstfragment in. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Haalt een waarde op die aangeeft of inline stijlen worden gebruikt om vermeldingen te markeren. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Stelt een waarde in die aangeeft of inline stijlen worden gebruikt om vermeldingen te markeren. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Haalt een kleur op die wordt gebruikt om vermeldingen te markeren. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Stelt een kleur in die wordt gebruikt om voorkomens te markeren. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Haalt de starttag op van de markering van het gevonden woord. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Stelt de starttag in van de markering van het gevonden woord. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Haalt de eindtag op van de markering van het gevonden woord. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Stelt de eindtag in van de markering van het gevonden woord. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialiseert een nieuwe instantie van de  HighlightOptions  klasse.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Initialiseert een nieuwe instantie van de  TextOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Haalt het maximale aantal woorden op in een tekstfragment vóór het gemarkeerde woord. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 7.


**Returns:**
int - Het maximale aantal woorden in een tekstfragment vóór het gemarkeerde woord.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Stelt het maximale aantal woorden in een tekstfragment vóór het gemarkeerde woord in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 7.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal woorden in een tekstfragment vóór het gemarkeerde woord. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Haalt het maximale aantal woorden op in een tekstfragment na het gemarkeerde woord. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 7.


**Returns:**
int - Het maximale aantal woorden in een tekstfragment na het gemarkeerde woord.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Stelt het maximale aantal woorden in een tekstfragment na het gemarkeerde woord in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 7.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal woorden in een tekstfragment na het gemarkeerde woord. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Haalt het maximale aantal woorden op in een tekstfragment. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 21.


**Returns:**
int - Het maximale aantal woorden in een tekstfragment.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Stelt het maximale aantal woorden in een tekstfragment in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is 21.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal woorden in een tekstfragment. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Haalt een waarde op die aangeeft of inline‑stijlen worden gebruikt om voorkomens te markeren. De standaardwaarde is true.


**Returns:**
boolean - Een waarde die aangeeft of inline‑stijlen worden gebruikt om voorkomens te markeren.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Stelt een waarde in die aangeeft of inline‑stijlen worden gebruikt om voorkomens te markeren. De standaardwaarde is true.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of inline‑stijlen worden gebruikt om voorkomens te markeren. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Haalt een kleur op die wordt gebruikt om voorkomens te markeren. De standaardwaarde is #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Stelt een kleur in die wordt gebruikt om voorkomens te markeren. De standaardwaarde is #FFD800.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Een kleur die wordt gebruikt om voorkomens te markeren. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Haalt de starttag op van de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks.


**Returns:**
java.lang.String - De starttag van de markering van het gevonden woord.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Stelt de starttag in van de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De starttag van de markering van het gevonden woord. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Haalt de eindtag op van de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks.


**Returns:**
java.lang.String - De eindtag van de markering van het gevonden woord.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Stelt de eindtag in van de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De eindtag van de markering van het gevonden woord. |
|

