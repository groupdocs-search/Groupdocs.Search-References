---
title: "Indexer"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل خدمة تدير توزيع المستندات المفهرسة عبر شظايا شبكة البحث."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

يمثل خدمة تدير توزيع المستندات المفهرسة عبر شظايا شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | ينفذ عملية الفهرسة. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | يحذف المستندات المفهرسة. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | يقلل عدد مقاطع الفهرس بدمجها واحدة مع الأخرى. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | يقوم بمزامنة قائمة المستندات المفهرسة مع تلك الموجودة على الشرائح. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | يطبق دفعة التغييرات المحددة للسمات على المستندات المفهرسة دون إعادة الفهرسة. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | يحصل على القاموس من الشريحة المحددة. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | يحصل على قاموس الأبجدية. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | يحصل على قاموس الأسماء المستعارة. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | يحصل على قاموس استبدال الأحرف. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | يحصل على قاموس المرادفات. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | يحصل على قاموس المتجانسات الصوتية. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | يحصل على قاموس مصحح الإملاء. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | يحصل على قاموس الكلمات الوقفية. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | يحصل على قاموس كلمات المرور. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | يضبط قاموسًا في الشريحة المحددة. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | يضبط قاموسًا في جميع الشرائح. |
|
|  | [deleteAllData()](#deleteAllData--) | يحذف جميع البيانات المفهرسة من جميع شرائح شبكة البحث. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


يقوم بعملية فهرسة. يدعم الفهرسة فقط من التدفق والبنية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | المستندات من نظام الملفات أو التدفق أو البنية. |
|
|  | كلمات المرور | java.lang.String[] | كلمات مرور المستند. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الإضافة. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


ينفذ عملية الفهرسة. يضيف البيانات المستخرجة إلى شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | البيانات المستخرجة. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | خيارات الفهرسة. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


يحذف المستندات المفهرسة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | مفاتيح المستندات المضافة من التدفقات أو الهياكل. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | خيارات الحذف. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


يقلل عدد مقاطع الفهرس عن طريق دمجها واحدة مع الأخرى. هذه العملية تحسن أداء البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | خيارات التحسين. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


يقوم بمزامنة قائمة المستندات المفهرسة مع تلك الموجودة على الشرائح. هذه العملية تصلح المشكلات المتعلقة بالفهرسة وحذف المستندات التي نتجت عن مشاكل التواصل مع عقد شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | خيارات المزامنة. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


يطبق دفعة التغييرات المحددة للسمات على المستندات المفهرسة دون إعادة الفهرسة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | دفعة تغيير السمة. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | خيارات تغيير السمات. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


يحصل على جميع السمات المرتبطة بالمستند المفهرس المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentKey | java.lang.String | مفتاح المستند. |
|

**Returns:**
java.lang.String[] - السمات المرتبطة بالمستند المفهرس المحدد.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


يحصل على القاموس من الشريحة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | نوع القاموس. |
|
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


يحصل على قاموس الأبجدية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


يحصل على قاموس الأسماء المستعارة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


يحصل على قاموس استبدال الأحرف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


يحصل على قاموس المرادفات.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


يحصل على قاموس المتجانسات الصوتية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


يحصل على قاموس مصحح الإملاء.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


يحصل على قاموس الكلمات الوقفية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


يحصل على قاموس كلمات المرور.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


يضبط قاموسًا في الشريحة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | القاموس. |
|
|  | shardIndex | int | فهرس الشريحة. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


يضبط قاموسًا في جميع الشرائح.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | القاموس. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


يحذف جميع البيانات المفهرسة من جميع شرائح شبكة البحث.


