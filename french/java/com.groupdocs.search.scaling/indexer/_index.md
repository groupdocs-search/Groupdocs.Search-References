---
title: "Indexer"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un service qui gère la distribution des documents indexés à travers les shards du réseau de recherche."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Représente un service qui gère la distribution des documents indexés à travers les shards du réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Effectue l'opération d'indexation. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Supprime les documents indexés. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Synchronise la liste des documents indexés avec ceux des segments. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Obtient tous les attributs associés au document indexé spécifié. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Obtient un dictionnaire à partir du segment spécifié. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Obtient le dictionnaire de l'alphabet. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Obtient le dictionnaire d'alias. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Obtient le dictionnaire de remplacement de caractères. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Obtient le dictionnaire des synonymes. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Obtient le dictionnaire des homophones. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Obtient le dictionnaire du correcteur orthographique. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Obtient le dictionnaire des mots vides. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Obtient le dictionnaire de mots de passe. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Définit un dictionnaire dans la partition spécifiée. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Définit un dictionnaire dans toutes les partitions. |
|
|  | [deleteAllData()](#deleteAllData--) | Supprime toutes les données indexées de toutes les partitions du réseau de recherche. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Effectue une opération d'indexation. L'indexation uniquement à partir du flux et de la structure est prise en charge.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Les documents provenant du système de fichiers, du flux ou de la structure. |
|
|  | mots de passe | java.lang.String[] | Les mots de passe du document. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'ajout. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Effectue une opération d'indexation. Ajoute les données extraites au réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Les données extraites. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options d'indexation. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Supprime les documents indexés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Les clés des documents ajoutés à partir de flux ou de structures. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Les options de suppression. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimise le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Les options d'optimisation. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Synchronise la liste des documents indexés avec ceux des partitions. Cette opération résout les problèmes d'indexation et de suppression de documents résultant de problèmes de communication avec les nœuds du réseau de recherche.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Les options de synchronisation. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Applique le lot spécifié de modifications d'attributs aux documents indexés sans réindexation.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Le lot de modifications d'attributs. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Les options de modification des attributs. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Obtient tous les attributs associés au document indexé spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | documentKey | java.lang.String | La clé du document. |
|

**Returns:**
java.lang.String[] - Les attributs associés au document indexé spécifié.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Obtient un dictionnaire à partir du segment spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Le type de dictionnaire. |
|
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Obtient le dictionnaire de l'alphabet.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Obtient le dictionnaire d'alias.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Obtient le dictionnaire de remplacement de caractères.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Obtient le dictionnaire des synonymes.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Obtient le dictionnaire des homophones.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Obtient le dictionnaire du correcteur orthographique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Obtient le dictionnaire des mots vides.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Obtient le dictionnaire de mots de passe.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | shardIndex | int | L'index de partition. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Définit un dictionnaire dans la partition spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Le dictionnaire. |
|
|  | shardIndex | int | L'index de partition. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Définit un dictionnaire dans toutes les partitions.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Le dictionnaire. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Supprime toutes les données indexées de toutes les partitions du réseau de recherche.


