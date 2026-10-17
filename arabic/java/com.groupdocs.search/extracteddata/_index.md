---
title: "ExtractedData"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل البيانات المستخرجة من مستند ومُعدة للفهرسة."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

يمثل البيانات المستخرجة من مستند ومُعدة للفهرسة.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [serialize()](#serialize--) | يسلسل المثيل الحالي إلى مصفوفة بايت. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | يفك تسلسل مثيل من مصفوفة بايت. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


يسلسل المثيل الحالي إلى مصفوفة بايت.


**Returns:**
byte[] - مصفوفة بايت تمثل المثيل الحالي.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


يفك تسلسل مثيل من مصفوفة بايت.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مصفوفة | byte[] | مصفوفة بايت للتسلسل العكسي منها. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

