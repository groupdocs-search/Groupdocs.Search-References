---
title: "IndexSettingsConfigurator"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज नेटवर्क में प्रत्येक शार्ड के लिए इंडेक्स सेटिंग्स कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.search.scaling.configuring/indexsettingsconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexSettingsConfigurator
```

खोज नेटवर्क में प्रत्येक शार्ड के लिए इंडेक्स सेटिंग्स कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [IndexSettingsConfigurator()](#IndexSettingsConfigurator--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | स्टॉप शब्दों के उपयोग का फ्लैग सेट करता है। |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | कैरेक्टर रिप्लेसमेंट्स के उपयोग का फ्लैग सेट करता है। |
|
|  | [setTextStorageSettings(boolean isUsed, Compression compression)](#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-) | पाठ संग्रह सेटिंग्स सेट करता है। |
|
|  | [setIndexType(IndexType indexType)](#setIndexType-com.groupdocs.search.options.IndexType-) | इंडेक्स प्रकार सेट करता है। |
|
|  | [setSearchThreads(NumberOfThreads numberOfThreads)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | सर्च थ्रेड्स की संख्या सेट करता है। |
|
|  | [completeIndexSettings()](#completeIndexSettings--) | इंडेक्स सेटिंग्स की कॉन्फ़िगरेशन पूरी करता है। |
|
### IndexSettingsConfigurator() {#IndexSettingsConfigurator--}
```
public IndexSettingsConfigurator()
```


### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public abstract IndexSettingsConfigurator setUseStopWords(boolean value)
```


स्टॉप शब्दों के उपयोग का फ्लैग सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | फ़्लैग मान। |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public abstract IndexSettingsConfigurator setUseCharacterReplacements(boolean value)
```


कैरेक्टर रिप्लेसमेंट्स के उपयोग का फ्लैग सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | फ़्लैग मान। |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setTextStorageSettings(boolean isUsed, Compression compression) {#setTextStorageSettings-boolean-com.groupdocs.search.options.Compression-}
```
public abstract IndexSettingsConfigurator setTextStorageSettings(boolean isUsed, Compression compression)
```


पाठ संग्रह सेटिंग्स सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | isUsed | boolean | इंडेक्स में टेक्स्ट स्टोरेज के उपयोग का फ़्लैग। |
|
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | संपीड़न स्तर। |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setIndexType(IndexType indexType) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract IndexSettingsConfigurator setIndexType(IndexType indexType)
```


इंडेक्स प्रकार सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexType | [IndexType](../../com.groupdocs.search.options/indextype) | इंडेक्स प्रकार। |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### setSearchThreads(NumberOfThreads numberOfThreads) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public abstract IndexSettingsConfigurator setSearchThreads(NumberOfThreads numberOfThreads)
```


सर्च थ्रेड्स की संख्या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | numberOfThreads | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | खोज थ्रेड्स की संख्या। |
|

**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### completeIndexSettings() {#completeIndexSettings--}
```
public abstract Configurator completeIndexSettings()
```


इंडेक्स सेटिंग्स की कॉन्फ़िगरेशन पूरी करता है।


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

