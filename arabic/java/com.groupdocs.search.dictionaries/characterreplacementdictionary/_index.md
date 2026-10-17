---
title: "CharacterReplacementDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس استبدال الأحرف الذي يُستخدم أثناء عملية الفهرسة."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

يحدد واجهة قاموس استبدال الأحرف الذي يُستخدم أثناء عملية الفهرسة. يمكن استخدام استبدال الأحرف، على سبيل المثال، لإزالة النبرات من الأحرف ذات النبرات أو لإنشاء فهرس غير حساس لحالة الأحرف.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الأحرف الموجودة في هذا  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | يضيف مجموعة الاستبدالات المحددة للأحرف إلى هذه النسخة من  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | يضيف مجموعة الاستبدالات المحددة للأحرف إلى هذه النسخة من  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | يزيل مجموعة الاستبدالات المحددة للأحرف من هذه النسخة من  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | يحدد ما إذا كان كائن  CharacterReplacementDictionary  يحتوي على استبدال للحرف المحدد. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | يحصل على استبدال للحرف المحدد. |
|
|  | [clear()](#clear--) | يزيل جميع استبدالات الأحرف من كائن  CharacterReplacementDictionary . |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الأحرف الموجودة في هذا  CharacterReplacementDictionary .


**Returns:**
int - عدد الأحرف في القاموس.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


يضيف مجموعة الاستبدالات المحددة للأحرف إلى هذه النسخة من  CharacterReplacementDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | مجموعة استبدالات الأحرف لإضافتها إلى القاموس. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


يضيف مجموعة الاستبدالات المحددة للأحرف إلى هذه النسخة من  CharacterReplacementDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | مجموعة استبدالات الأحرف لإضافتها إلى القاموس. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


يزيل مجموعة الاستبدالات المحددة للأحرف من هذه النسخة من  CharacterReplacementDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | أحرف | char[] | مجموعة الأحرف المراد إزالتها. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


يحدد ما إذا كان كائن  CharacterReplacementDictionary  يحتوي على استبدال للحرف المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | حرف | char | الحرف المراد تحديد موقعه في كائن  CharacterReplacementDictionary . |
|

**Returns:**
منطقي -  true  إذا كان كائن  CharacterReplacementDictionary  يحتوي على الحرف المحدد؛ وإلا،  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


يحصل على استبدال للحرف المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | حرف | char | الحرف المراد الحصول على بديل له. |
|

**Returns:**
حرف - البديل للحرف المحدد.

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع استبدالات الأحرف من كائن  CharacterReplacementDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.Character> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

