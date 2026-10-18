---
title: "Extractor"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belgelerden ön veri çıkarımı için, sonraki hızlı indeksleme aşamasını ayırmaya yarayan bir aracı temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Belgelerden ön veri çıkarımı için, sonraki hızlı indeksleme aşamasını ayırmaya yarayan bir aracı temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Extractor()](#Extractor--) | Extractor sınıfının yeni bir örneğini başlatır. |
|
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Bir çıkarıcı işlemi sırasında bir hata oluştuğunda meydana gelir. |
|
|  | [ImagePreparing](#ImagePreparing) | Bir görüntü indeksleme için hazırlanırken meydana gelir. |
|
|  | [PasswordRequired](#PasswordRequired) | Bir belge açmak için şifre gerektirdiğinde meydana gelir. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSettings()](#getSettings--) | Çıkarıcı ayarlarını alır. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Bir belgeden veri çıkarır. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Extractor sınıfının yeni bir örneğini başlatır.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Bir çıkarıcı işlemi sırasında bir hata oluştuğunda meydana gelir.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Bir görüntü indeksleme için hazırlanırken meydana gelir.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Bir belge açmak için şifre gerektirdiğinde meydana gelir.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Çıkarıcı ayarlarını alır.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Bir belgeden veri çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Dosya sisteminden, akıştan veya yapıdan gelen belge. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Çıkarma seçenekleri. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mesaj | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
