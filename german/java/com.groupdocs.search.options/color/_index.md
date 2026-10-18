---
title: "Color"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt eine ARGB‑Alpha‑Rot‑Grün‑Blau‑Farbe dar."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Stellt eine ARGB‑Farbe (Alpha, Rot, Grün, Blau) dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Initialisiert eine neue Instanz der  Color  Klasse. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Initialisiert eine neue Instanz der  Color  Klasse. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Initialisiert eine neue Instanz der  Color  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Liest den Alpha‑Komponentenwert dieser Instanz. |
|
|  | [getRed()](#getRed--) | Gibt den Rotkomponentenwert dieser Instanz zurück. |
|
|  | [getGreen()](#getGreen--) | Gibt den Grünkomponentenwert dieser Instanz zurück. |
|
|  | [getBlue()](#getBlue--) | Gibt den Blaukomponentenwert dieser Instanz zurück. |
|
|  | [toString()](#toString--) | Gibt einen String zurück, der die aktuelle Farbe darstellt. |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Initialisiert eine neue Instanz der  Color  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Alpha | int | Die Alpha‑Komponente von 0 bis 255. |
|
|  | Rot | int | Die Rot‑Komponente von 0 bis 255. |
|
|  | Grün | int | Die Grün‑Komponente von 0 bis 255. |
|
|  | Blau | int | Die Blau‑Komponente von 0 bis 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Initialisiert eine neue Instanz der  Color  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Rot | int | Die Rot‑Komponente von 0 bis 255. |
|
|  | Grün | int | Die Grün‑Komponente von 0 bis 255. |
|
|  | Blau | int | Die Blau‑Komponente von 0 bis 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Initialisiert eine neue Instanz der  Color  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Liest den Alpha‑Komponentenwert dieser Instanz.


**Returns:**
int - Der Alpha‑Komponentenwert dieser Instanz.

### getRed() {#getRed--}
```
public int getRed()
```


Gibt den Rotkomponentenwert dieser Instanz zurück.


**Returns:**
int - Der Rot‑Komponentenwert dieser Instanz.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Gibt den Grünkomponentenwert dieser Instanz zurück.


**Returns:**
int - Der Grün‑Komponentenwert dieser Instanz.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Gibt den Blaukomponentenwert dieser Instanz zurück.


**Returns:**
int - Der Blau‑Komponentenwert dieser Instanz.

### toString() {#toString--}
```
public String toString()
```


Gibt einen String zurück, der die aktuelle Farbe darstellt.


**Returns:**
java.lang.String - Ein String, der die aktuelle Farbe darstellt.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
