---
title: "AliasDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义别名字典的接口。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

定义别名字典的接口。


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取 AliasDictionary 中包含的别名数量。 |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | 向此 AliasDictionary 实例添加指定的别名/替换对集合。 |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | 向此 AliasDictionary 实例添加指定的别名/替换对集合。 |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | 向此 AliasDictionary 实例添加指定的别名及其关联文本对。 |
|
|  | [remove(String alias)](#remove-java.lang.String-) | 从 AliasDictionary 对象中移除指定的别名。 |
|
|  | [contains(String alias)](#contains-java.lang.String-) | 确定 AliasDictionary 对象是否包含指定的别名。 |
|
|  | [getText(String alias)](#getText-java.lang.String-) | 获取与指定别名关联的文本。 |
|
|  | [clear()](#clear--) | 从 AliasDictionary 对象中移除所有别名。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取 AliasDictionary 中包含的别名数量。


**Returns:**
int - AliasDictionary 中包含的别名数量。

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


向此 AliasDictionary 实例添加指定的别名/替换对集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 对 | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | 要添加到字典的别名/替换对集合。 |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


向此 AliasDictionary 实例添加指定的别名/替换对集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | 要添加到字典的别名/替换对集合。 |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


向此 AliasDictionary 实例添加指定的别名及其关联文本对。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 别名 | java.lang.String | 要添加到字典的别名。 |
|
|  | 文本 | java.lang.String | 要与别名关联的文本。 |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


从 AliasDictionary 对象中移除指定的别名。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 别名 | java.lang.String | 要移除的别名。 |
|

**Returns:**
boolean - 如果成功找到并删除别名，此方法返回  true ；如果在  AliasDictionary  对象中未找到别名，此方法返回  false  。

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


确定 AliasDictionary 对象是否包含指定的别名。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 别名 | java.lang.String | 要在  AliasDictionary  对象中定位的别名。 |
|

**Returns:**
boolean - 如果  AliasDictionary  对象包含指定的别名，则为  true ；否则为  false 。

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


获取与指定别名关联的文本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 别名 | java.lang.String | 要在  AliasDictionary  对象中定位的别名。 |
|

**Returns:**
java.lang.String - 与指定别名关联的文本，或为  null 。

### clear() {#clear--}
```
public abstract void clear()
```


从 AliasDictionary 对象中移除所有别名。


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.String> - 可用于遍历集合的迭代器。

