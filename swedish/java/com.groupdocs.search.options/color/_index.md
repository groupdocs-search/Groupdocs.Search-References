---
title: "Color"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en ARGB alfa röd grön blå färg."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Representerar en ARGB-färg (alpha, röd, grön, blå).

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Initierar en ny instans av  Color  klassen. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Initierar en ny instans av  Color  klassen. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Initierar en ny instans av  Color  klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Hämtar alfakomponentens värde för denna instans. |
|
|  | [getRed()](#getRed--) | Hämtar det röda komponentvärdet för den här instansen. |
|
|  | [getGreen()](#getGreen--) | Hämtar det gröna komponentvärdet för den här instansen. |
|
|  | [getBlue()](#getBlue--) | Hämtar det blåa komponentvärdet för den här instansen. |
|
|  | [toString()](#toString--) | Returnerar en  String  som representerar den aktuella  Color . |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Initierar en ny instans av  Color  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | alpha | int | Alfakomponenten från 0 till 255. |
|
|  | röd | int | Den röda komponenten från 0 till 255. |
|
|  | grön | int | Den gröna komponenten från 0 till 255. |
|
|  | blå | int | Den blåa komponenten från 0 till 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Initierar en ny instans av  Color  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | röd | int | Den röda komponenten från 0 till 255. |
|
|  | grön | int | Den gröna komponenten från 0 till 255. |
|
|  | blå | int | Den blåa komponenten från 0 till 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Initierar en ny instans av  Color  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Hämtar alfakomponentens värde för denna instans.


**Returns:**
int - Alfakomponentvärdet för den här instansen.

### getRed() {#getRed--}
```
public int getRed()
```


Hämtar det röda komponentvärdet för den här instansen.


**Returns:**
int - Det röda komponentvärdet för den här instansen.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Hämtar det gröna komponentvärdet för den här instansen.


**Returns:**
int - Det gröna komponentvärdet för den här instansen.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Hämtar det blåa komponentvärdet för den här instansen.


**Returns:**
int - Det blåa komponentvärdet för den här instansen.

### toString() {#toString--}
```
public String toString()
```


Returnerar en  String  som representerar den aktuella  Color .


**Returns:**
java.lang.String - En  String  som representerar den aktuella  Color .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
