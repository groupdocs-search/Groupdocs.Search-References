---
title: "EnglishWordFormsProvider"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل موفر صيغ الكلمات الإنجليزية."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

يمثل موفر صيغ الكلمات الإنجليزية.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | يُنشئ مثيلاً جديدًا لـ |
EnglishWordFormsProvider
الفئة.
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | يحصل على صيغ الكلمة للكلمة المحددة. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


يُنشئ مثيلاً جديدًا لـ
EnglishWordFormsProvider
الفئة.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


يحصل على صيغ الكلمة للكلمة المحددة.
المصفوفة الناتجة لا تحتوي على الكلمة الأصلية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة للحصول على صيغ الكلمة. |
|

**Returns:**
java.lang.String[] - صيغ الكلمات للكلمة المحددة أو مصفوفة فارغة إذا لم يقدم IWordFormsProvider صيغ الكلمات للكلمة المحددة.

