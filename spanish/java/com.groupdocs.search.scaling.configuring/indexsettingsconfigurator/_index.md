---
title: "IndexSettingsConfigurator"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el configurador de ajustes del índice para cada fragmento en la red de búsqueda."
type: docs
weight: 12
url: /es/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

Representa el configurador de ajustes del índice para cada fragmento en la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Establece la bandera de uso de palabras vacías. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Establece la bandera de uso de reemplazos de caracteres. |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | Establece la configuración de almacenamiento de texto. |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | Establece el tipo de índice. |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Establece el número de hilos de búsqueda. |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | Completa la configuración de los ajustes del índice. |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


Establece la bandera de uso de palabras vacías.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | El valor de la bandera. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


Establece la bandera de uso de reemplazos de caracteres.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | El valor de la bandera. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


Establece la configuración de almacenamiento de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | seUsa | boolean | La bandera de uso del almacenamiento de texto en el índice. |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | El nivel de compresión. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


Establece el tipo de índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | El tipo de índice. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


Establece el número de hilos de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | El número de hilos de búsqueda. |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


Completa la configuración de los ajustes del índice.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

