---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il configuratore delle impostazioni dell'indice per ogni shard nella rete di ricerca."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

Rappresenta il configuratore delle impostazioni dell'indice per ogni shard nella rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Imposta il flag di utilizzo delle parole di stop. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Imposta il flag di utilizzo delle sostituzioni dei caratteri. |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | Imposta le impostazioni di archiviazione del testo. |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | Imposta il tipo di indice. |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Imposta il numero di thread di ricerca. |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | Completa la configurazione delle impostazioni dell'indice. |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


Imposta il flag di utilizzo delle parole di stop.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il valore del flag. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


Imposta il flag di utilizzo delle sostituzioni dei caratteri.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il valore del flag. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


Imposta le impostazioni di archiviazione del testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | isUsed | boolean | Il flag per l'uso dell'archiviazione del testo nell'indice. |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Il livello di compressione. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


Imposta il tipo di indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | Il tipo di indice. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


Imposta il numero di thread di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Il numero di thread di ricerca. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


Completa la configurazione delle impostazioni dell'indice.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

