---
title: "الأبجدية"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس الأحرف الذي يُستخدم أثناء الفهرسة لاكتشاف نوع الحرف."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

يحدد واجهة قاموس الأحرف الذي يُستخدم أثناء الفهرسة لاكتشاف نوع الحرف. يمكن التعامل مع كل حرف كفاصل أو كحرف أو كلاهما.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | يحصل على نوع الحرف. |
|
|  | [getCount()](#getCount--) | يحصل على عدد الأحرف الموجودة في الـ Alphabet. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | يضبط النوع لكل حرف من المجموعة المحددة في هذه النسخة من الـ Alphabet. |
|
|  | [clear()](#clear--) | يضبط النوع CharacterType.Separator لجميع الأحرف في هذا الـ Alphabet. |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


يحصل على نوع الحرف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | حرف | char | الحرف للحصول على نوع. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الأحرف الموجودة في الـ Alphabet.


**Returns:**
int - عدد الأحرف في القاموس.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


يضبط النوع لكل حرف من المجموعة المحددة في هذه النسخة من الـ Alphabet.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | أحرف | char[] | مجموعة الأحرف لضبط النوع. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | نوع الحرف. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يضبط النوع CharacterType.Separator لجميع الأحرف في هذا الـ Alphabet.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.Character> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

