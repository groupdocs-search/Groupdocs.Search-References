---
title: "التكوين"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل تكوين شبكة البحث."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

يمثل تكوين شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | يحفظ هذا التكوين إلى ملف. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | يحفظ هذا التكوين إلى تدفق. |
|
|  | [load(String filePath)](#load-java.lang.String-) | يقوم بتحميل تكوين شبكة البحث من ملف. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | يقوم بتحميل تكوين شبكة البحث من تدفق. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


يحفظ هذا التكوين إلى ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | الملف المراد الحفظ إليه. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


يحفظ هذا التكوين إلى تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.OutputStream | التدفق المراد الحفظ إليه. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


يقوم بتحميل تكوين شبكة البحث من ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | الملف المراد التحميل منه. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


يقوم بتحميل تكوين شبكة البحث من تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | التدفق المراد التحميل منه. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

