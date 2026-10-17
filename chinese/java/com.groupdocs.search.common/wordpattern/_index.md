---
title: "WordPattern"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示用于单词通配符搜索的单词模式。"
type: docs
weight: 34
url: /zh/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

表示用于单词通配符搜索的单词模式。


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | 初始化 WordPattern 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | 向单词模式追加字符串。 |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | 向单词模式追加字符。 |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | 向单词模式追加单字符通配符。 |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | 向单词模式追加零或一个字符的通配符。 |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | 向单词模式追加零个或多个字符的通配符。 |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | 向单词模式追加一个或多个字符的通配符。 |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | 向单词模式追加通配符。 |
|
|  | [toString()](#toString--) | 返回一个 System.String，表示当前的 WordPattern。 |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


初始化 WordPattern 类的新实例。


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


向单词模式追加字符串。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文本 | java.lang.String | 要追加的字符串。 |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


向单词模式追加字符。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char | 要追加的字符。 |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


向单词模式追加单字符通配符。


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


向单词模式追加零或一个字符的通配符。


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


向单词模式追加零个或多个字符的通配符。


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


向单词模式追加一个或多个字符的通配符。


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


向单词模式追加通配符。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 最小 | int | 字符的最小数量。 |
|
|  | 最大 | int | 字符的最大数量。 |
|

### toString() {#toString--}
```
public String toString()
```


返回一个 System.String，表示当前的 WordPattern。


**Returns:**
java.lang.String - 一个 System.String，表示当前的 WordPattern。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
