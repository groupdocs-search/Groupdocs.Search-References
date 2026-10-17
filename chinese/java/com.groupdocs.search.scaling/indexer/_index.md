---
title: "Indexer"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示管理已索引文档在搜索网络分片之间分配的服务。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

表示管理已索引文档在搜索网络分片之间分配的服务。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | 执行索引操作。 |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | 删除已索引的文档。 |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | 通过将它们相互合并来最小化索引段的数量。 |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | 将已索引文档的列表与分片上的文档同步。 |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | 在不重新索引的情况下，将指定批次的属性更改应用于已索引的文档。 |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | 获取与指定已索引文档关联的所有属性。 |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | 从指定的分片获取字典。 |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | 获取字母表字典。 |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | 获取别名字典。 |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | 获取字符替换字典。 |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | 获取同义词字典。 |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | 获取同音字字典。 |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | 获取拼写纠正字典。 |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | 获取停用词字典。 |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | 获取密码字典。 |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | 在指定的分片中设置字典。 |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | 在所有分片中设置字典。 |
|
|  | [deleteAllData()](#deleteAllData--) | 删除搜索网络中所有分片的所有已索引数据。 |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


执行索引操作。仅支持来自流和结构的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | 来自文件系统、流或结构的文档。 |
|
|  | 密码 | java.lang.String[] | 文档密码。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 添加选项。 |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


执行索引操作。将提取的数据添加到搜索网络。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 提取的数据。 |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 索引选项。 |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


删除已索引的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | 从流或结构中添加的文档的键。 |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | 删除选项。 |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


通过将索引段相互合并来最小化索引段的数量。此操作可提升搜索性能。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | 优化选项。 |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


同步已索引文档列表与分片上的文档。此操作修复因与搜索网络节点通信问题导致的文档索引和删除问题。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | 同步选项。 |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


在不重新索引的情况下，将指定批次的属性更改应用于已索引的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 属性更改批次。 |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | 更改属性选项。 |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


获取与指定已索引文档关联的所有属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文档键 | java.lang.String | 文档键。 |
|

**Returns:**
java.lang.String[] - 与指定已索引文档关联的属性。

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


从指定的分片获取字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | 字典类型。 |
|
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


获取字母表字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


获取别名字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


获取字符替换字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


获取同义词字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


获取同音字字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


获取拼写纠正字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


获取停用词字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


获取密码字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | shardIndex | int | 分片索引。 |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


在指定的分片中设置字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 字典。 |
|
|  | shardIndex | int | 分片索引。 |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


在所有分片中设置字典。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 字典。 |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


删除搜索网络中所有分片的所有已索引数据。


