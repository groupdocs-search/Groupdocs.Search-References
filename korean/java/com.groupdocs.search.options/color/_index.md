---
title: "Color"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "ARGB 알파 빨강 초록 파랑 색상을 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.options/color/
---
**Inheritance:**
java.lang.Object
```
public class Color
```

ARGB(알파, 빨강, 초록, 파랑) 색상을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Color(int alpha, int red, int green, int blue)](#Color-int-int-int-int-) | Color 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [Color(int red, int green, int blue)](#Color-int-int-int-) | Color 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [Color(Object data)](#Color-java.lang.Object-) | Color 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getAlpha()](#getAlpha--) | 이 인스턴스의 알파 구성 요소 값을 가져옵니다. |
|
|  | [getRed()](#getRed--) | 이 인스턴스의 빨간색 구성 요소 값을 가져옵니다. |
|
|  | [getGreen()](#getGreen--) | 이 인스턴스의 녹색 구성 요소 값을 가져옵니다. |
|
|  | [getBlue()](#getBlue--) | 이 인스턴스의 파란색 구성 요소 값을 가져옵니다. |
|
|  | [toString()](#toString--) | 현재  Color  를 나타내는  String  을 반환합니다. |
|
| [getCore()](#getCore--) |  |
### Color(int alpha, int red, int green, int blue) {#Color-int-int-int-int-}
```
public Color(int alpha, int red, int green, int blue)
```


Color 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 알파 | int | 0에서 255 사이의 알파 구성 요소. |
|
|  | 빨강 | int | 0에서 255 사이의 빨간색 구성 요소. |
|
|  | 녹색 | int | 0에서 255 사이의 녹색 구성 요소. |
|
|  | 파랑 | int | 0에서 255 사이의 파란색 구성 요소. |
|

### Color(int red, int green, int blue) {#Color-int-int-int-}
```
public Color(int red, int green, int blue)
```


Color 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 빨강 | int | 0에서 255 사이의 빨간색 구성 요소. |
|
|  | 녹색 | int | 0에서 255 사이의 녹색 구성 요소. |
|
|  | 파랑 | int | 0에서 255 사이의 파란색 구성 요소. |
|

### Color(Object data) {#Color-java.lang.Object-}
```
public Color(Object data)
```


Color 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getAlpha() {#getAlpha--}
```
public int getAlpha()
```


이 인스턴스의 알파 구성 요소 값을 가져옵니다.


**Returns:**
int - 이 인스턴스의 알파 구성 요소 값.

### getRed() {#getRed--}
```
public int getRed()
```


이 인스턴스의 빨간색 구성 요소 값을 가져옵니다.


**Returns:**
int - 이 인스턴스의 빨간색 구성 요소 값.

### getGreen() {#getGreen--}
```
public int getGreen()
```


이 인스턴스의 녹색 구성 요소 값을 가져옵니다.


**Returns:**
int - 이 인스턴스의 녹색 구성 요소 값.

### getBlue() {#getBlue--}
```
public int getBlue()
```


이 인스턴스의 파란색 구성 요소 값을 가져옵니다.


**Returns:**
int - 이 인스턴스의 파란색 구성 요소 값.

### toString() {#toString--}
```
public String toString()
```


현재  Color  를 나타내는  String  을 반환합니다.


**Returns:**
java.lang.String - 현재  Color  를 나타내는  String  입니다.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
