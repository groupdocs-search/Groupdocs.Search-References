---
title: "TextStorageSettings"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "텍스트 저장 설정을 나타냅니다."
type: docs
weight: 42
url: /ko/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

텍스트 저장 설정을 나타냅니다.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | TextStorageSettings 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCompression()](#getCompression--) | 텍스트 저장소의 압축을 가져옵니다. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | 텍스트 저장소의 압축을 설정합니다. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


TextStorageSettings 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | 텍스트 저장소의 압축입니다. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


텍스트 저장소의 압축을 가져옵니다. 기본값은 Compression.Normal입니다.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


텍스트 저장소의 압축을 설정합니다. 기본값은 Compression.Normal입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | 텍스트 저장소의 압축입니다. |
|

