---
title: "Indexer"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un servicio que gestiona la distribución de documentos indexados entre fragmentos de la red de búsqueda."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Representa un servicio que gestiona la distribución de documentos indexados entre fragmentos de la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Realiza la operación de indexación. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Elimina documentos indexados. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Minimiza el número de segmentos del índice fusionándolos uno con otro. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Sincroniza la lista de documentos indexados con los de los fragmentos. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Aplica el lote especificado de cambios de atributos a los documentos indexados sin reindexar. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Obtiene todos los atributos asociados con el documento indexado especificado. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Obtiene un diccionario del fragmento especificado. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Obtiene el diccionario alfabético. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Obtiene el diccionario de alias. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Obtiene el diccionario de sustitución de caracteres. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Obtiene el diccionario de sinónimos. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Obtiene el diccionario de homófonos. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Obtiene el diccionario del corrector ortográfico. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Obtiene el diccionario de palabras vacías. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Obtiene el diccionario de contraseñas. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Establece un diccionario en el fragmento especificado. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Establece un diccionario en todos los fragmentos. |
|
|  | [deleteAllData()](#deleteAllData--) | Elimina todos los datos indexados de todos los fragmentos de la red de búsqueda. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Realiza una operación de indexación. Sólo se admite la indexación desde flujo y estructura.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Los documentos del sistema de archivos, flujo o estructura. |
|
|  | contraseñas | java.lang.String[] | Las contraseñas del documento. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de agregar. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Realiza una operación de indexación. Añade los datos extraídos a la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Los datos extraídos. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones de indexación. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Elimina documentos indexados.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Las claves de los documentos añadidos desde flujos o estructuras. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Las opciones de eliminación. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimiza el número de segmentos de índice fusionándolos uno con otro. Esta operación mejora el rendimiento de la búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Las opciones de optimización. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Sincroniza la lista de documentos indexados con los de los fragmentos. Esta operación corrige problemas de indexación y eliminación de documentos que resultaron de problemas de comunicación con los nodos de la red de búsqueda.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Las opciones de sincronización. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Aplica el lote especificado de cambios de atributos a los documentos indexados sin reindexar.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | El lote de cambios de atributos. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Las opciones de cambio de atributos. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Obtiene todos los atributos asociados con el documento indexado especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clave del documento. |
|

**Returns:**
java.lang.String[] - Los atributos asociados con el documento indexado especificado.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Obtiene un diccionario del fragmento especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | El tipo de diccionario. |
|
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Obtiene el diccionario alfabético.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Obtiene el diccionario de alias.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Obtiene el diccionario de sustitución de caracteres.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Obtiene el diccionario de sinónimos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Obtiene el diccionario de homófonos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Obtiene el diccionario del corrector ortográfico.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Obtiene el diccionario de palabras vacías.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Obtiene el diccionario de contraseñas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | shardIndex | int | El índice del fragmento. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Establece un diccionario en el fragmento especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | El diccionario. |
|
|  | shardIndex | int | El índice del fragmento. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Establece un diccionario en todos los fragmentos.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | El diccionario. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Elimina todos los datos indexados de todos los fragmentos de la red de búsqueda.


