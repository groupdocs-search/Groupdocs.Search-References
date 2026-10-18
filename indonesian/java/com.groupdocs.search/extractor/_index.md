---
title: "Extractor"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili alat untuk ekstraksi data awal dari dokumen guna memisahkan tahap pengindeksan cepat berikutnya."
type: docs
weight: 16
url: /id/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Mewakili alat untuk ekstraksi data awal dari dokumen guna memisahkan tahap pengindeksan cepat berikutnya.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Extractor()](#Extractor--) | Menginisialisasi sebuah instance baru dari kelas Extractor. |
|
## Fields

| Field | Deskripsi |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Terjadi ketika kesalahan terjadi selama operasi extractor. |
|
|  | [ImagePreparing](#ImagePreparing) | Terjadi ketika sebuah gambar akan dipersiapkan untuk pengindeksan. |
|
|  | [PasswordRequired](#PasswordRequired) | Terjadi ketika sebuah dokumen memerlukan kata sandi untuk dibuka. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSettings()](#getSettings--) | Mendapatkan pengaturan extractor. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Mengekstrak data dari sebuah dokumen. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Menginisialisasi sebuah instance baru dari kelas Extractor.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Terjadi ketika kesalahan terjadi selama operasi extractor.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Terjadi ketika sebuah gambar akan dipersiapkan untuk pengindeksan.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Terjadi ketika sebuah dokumen memerlukan kata sandi untuk dibuka.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Mendapatkan pengaturan extractor.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Mengekstrak data dari sebuah dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Dokumen dari sistem file, aliran, atau struktur. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Opsi ekstraksi. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
