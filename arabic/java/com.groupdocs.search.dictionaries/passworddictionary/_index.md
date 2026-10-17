---
title: "PasswordDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس كلمات مرور المستندات."
type: docs
weight: 20
url: /ar/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

يحدد واجهة قاموس كلمات مرور المستندات.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في القاموس. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | يحصل على كلمة المرور للملف. |
|
|  | [clear()](#clear--) | يزيل جميع كلمات المرور من كائن  PasswordDictionary  هذا. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | يحدد ما إذا كان القاموس يحتوي على كلمة مرور للمستند المحدد. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | يضيف كلمة مرور لمستند إلى القاموس. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | يزيل كلمة مرور للمستند المحدد من القاموس. |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد العناصر الموجودة في القاموس.


**Returns:**
int - عدد العناصر الموجودة في القاموس.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


يحصل على كلمة المرور للملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار الملف. |
|

**Returns:**
java.lang.String - كلمة المرور للملف.

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع كلمات المرور من كائن  PasswordDictionary  هذا.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


يحدد ما إذا كان القاموس يحتوي على كلمة مرور للمستند المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف المستند. |
|

**Returns:**
boolean -  true  إذا كان القاموس يحتوي على كلمة مرور للمستند؛ وإلا،  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


يضيف كلمة مرور لمستند إلى القاموس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف المستند. |
|
|  | كلمة المرور | java.lang.String | كلمة مرور المستند. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


يزيل كلمة مرور للمستند المحدد من القاموس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف المستند. |
|

**Returns:**
boolean -  true  إذا تمت إزالة كلمة المرور بنجاح؛ وإلا،  false . كما تُعيد هذه الطريقة  false  إذا لم يتم العثور على  filePath  في القاموس.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.String> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

