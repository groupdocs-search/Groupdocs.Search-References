---
title: "Dizinleyici"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağının parçaları arasında indekslenmiş belgelerin dağıtımını yöneten bir hizmeti temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Arama ağının parçaları arasında indekslenmiş belgelerin dağıtımını yöneten bir hizmeti temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Dizinleme işlemini gerçekleştirir. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | İndekslenmiş belgeleri siler. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Dizin segmentlerinin sayısını birbiriyle birleştirerek azaltır. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | İndekslenmiş belgelerin listesini parçalar üzerindekilerle senkronize eder. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | İndekslenmiş belgelere yeniden indekslemeden belirtilen öznitelik değişiklikleri topluluğunu uygular. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Belirtilen indekslenmiş belgeyle ilişkili tüm öznitelikleri alır. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Belirtilen parçadan bir sözlük alır. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Alfabe sözlüğünü alır. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Takma ad sözlüğünü alır. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Karakter değiştirme sözlüğünü alır. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Eşanlamlı sözlüğünü alır. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Eşsesli sözlüğünü alır. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Yazım düzeltici sözlüğünü alır. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Durdurma kelimeleri sözlüğünü alır. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Parola sözlüğünü alır. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Belirtilen parçaya bir sözlük ayarlar. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Tüm parçalara bir sözlük ayarlar. |
|
|  | [deleteAllData()](#deleteAllData--) | Arama ağının tüm parçalarındaki tüm indekslenmiş verileri siler. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


İndeksleme işlemi gerçekleştirir. Yalnızca akış ve yapıdan indeksleme desteklenir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dosya sisteminden, akıştan veya yapıdan gelen belgeler. |
|
|  | parolalar | java.lang.String[] | Belge şifreleri. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Ekleme seçenekleri. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Dizinleme işlemi gerçekleştirir. Çıkarılan verileri arama ağına ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Çıkarılan veri. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Dizinleme seçenekleri. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


İndekslenmiş belgeleri siler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Akışlardan veya yapılardan eklenen belgelerin anahtarları. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Silme seçenekleri. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Dizin segmentlerinin sayısını birbiriyle birleştirerek en aza indirir. Bu işlem arama performansını artırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Optimizasyon seçenekleri. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Dizinlenmiş belgelerin listesini parçalar üzerindekilerle senkronize eder. Bu işlem, arama ağı düğümleriyle iletişim sorunlarından kaynaklanan indeksleme ve belge silme problemlerini düzeltir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Senkronizasyon seçenekleri. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


İndekslenmiş belgelere yeniden indekslemeden belirtilen öznitelik değişiklikleri topluluğunu uygular.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Özellik değişim paketi. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Özellikleri değiştirme seçenekleri. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Belirtilen indekslenmiş belgeyle ilişkili tüm öznitelikleri alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentKey | java.lang.String | Belgenin anahtarı. |
|

**Returns:**
java.lang.String[] - Belirtilen dizinlenmiş belgeyle ilişkili özellikler.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Belirtilen parçadan bir sözlük alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Sözlük türü. |
|
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Alfabe sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Takma ad sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Karakter değiştirme sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Eşanlamlı sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Eşsesli sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Yazım düzeltici sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Durdurma kelimeleri sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Parola sözlüğünü alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Belirtilen parçaya bir sözlük ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Sözlük. |
|
|  | shardIndex | int | Parça indeksi. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Tüm parçalara bir sözlük ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Sözlük. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Arama ağının tüm parçalarındaki tüm indekslenmiş verileri siler.


