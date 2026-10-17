---
title: "Color"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示 ARGB（alpha、red、green、blue）颜色。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

表示 ARGB（alpha、red、green、blue）颜色。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | 初始化 Color 类的新实例。 |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | 初始化 Color 类的新实例。 |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | 初始化 Color 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | 获取此实例的 alpha 组件值。 |
|
|  | [getRed()](#getRed--) | 获取此实例的红色分量值。 |
|
|  | [getGreen()](#getGreen--) | 获取此实例的绿色分量值。 |
|
|  | [getBlue()](#getBlue--) | 获取此实例的蓝色分量值。 |
|
|  | [toString()](#toString--) | 返回一个  String ，表示当前的  Color 。 |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


初始化 Color 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | alpha | int | alpha 分量的取值范围为 0 到 255。 |
|
|  | red | int | red 分量的取值范围为 0 到 255。 |
|
|  | green | int | green 分量的取值范围为 0 到 255。 |
|
|  | blue | int | blue 分量的取值范围为 0 到 255。 |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


初始化 Color 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | red | int | red 分量的取值范围为 0 到 255。 |
|
|  | green | int | green 分量的取值范围为 0 到 255。 |
|
|  | blue | int | blue 分量的取值范围为 0 到 255。 |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


初始化 Color 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


获取此实例的 alpha 组件值。


**Returns:**
int - 此实例的 alpha 分量值。

### getRed() {#getRed--}
```
public int getRed()
```


获取此实例的红色分量值。


**Returns:**
int - 此实例的 red 分量值。

### getGreen() {#getGreen--}
```
public int getGreen()
```


获取此实例的绿色分量值。


**Returns:**
int - 此实例的 green 分量值。

### getBlue() {#getBlue--}
```
public int getBlue()
```


获取此实例的蓝色分量值。


**Returns:**
int - 此实例的 blue 分量值。

### toString() {#toString--}
```
public String toString()
```


返回一个  String ，表示当前的  Color 。


**Returns:**
java.lang.String - 一个  String ，表示当前的  Color 。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
