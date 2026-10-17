---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络中每个分片的索引设置配置器。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

表示搜索网络中每个分片的索引设置配置器。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | 设置使用停用词标志。 |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | 设置使用字符替换标志。 |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | 设置文本存储设置。 |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | 设置索引类型。 |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | 设置搜索线程数。 |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | 完成索引设置的配置。 |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


设置使用停用词标志。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 标志值。 |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


设置使用字符替换标志。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 标志值。 |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


设置文本存储设置。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | isUsed | boolean | 在索引中使用文本存储的标志。 |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | 压缩级别。 |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


设置索引类型。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | 索引类型。 |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


设置搜索线程数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | 搜索线程的数量。 |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


完成索引设置的配置。


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

