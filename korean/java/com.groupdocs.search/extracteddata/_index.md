---
title: "ExtractedData"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서에서 검색되어 인덱싱을 위해 준비된 데이터를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

문서에서 검색되어 인덱싱을 위해 준비된 데이터를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [serialize()](#serialize--) | 현재 인스턴스를 바이트 배열로 직렬화합니다. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 바이트 배열에서 인스턴스를 역직렬화합니다. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


현재 인스턴스를 바이트 배열로 직렬화합니다.


**Returns:**
byte[] - 현재 인스턴스를 나타내는 바이트 배열.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


바이트 배열에서 인스턴스를 역직렬화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 배열 | byte[] | 역직렬화에 사용할 바이트 배열. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

