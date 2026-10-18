---
title: "Color"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un color ARGB alfa rojo verde azul."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Representa un color ARGB (alfa, rojo, verde, azul).

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Inicializa una nueva instancia de la  Color  clase. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Inicializa una nueva instancia de la  Color  clase. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Inicializa una nueva instancia de la  Color  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Obtiene el valor del componente alfa de esta instancia. |
|
|  | [getRed()](#getRed--) | Obtiene el valor del componente rojo de esta instancia. |
|
|  | [getGreen()](#getGreen--) | Obtiene el valor del componente verde de esta instancia. |
|
|  | [getBlue()](#getBlue--) | Obtiene el valor del componente azul de esta instancia. |
|
|  | [toString()](#toString--) | Devuelve una  String  que representa el  Color  actual. |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Inicializa una nueva instancia de la  Color  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | alfa | int | El componente alfa de 0 a 255. |
|
|  | rojo | int | El componente rojo de 0 a 255. |
|
|  | verde | int | El componente verde de 0 a 255. |
|
|  | azul | int | El componente azul de 0 a 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Inicializa una nueva instancia de la  Color  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | rojo | int | El componente rojo de 0 a 255. |
|
|  | verde | int | El componente verde de 0 a 255. |
|
|  | azul | int | El componente azul de 0 a 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Inicializa una nueva instancia de la  Color  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Obtiene el valor del componente alfa de esta instancia.


**Returns:**
int - El valor del componente alfa de esta instancia.

### getRed() {#getRed--}
```
public int getRed()
```


Obtiene el valor del componente rojo de esta instancia.


**Returns:**
int - El valor del componente rojo de esta instancia.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Obtiene el valor del componente verde de esta instancia.


**Returns:**
int - El valor del componente verde de esta instancia.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Obtiene el valor del componente azul de esta instancia.


**Returns:**
int - El valor del componente azul de esta instancia.

### toString() {#toString--}
```
public String toString()
```


Devuelve una  String  que representa el  Color  actual.


**Returns:**
java.lang.String - Una  String  que representa el  Color  actual.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
