---
title: "HighlightOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "찾은 용어를 강조 표시하기 위한 옵션을 제공합니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

찾은 용어를 강조 표시하기 위한 옵션을 제공합니다.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | HighlightOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | TextOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | 하이라이트된 단어 앞의 텍스트 스니펫에서 최대 단어 수를 가져옵니다. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | 하이라이트된 단어 앞의 텍스트 스니펫에서 최대 단어 수를 설정합니다. |
|
|  | [getTermsAfter()](#getTermsAfter--) | 하이라이트된 단어 뒤의 텍스트 스니펫에서 최대 단어 수를 가져옵니다. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | 하이라이트된 단어 뒤의 텍스트 스니펫에서 최대 단어 수를 설정합니다. |
|
|  | [getTermsTotal()](#getTermsTotal--) | 텍스트 스니펫에서 최대 단어 수를 가져옵니다. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | 텍스트 스니펫에서 최대 단어 수를 설정합니다. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | 인라인 스타일을 사용하여 발생을 하이라이트하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | 인라인 스타일을 사용하여 발생을 하이라이트하는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getHighlightColor()](#getHighlightColor--) | 발생을 하이라이트하는 데 사용되는 색상을 가져옵니다. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | 발생을 강조 표시하는 데 사용되는 색상을 설정합니다. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | 찾은 단어의 강조 표시 시작 태그를 가져옵니다. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | 찾은 단어의 강조 표시 시작 태그를 설정합니다. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | 찾은 단어의 강조 표시 종료 태그를 가져옵니다. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | 찾은 단어의 강조 표시 종료 태그를 설정합니다. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


HighlightOptions 클래스의 새 인스턴스를 초기화합니다.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


TextOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


강조 표시된 단어 앞의 텍스트 스니펫에서 최대 단어 수를 가져옵니다. 값은 0에서 10000 사이여야 합니다. 기본값은 7입니다.


**Returns:**
int - 강조 표시된 단어 앞의 텍스트 스니펫에서 최대 단어 수.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


강조 표시된 단어 앞의 텍스트 스니펫에서 최대 단어 수를 설정합니다. 값은 0에서 10000 사이여야 합니다. 기본값은 7입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 강조 표시된 단어 앞의 텍스트 스니펫에서 최대 단어 수. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


강조 표시된 단어 뒤의 텍스트 스니펫에서 최대 단어 수를 가져옵니다. 값은 0에서 10000 사이여야 합니다. 기본값은 7입니다.


**Returns:**
int - 강조 표시된 단어 뒤의 텍스트 스니펫에서 최대 단어 수.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


강조 표시된 단어 뒤의 텍스트 스니펫에서 최대 단어 수를 설정합니다. 값은 0에서 10000 사이여야 합니다. 기본값은 7입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 강조 표시된 단어 뒤의 텍스트 스니펫에서 최대 단어 수. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


텍스트 스니펫에서 최대 단어 수를 가져옵니다. 값은 0에서 10000 사이여야 합니다. 기본값은 21입니다.


**Returns:**
int - 텍스트 스니펫에서 최대 단어 수.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


텍스트 스니펫에서 최대 단어 수를 설정합니다. 값은 0에서 10000 사이여야 합니다. 기본값은 21입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 텍스트 스니펫에서 최대 단어 수. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


발생을 강조 표시하는 데 인라인 스타일이 사용되는지 여부를 나타내는 값을 가져옵니다. 기본값은 true입니다.


**Returns:**
boolean - 발생을 강조 표시하는 데 인라인 스타일이 사용되는지 여부를 나타내는 값.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


발생을 강조 표시하는 데 인라인 스타일이 사용되는지 여부를 나타내는 값을 설정합니다. 기본값은 true입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 발생을 강조 표시하는 데 인라인 스타일이 사용되는지 여부를 나타내는 값. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


발생을 강조 표시하는 데 사용되는 색상을 가져옵니다. 기본값은 #FFD800입니다.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


발생을 강조 표시하는 데 사용되는 색상을 설정합니다. 기본값은 #FFD800입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | 발생을 강조하는 데 사용되는 색상입니다. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


찾은 단어의 강조 시작 태그를 가져옵니다. 이 태그는 일반 텍스트에서 강조할 때만 사용됩니다. 기본값은 빈 문자열입니다.


**Returns:**
java.lang.String - 찾은 단어의 강조 시작 태그.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


찾은 단어의 강조 시작 태그를 설정합니다. 이 태그는 일반 텍스트에서 강조할 때만 사용됩니다. 기본값은 빈 문자열입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 찾은 단어의 강조 시작 태그. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


찾은 단어의 강조 종료 태그를 가져옵니다. 이 태그는 일반 텍스트에서 강조할 때만 사용됩니다. 기본값은 빈 문자열입니다.


**Returns:**
java.lang.String - 찾은 단어의 강조 종료 태그.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


찾은 단어의 강조 종료 태그를 설정합니다. 이 태그는 일반 텍스트에서 강조할 때만 사용됩니다. 기본값은 빈 문자열입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 찾은 단어의 강조 종료 태그. |
|

