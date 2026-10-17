---
title: "AliasDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس الأسماء المستعارة."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

يحدد واجهة قاموس الأسماء المستعارة.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الأسماء المستعارة الموجودة في AliasDictionary . |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | يضيف مجموعة أزواج الاسم المستعار/البديل المحددة إلى هذه المثيلة من AliasDictionary . |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | يضيف مجموعة أزواج الاسم المستعار/البديل المحددة إلى هذه المثيلة من AliasDictionary . |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | يضيف الزوج المحدد من الاسم المستعار والنص المرتبط إلى هذه المثيلة من AliasDictionary . |
|
|  | [remove(String alias)](#remove-java.lang.String-) | يزيل الاسم المستعار المحدد من كائن AliasDictionary . |
|
|  | [contains(String alias)](#contains-java.lang.String-) | يحدد ما إذا كان كائن AliasDictionary يحتوي على الاسم المستعار المحدد. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | يحصل على النص المرتبط بالاسم المستعار المحدد. |
|
|  | [clear()](#clear--) | يزيل جميع الأسماء المستعارة من كائن AliasDictionary . |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الأسماء المستعارة الموجودة في AliasDictionary .


**Returns:**
int - عدد الأسماء المستعارة الموجودة في AliasDictionary .

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


يضيف مجموعة أزواج الاسم المستعار/البديل المحددة إلى هذه المثيلة من AliasDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | أزواج | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | المجموعة من أزواج الاسم المستعار/البديل لإضافتها إلى القاموس. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


يضيف مجموعة أزواج الاسم المستعار/البديل المحددة إلى هذه المثيلة من AliasDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | المجموعة من أزواج الاسم المستعار/البديل لإضافتها إلى القاموس. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


يضيف الزوج المحدد من الاسم المستعار والنص المرتبط إلى هذه المثيلة من AliasDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | اسم مستعار | java.lang.String | الاسم المستعار لإضافته إلى القاموس. |
|
|  | نص | java.lang.String | النص المرتبط بالاسم المستعار. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


يزيل الاسم المستعار المحدد من كائن AliasDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | اسم مستعار | java.lang.String | الاسم المستعار للإزالة. |
|

**Returns:**
boolean - تُعيد هذه الطريقة  true  إذا تم العثور على الاسم المستعار وإزالته بنجاح. تُعيد هذه الطريقة  false  إذا لم يُعثر على الاسم المستعار في كائن AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


يحدد ما إذا كان كائن AliasDictionary يحتوي على الاسم المستعار المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | اسم مستعار | java.lang.String | الاسم المستعار للبحث عنه في كائن AliasDictionary . |
|

**Returns:**
boolean -  true  إذا كان كائن AliasDictionary يحتوي على الاسم المستعار المحدد؛ وإلا،  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


يحصل على النص المرتبط بالاسم المستعار المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | اسم مستعار | java.lang.String | الاسم المستعار للبحث عنه في كائن AliasDictionary . |
|

**Returns:**
java.lang.String - نص مرتبط بالاسم المستعار المحدد أو  null .

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع الأسماء المستعارة من كائن AliasDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.String> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

