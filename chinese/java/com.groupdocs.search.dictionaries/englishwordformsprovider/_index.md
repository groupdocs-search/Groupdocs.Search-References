---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示英文词形提供程序。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

表示英文词形提供程序。


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | 初始化一个新的实例 |
EnglishWordFormsProvider
类。
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | 获取指定词的词形。 |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


初始化一个新的实例
EnglishWordFormsProvider
类。


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


获取指定词的词形。
结果数组不包含原始词。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 用于建议词形的词。 |
|

**Returns:**
java.lang.String[] - 指定词的词形，若 IWordFormsProvider 未提供该词的词形，则返回空数组。

