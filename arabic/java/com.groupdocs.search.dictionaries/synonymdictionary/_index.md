---
title: "SynonymDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس المرادفات."
type: docs
weight: 23
url: /ar/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

يحدد واجهة قاموس المرادفات.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الكلمات الموجودة في هذا SynonymDictionary. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | يضيف مجموعة المرادفات المحددة إلى هذه النسخة من SynonymDictionary. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | يضيف مجموعة المرادفات المحددة إلى هذه النسخة من SynonymDictionary. |
|
|  | [clear()](#clear--) | يزيل جميع الكلمات من كائن SynonymDictionary هذا. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | يحصل على المرادفات للكلمة المحددة. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | يحصل على جميع مجموعات المرادفات التي تنتمي إليها الكلمة المحددة. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | يحصل على جميع مجموعات المرادفات الموجودة في هذا القاموس. |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الكلمات الموجودة في هذا SynonymDictionary.


**Returns:**
int - عدد الكلمات الموجودة في هذا SynonymDictionary.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


يضيف مجموعة المرادفات المحددة إلى هذه النسخة من SynonymDictionary.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مرادفات | java.lang.Iterable<java.lang.String[]> | مجموعة من مجموعات المرادفات لإضافتها إلى القاموس. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


يضيف مجموعة المرادفات المحددة إلى هذه النسخة من SynonymDictionary.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مرادفات | java.lang.String[][] | مجموعة من مجموعات المرادفات لإضافتها إلى القاموس. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع الكلمات من كائن SynonymDictionary هذا.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


يحصل على المرادفات للكلمة المحددة. المصفوفة الناتجة لا تحتوي على الكلمة الأصلية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة للحصول على المرادفات. |
|

**Returns:**
java.lang.String[] - المرادفات للكلمة المحددة أو مصفوفة فارغة إذا كان كائن SynonymDictionary لا يحتوي على الكلمة المحددة.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


يحصل على جميع مجموعات المرادفات التي تنتمي إليها الكلمة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة للحصول على مجموعات المرادفات. |
|

**Returns:**
java.lang.String[][] - جميع مجموعات المرادفات التي تنتمي إليها الكلمة المحددة.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


يحصل على جميع مجموعات المرادفات الموجودة في هذا القاموس.


**Returns:**
java.lang.String[][] - جميع مجموعات المرادفات.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.String> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

