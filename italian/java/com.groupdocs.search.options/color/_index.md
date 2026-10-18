---
title: "Color"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un colore ARGB alfa rosso verde blu."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Rappresenta un colore ARGB (alpha, rosso, verde, blu).

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Inizializza una nuova istanza della classe Color. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Inizializza una nuova istanza della classe Color. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Inizializza una nuova istanza della classe Color. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Ottiene il valore del componente alfa di questa istanza. |
|
|  | [getRed()](#getRed--) | Ottiene il valore del componente rosso di questa istanza. |
|
|  | [getGreen()](#getGreen--) | Ottiene il valore del componente verde di questa istanza. |
|
|  | [getBlue()](#getBlue--) | Ottiene il valore del componente blu di questa istanza. |
|
|  | [toString()](#toString--) | Restituisce una  String  che rappresenta il  Color . |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Inizializza una nuova istanza della classe Color.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | alpha | int | Il componente alpha da 0 a 255. |
|
|  | red | int | Il componente rosso da 0 a 255. |
|
|  | green | int | Il componente verde da 0 a 255. |
|
|  | blue | int | Il componente blu da 0 a 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Inizializza una nuova istanza della classe Color.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | red | int | Il componente rosso da 0 a 255. |
|
|  | green | int | Il componente verde da 0 a 255. |
|
|  | blue | int | Il componente blu da 0 a 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Inizializza una nuova istanza della classe Color.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Ottiene il valore del componente alfa di questa istanza.


**Returns:**
int - Il valore del componente alpha di questa istanza.

### getRed() {#getRed--}
```
public int getRed()
```


Ottiene il valore del componente rosso di questa istanza.


**Returns:**
int - Il valore del componente rosso di questa istanza.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Ottiene il valore del componente verde di questa istanza.


**Returns:**
int - Il valore del componente verde di questa istanza.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Ottiene il valore del componente blu di questa istanza.


**Returns:**
int - Il valore del componente blu di questa istanza.

### toString() {#toString--}
```
public String toString()
```


Restituisce una  String  che rappresenta il  Color .


**Returns:**
java.lang.String - Una  String  che rappresenta il  Color .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
