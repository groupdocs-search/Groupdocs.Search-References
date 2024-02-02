---
title: IndexSettingsConfigurator
second_title: GroupDocs.Search for Java API Reference
description: Represents the index settings configurator for each shard in the search network.
type: docs
weight: 12
url: /java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

Represents the index settings configurator for each shard in the search network.
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## Methods

| Method | Description |
| --- | --- |
| [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Sets the use stop words flag. |
| [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Sets the use character replacements flag. |
| [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | Sets the text storage settings. |
| [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | Sets the index type. |
| [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Sets the number of search threads. |
| [completeIndexSettings()](#completeIndexSettings--) | Completes the configuration of the index settings. |
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


Sets the use stop words flag.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag value. |

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


Sets the use character replacements flag.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag value. |

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


Sets the text storage settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isUsed | boolean | The flag of using the text storage in index. |
| compression | [Compression](../../com.groupdocs.search.options/compression) | The compression level. |

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


Sets the index type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexType | [IndexType](../../com.groupdocs.search.options/indextype) | The index type. |

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


Sets the number of search threads.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | The number of search threads. |

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.
### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


Completes the configuration of the index settings.

**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.
