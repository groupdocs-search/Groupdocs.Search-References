---
title: "IndexType"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد نوع الفهرس."
type: docs
weight: 49
url: /ar/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

يحدد نوع الفهرس.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | فهرس عادي يتضمن بيانات تعريف المستندات ومحتوى المستندات ويدعم جميع ميزات البحث. |
|
|  | [MetadataIndex](#MetadataIndex) | فهرس يحتوي فقط على بيانات تعريف المستندات، دون المحتوى. |
|
|  | [CompactIndex](#CompactIndex) | نوع الفهرس الذي يشغل مساحة قرص أقل بكثير لكنه لا يدعم ميزات البحث بالعبارات والبحث في نطاقات التاريخ. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


فهرس عادي يتضمن بيانات تعريف المستندات ومحتوى المستندات ويدعم جميع ميزات البحث.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


فهرس يحتوي فقط على بيانات تعريف المستندات، دون المحتوى.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


نوع الفهرس الذي يشغل مساحة قرص أقل بكثير لكنه لا يدعم ميزات البحث بالعبارات والبحث في نطاقات التاريخ.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
