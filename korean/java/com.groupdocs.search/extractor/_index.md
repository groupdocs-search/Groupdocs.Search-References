---
title: "Extractor"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "후속 빠른 인덱싱 단계와 분리하기 위해 문서에서 사전 데이터 추출을 수행하는 도구를 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

후속 빠른 인덱싱 단계와 분리하기 위해 문서에서 사전 데이터 추출을 수행하는 도구를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Extractor()](#Extractor--) | 새로운 Extractor 클래스 인스턴스를 초기화합니다. |
|
## 필드

| 필드 | 설명 |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | 추출기 작업 중 오류가 발생할 때 발생합니다. |
|
|  | [ImagePreparing](#ImagePreparing) | 이미지를 인덱싱을 위해 준비할 때 발생합니다. |
|
|  | [PasswordRequired](#PasswordRequired) | 문서를 열기 위해 비밀번호가 필요할 때 발생합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSettings()](#getSettings--) | 추출기 설정을 가져옵니다. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | 문서에서 데이터를 추출합니다. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


새로운 Extractor 클래스 인스턴스를 초기화합니다.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


추출기 작업 중 오류가 발생할 때 발생합니다.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


이미지를 인덱싱을 위해 준비할 때 발생합니다.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


문서를 열기 위해 비밀번호가 필요할 때 발생합니다.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


추출기 설정을 가져옵니다.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


문서에서 데이터를 추출합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | 파일 시스템, 스트림 또는 구조에서 가져온 문서. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | 추출 옵션. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 메시지 | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
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
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
