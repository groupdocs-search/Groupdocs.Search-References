---
title: "FragmentContainer"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل حاوية لقطاعات النص مع تسليط الضوء على المصطلحات المكتشفة في حقل مستند واحد."
type: docs
weight: 22
url: /ar/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

يمثل حاوية لقطاعات النص مع تسليط الضوء على المصطلحات المكتشفة في حقل مستند واحد.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | يحصل على اسم حقل المستند. |
|
|  | [getCount()](#getCount--) | يحصل على عدد مقاطع النص المتضمنة. |
|
|  | [getFragments()](#getFragments--) | يحصل على مصفوفة من مقاطع النص المتضمنة. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


يحصل على اسم حقل المستند.


**Returns:**
java.lang.String - اسم حقل المستند.

### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد مقاطع النص المتضمنة.


**Returns:**
int - عدد مقاطع النص المتضمنة.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


يحصل على مصفوفة من مقاطع النص المتضمنة.


**Returns:**
java.lang.String[] - مصفوفة من مقاطع النص المتضمنة.

