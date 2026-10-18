---
title: "EventHubBase"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이벤트 허브를 위한 기본 추상 클래스입니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.events/eventhubbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class EventHubBase
```

이벤트 허브를 위한 기본 추상 클래스입니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [EventHubBase()](#EventHubBase--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### EventHubBase() {#EventHubBase--}
```
public EventHubBase()
```


### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public abstract void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 메시지 | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public abstract void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| stream | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public abstract String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
