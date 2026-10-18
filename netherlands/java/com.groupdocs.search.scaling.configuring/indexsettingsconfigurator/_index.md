---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de indexinstellingenconfigurator voor elke shard in het zoeknetwerk voor."
type: docs
weight: 12
url: /nl/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

Stelt de indexinstellingenconfigurator voor elke shard in het zoeknetwerk voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Stelt de vlag voor het gebruik van stopwoorden in. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Stelt de vlag voor het gebruik van tekenvervangingen in. |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | Stelt de tekstopslaginstellingen in. |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | Stelt het indextype in. |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Stelt het aantal zoekthreads in. |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | Rondt de configuratie van de indexinstellingen af. |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


Stelt de vlag voor het gebruik van stopwoorden in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlagwaarde. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


Stelt de vlag voor het gebruik van tekenvervangingen in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlagwaarde. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


Stelt de tekstopslaginstellingen in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | isUsed | boolean | De vlag voor het gebruik van de tekstopslag in de index. |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Het compressieniveau. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


Stelt het indextype in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | Het type index. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


Stelt het aantal zoekthreads in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Het aantal zoekthreads. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


Rondt de configuratie van de indexinstellingen af.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

