---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt den Konfigurator für Indexeinstellungen jedes Shards im Suchnetzwerk dar."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

Stellt den Konfigurator für Indexeinstellungen jedes Shards im Suchnetzwerk dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Setzt das Flag für die Verwendung von Stoppwörtern. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Setzt das Flag für die Verwendung von Zeichenersetzungen. |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | Setzt die Einstellungen für die Textspeicherung. |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | Setzt den Index-Typ. |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Setzt die Anzahl der Such-Threads. |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | Vollständigt die Konfiguration der Indexeinstellungen. |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


Setzt das Flag für die Verwendung von Stoppwörtern.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Der Flag-Wert. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


Setzt das Flag für die Verwendung von Zeichenersetzungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Der Flag-Wert. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


Setzt die Einstellungen für die Textspeicherung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | isUsed | boolean | Das Flag für die Verwendung des Textspeichers im Index. |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Die Komprimierungsstufe. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


Setzt den Index-Typ.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | Der Indextyp. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


Setzt die Anzahl der Such-Threads.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Die Anzahl der Such-Threads. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


Vollständigt die Konfiguration der Indexeinstellungen.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

