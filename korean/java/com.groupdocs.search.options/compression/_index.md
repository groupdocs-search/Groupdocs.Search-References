---
title: "Compression"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "압축 수준을 지정합니다."
type: docs
weight: 47
url: /ko/java/com.groupdocs.search.options/compression/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum Compression extends Enum<Compression>
```

압축 수준을 지정합니다.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [None](#None) | 압축이 비활성화되었습니다. |
|
|  | [Normal](#Normal) | 보통 압축 수준입니다. |
|
|  | [High](#High) | 높은 압축 수준입니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### None {#None}
```
public static final Compression None
```


압축이 비활성화되었습니다.


### Normal {#Normal}
```
public static final Compression Normal
```


보통 압축 수준입니다.


### High {#High}
```
public static final Compression High
```


높은 압축 수준입니다.


### values() {#values--}
```
public static Compression[] values()
```




**Returns:**
com.groupdocs.search.options.Compression[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static Compression valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Compression](../../com.groupdocs.search.options/compression)
