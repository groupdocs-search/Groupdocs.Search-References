---
title: "Color"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет цвет ARGB (альфа, красный, зелёный, синий)."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

Представляет цвет ARGB (альфа, красный, зеленый, синий).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Создает новый экземпляр класса Color. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Создает новый экземпляр класса Color. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Создает новый экземпляр класса Color. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | Получает значение альфа‑компоненты этого экземпляра. |
|
|  | [getRed()](#getRed--) | Получает значение красного компонента этого экземпляра. |
|
|  | [getGreen()](#getGreen--) | Получает значение зелёного компонента этого экземпляра. |
|
|  | [getBlue()](#getBlue--) | Получает значение синего компонента этого экземпляра. |
|
|  | [toString()](#toString--) | Возвращает  String  который представляет текущий  Color . |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Создает новый экземпляр класса Color.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | alpha | int | Альфа‑компонент от 0 до 255. |
|
|  | red | int | Красный компонент от 0 до 255. |
|
|  | green | int | Зелёный компонент от 0 до 255. |
|
|  | blue | int | Синий компонент от 0 до 255. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Создает новый экземпляр класса Color.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | red | int | Красный компонент от 0 до 255. |
|
|  | green | int | Зелёный компонент от 0 до 255. |
|
|  | blue | int | Синий компонент от 0 до 255. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Создает новый экземпляр класса Color.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


Получает значение альфа‑компоненты этого экземпляра.


**Returns:**
int - Значение альфа‑компонента этого экземпляра.

### getRed() {#getRed--}
```
public int getRed()
```


Получает значение красного компонента этого экземпляра.


**Returns:**
int - Значение красного компонента этого экземпляра.

### getGreen() {#getGreen--}
```
public int getGreen()
```


Получает значение зелёного компонента этого экземпляра.


**Returns:**
int - Значение зелёного компонента этого экземпляра.

### getBlue() {#getBlue--}
```
public int getBlue()
```


Получает значение синего компонента этого экземпляра.


**Returns:**
int - Значение синего компонента этого экземпляра.

### toString() {#toString--}
```
public String toString()
```


Возвращает  String  который представляет текущий  Color .


**Returns:**
java.lang.String -  String  который представляет текущий  Color .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
