---
title: "HomophoneDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس المتجانسات الهجائية."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

يحدد واجهة قاموس المتجانسات الهجائية.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الكلمات الموجودة في هذا  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | يضيف مجموعة المحددة من مجموعات المتجانسات الصوتية إلى هذه النسخة من  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | يضيف مجموعة المحددة من مجموعات المتجانسات الصوتية إلى هذه النسخة من  HomophoneDictionary . |
|
|  | [clear()](#clear--) | يزيل جميع الكلمات من كائن  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | يحصل على المتجانسات الصوتية للكلمة المحددة. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | يحصل على جميع مجموعات المتجانسات الصوتية التي تنتمي إليها الكلمة المحددة. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | يحصل على جميع مجموعات المتجانسات الصوتية الموجودة في هذا القاموس. |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الكلمات الموجودة في هذا  HomophoneDictionary .


**Returns:**
int - عدد الكلمات.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


يضيف مجموعة المحددة من مجموعات المتجانسات الصوتية إلى هذه النسخة من  HomophoneDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المتجانسات الصوتية | java.lang.Iterable<java.lang.String[]> | المجموعة من مجموعات المتجانسات الصوتية لإضافتها إلى القاموس. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


يضيف مجموعة المحددة من مجموعات المتجانسات الصوتية إلى هذه النسخة من  HomophoneDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المتجانسات الصوتية | java.lang.String[][] | المجموعة من مجموعات المتجانسات الصوتية لإضافتها إلى القاموس. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع الكلمات من كائن  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


يحصل على المتجانسات الصوتية للكلمة المحددة. المصفوفة الناتجة لا تحتوي على الكلمة الأصلية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة لاقتراح المتجانسات الصوتية. |
|

**Returns:**
java.lang.String[] - المتجانسات الصوتية للكلمة المحددة أو مصفوفة فارغة إذا كان كائن  HomophoneDictionary  لا يحتوي على الكلمة المحددة.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


يحصل على جميع مجموعات المتجانسات الصوتية التي تنتمي إليها الكلمة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة للحصول على مجموعات المتجانسات الصوتية. |
|

**Returns:**
java.lang.String[][] - جميع مجموعات المتجانسات الصوتية التي تنتمي إليها الكلمة المحددة.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


يحصل على جميع مجموعات المتجانسات الصوتية الموجودة في هذا القاموس.


**Returns:**
java.lang.String[][] - جميع مجموعات المتجانسات الصوتية.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.String> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

