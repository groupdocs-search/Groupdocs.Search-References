---
title: "HighlightOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供突出显示已找到术语的选项。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

提供突出显示已找到术语的选项。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | 初始化 HighlightOptions 类的新实例。 |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | 初始化 TextOptions 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | 获取高亮词之前的文本片段中最大单词数。 |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | 设置高亮词之前的文本片段中最大单词数。 |
|
|  | [getTermsAfter()](#getTermsAfter--) | 获取高亮词之后的文本片段中最大单词数。 |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | 设置高亮词之后的文本片段中最大单词数。 |
|
|  | [getTermsTotal()](#getTermsTotal--) | 获取文本片段中的最大单词数。 |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | 设置文本片段中的最大单词数。 |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | 获取指示是否使用内联样式来高亮出现位置的值。 |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | 设置指示是否使用内联样式来高亮出现位置的值。 |
|
|  | [getHighlightColor()](#getHighlightColor--) | 获取用于高亮出现位置的颜色。 |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | 设置用于高亮出现的颜色。 |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | 获取已找到单词的高亮起始标签。 |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | 设置已找到单词的高亮起始标签。 |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | 获取已找到单词的高亮结束标签。 |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | 设置已找到单词的高亮结束标签。 |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


初始化 HighlightOptions 类的新实例。


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


初始化 TextOptions 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


获取高亮词之前的文本片段中最大单词数。该值必须在 0 到 10000 的范围内。默认值为 7。


**Returns:**
int - 高亮词之前的文本片段中最大单词数。

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


设置高亮词之前的文本片段中最大单词数。该值必须在 0 到 10000 的范围内。默认值为 7。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 高亮词之前的文本片段中最大单词数。 |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


获取高亮词之后的文本片段中最大单词数。该值必须在 0 到 10000 的范围内。默认值为 7。


**Returns:**
int - 高亮词之后的文本片段中最大单词数。

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


设置高亮词之后的文本片段中最大单词数。该值必须在 0 到 10000 的范围内。默认值为 7。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 高亮词之后的文本片段中最大单词数。 |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


获取文本片段中的最大单词数。该值必须在 0 到 10000 的范围内。默认值为 21。


**Returns:**
int - 文本片段中的最大单词数。

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


设置文本片段中的最大单词数。该值必须在 0 到 10000 的范围内。默认值为 21。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 文本片段中的最大单词数。 |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


获取指示是否使用内联样式来高亮出现的值。默认值为 true。


**Returns:**
boolean - 指示是否使用内联样式来高亮出现的值。

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


设置指示是否使用内联样式来高亮出现的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否使用内联样式来高亮出现的值。 |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


获取用于高亮出现的颜色。默认值为 #FFD800。


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


设置用于高亮出现的颜色。默认值为 #FFD800。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | 用于突出显示出现位置的颜色。 |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


获取找到的单词高亮显示的起始标签。此标签仅在纯文本高亮时使用。默认值为空字符串。


**Returns:**
java.lang.String - 找到的单词高亮显示的起始标签。

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


设置找到的单词高亮显示的起始标签。此标签仅在纯文本高亮时使用。默认值为空字符串。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 找到的单词高亮显示的起始标签。 |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


获取找到的单词高亮显示的结束标签。此标签仅在纯文本高亮时使用。默认值为空字符串。


**Returns:**
java.lang.String - 找到的单词高亮显示的结束标签。

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


设置找到的单词高亮显示的结束标签。此标签仅在纯文本高亮时使用。默认值为空字符串。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 找到的单词高亮显示的结束标签。 |
|

