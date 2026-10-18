---
title: "HighlightOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per evidenziare i termini trovati."
type: docs
weight: 22
url: /it/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Fornisce opzioni per evidenziare i termini trovati.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Inizializza una nuova istanza della classe  HighlightOptions . |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Inizializza una nuova istanza della classe  TextOptions . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Ottiene il numero massimo di parole in un frammento di testo prima della parola evidenziata. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Imposta il numero massimo di parole in un frammento di testo prima della parola evidenziata. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Ottiene il numero massimo di parole in un frammento di testo dopo la parola evidenziata. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Imposta il numero massimo di parole in un frammento di testo dopo la parola evidenziata. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Ottiene il numero massimo di parole in un frammento di testo. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Imposta il numero massimo di parole in un frammento di testo. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Ottiene un valore che indica se gli stili inline sono usati per evidenziare le occorrenze. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Imposta un valore che indica se gli stili inline sono usati per evidenziare le occorrenze. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Ottiene un colore che è usato per evidenziare le occorrenze. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Imposta un colore utilizzato per evidenziare le occorrenze. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Ottiene il tag di inizio dell'evidenziazione della parola trovata. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Imposta il tag di inizio dell'evidenziazione della parola trovata. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Ottiene il tag di fine dell'evidenziazione della parola trovata. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Imposta il tag di fine dell'evidenziazione della parola trovata. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Inizializza una nuova istanza della classe  HighlightOptions .


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Inizializza una nuova istanza della classe  TextOptions .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Ottiene il numero massimo di parole in un frammento di testo prima della parola evidenziata. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 7.


**Returns:**
int - Il numero massimo di parole in un frammento di testo prima della parola evidenziata.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Imposta il numero massimo di parole in un frammento di testo prima della parola evidenziata. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 7.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di parole in un frammento di testo prima della parola evidenziata. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Ottiene il numero massimo di parole in un frammento di testo dopo la parola evidenziata. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 7.


**Returns:**
int - Il numero massimo di parole in un frammento di testo dopo la parola evidenziata.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Imposta il numero massimo di parole in un frammento di testo dopo la parola evidenziata. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 7.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di parole in un frammento di testo dopo la parola evidenziata. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Ottiene il numero massimo di parole in un frammento di testo. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 21.


**Returns:**
int - Il numero massimo di parole in un frammento di testo.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Imposta il numero massimo di parole in un frammento di testo. Il valore deve essere compreso nell'intervallo da 0 a 10000. Il valore predefinito è 21.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di parole in un frammento di testo. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Ottiene un valore che indica se gli stili inline sono usati per evidenziare le occorrenze. Il valore predefinito è true.


**Returns:**
boolean - Un valore che indica se gli stili inline sono usati per evidenziare le occorrenze.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Imposta un valore che indica se gli stili inline sono usati per evidenziare le occorrenze. Il valore predefinito è true.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se gli stili inline sono usati per evidenziare le occorrenze. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Ottiene un colore utilizzato per evidenziare le occorrenze. Il valore predefinito è #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Imposta un colore utilizzato per evidenziare le occorrenze. Il valore predefinito è #FFD800.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Un colore utilizzato per evidenziare le occorrenze. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Restituisce il tag di inizio dell'evidenziazione della parola trovata. Questo tag è usato solo quando si evidenzia in testo semplice. Il valore predefinito è una stringa vuota.


**Returns:**
java.lang.String - Il tag di inizio dell'evidenziazione della parola trovata.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Imposta il tag di inizio dell'evidenziazione della parola trovata. Questo tag è usato solo quando si evidenzia in testo semplice. Il valore predefinito è una stringa vuota.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il tag di inizio dell'evidenziazione della parola trovata. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Restituisce il tag di fine dell'evidenziazione della parola trovata. Questo tag è usato solo quando si evidenzia in testo semplice. Il valore predefinito è una stringa vuota.


**Returns:**
java.lang.String - Il tag di fine dell'evidenziazione della parola trovata.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Imposta il tag di fine dell'evidenziazione della parola trovata. Questo tag è usato solo quando si evidenzia in testo semplice. Il valore predefinito è una stringa vuota.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | Il tag di fine dell'evidenziazione della parola trovata. |
|

