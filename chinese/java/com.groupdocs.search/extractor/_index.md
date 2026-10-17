---
title: "Extractor"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示用于从文档进行初步数据提取以分离后续快速索引阶段的工具。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

表示用于从文档进行初步数据提取以分离后续快速索引阶段的工具。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Extractor()](#Extractor--) | 初始化 Extractor 类的新实例。 |
|
## Fields

| Field | 描述 |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | 在提取器操作期间发生错误时出现。 |
|
|  | [ImagePreparing](#ImagePreparing) | 在准备图像进行索引时出现。 |
|
|  | [PasswordRequired](#PasswordRequired) | 在文档打开需要密码时出现。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getSettings()](#getSettings--) | 获取提取器设置。 |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | 从文档中提取数据。 |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


初始化 Extractor 类的新实例。


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


在提取器操作期间发生错误时出现。


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


在准备图像进行索引时出现。


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


在文档打开需要密码时出现。


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


获取提取器设置。


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


从文档中提取数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | 来自文件系统、流或结构的文档。 |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | 提取选项。 |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文档键 | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| 流 | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 文件路径 | java.lang.String |  |

**Returns:**
java.lang.String
