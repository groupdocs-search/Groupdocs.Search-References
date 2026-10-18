---
title: "Extractor"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ों से प्रारंभिक डेटा निष्कर्षण के लिए एक उपकरण का प्रतिनिधित्व करता है, जिससे बाद के तेज़ इंडेक्सिंग चरण को अलग किया जा सके।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

दस्तावेज़ों से प्रारंभिक डेटा निष्कर्षण के लिए एक उपकरण का प्रतिनिधित्व करता है, जिससे बाद के तेज़ इंडेक्सिंग चरण को अलग किया जा सके।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Extractor()](#Extractor--) | Extractor क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## Fields

| Field | विवरण |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | एक्सट्रैक्टर ऑपरेशन के दौरान त्रुटि होने पर होता है। |
|
|  | [ImagePreparing](#ImagePreparing) | इंडेक्सिंग के लिए छवि तैयार होने पर होता है। |
|
|  | [PasswordRequired](#PasswordRequired) | दस्तावेज़ को खोलने के लिए पासवर्ड चाहिए होने पर होता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getSettings()](#getSettings--) | एक्सट्रैक्टर सेटिंग्स प्राप्त करता है। |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | दस्तावेज़ से डेटा निकालता है। |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Extractor क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


एक्सट्रैक्टर ऑपरेशन के दौरान त्रुटि होने पर होता है।


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


इंडेक्सिंग के लिए छवि तैयार होने पर होता है।


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


दस्तावेज़ को खोलने के लिए पासवर्ड चाहिए होने पर होता है।


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


एक्सट्रैक्टर सेटिंग्स प्राप्त करता है।


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


दस्तावेज़ से डेटा निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़। |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | निकालने के विकल्प। |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| संदेश | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़कुंजी | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| स्ट्रीम | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइलपथ | java.lang.String |  |

**Returns:**
java.lang.String
