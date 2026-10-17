---
title: "Color"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une couleur ARGB alpha rouge vert bleu."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Représente une couleur ARGB (alpha, rouge, vert, bleu).

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Initialise une nouvelle instance de la classe  Color . |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Initialise une nouvelle instance de la classe  Color . |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Initialise une nouvelle instance de la classe  Color . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Obtient la valeur du composant alpha de cette instance. |
|
|  | [getRed()](#getRed--) | Obtient la valeur du composant rouge de cette instance. |
|
|  | [getGreen()](#getGreen--) | Obtient la valeur du composant vert de cette instance. |
|
|  | [getBlue()](#getBlue--) | Obtient la valeur du composant bleu de cette instance. |
|
|  | [toString()](#toString--) | Renvoie une String qui représente la Color actuelle. |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Initialise une nouvelle instance de la classe  Color .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | alpha | int | Le composant alpha de 0 à 255. |
|
|  | rouge | int | Le composant rouge de 0 à 255. |
|
|  | vert | int | Le composant vert de 0 à 255. |
|
|  | bleu | int | Le composant bleu de 0 à 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Initialise une nouvelle instance de la classe  Color .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | rouge | int | Le composant rouge de 0 à 255. |
|
|  | vert | int | Le composant vert de 0 à 255. |
|
|  | bleu | int | Le composant bleu de 0 à 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Initialise une nouvelle instance de la classe  Color .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Obtient la valeur du composant alpha de cette instance.


**Returns:**
int - La valeur du composant alpha de cette instance.

### getRed() {#getRed--}
```
public int getRed()
```


Obtient la valeur du composant rouge de cette instance.


**Returns:**
int - La valeur du composant rouge de cette instance.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Obtient la valeur du composant vert de cette instance.


**Returns:**
int - La valeur du composant vert de cette instance.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Obtient la valeur du composant bleu de cette instance.


**Returns:**
int - La valeur du composant bleu de cette instance.

### toString() {#toString--}
```
public String toString()
```


Renvoie une String qui représente la Color actuelle.


**Returns:**
java.lang.String - Une String qui représente la Color actuelle.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
