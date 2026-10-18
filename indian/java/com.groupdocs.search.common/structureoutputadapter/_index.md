---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को प्रत्येक फ़ील्ड को अलग-अलग शामिल करने वाली संरचना के रूप में एकत्र करता है।"
type: docs
weight: 33
url: /hi/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को प्रत्येक फ़ील्ड को अलग-अलग शामिल करने वाली संरचना के रूप में एकत्र करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StructureOutputAdapter वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getResult()](#getResult--) | परिणामी फ़ील्ड्स की सरणी प्राप्त करता है। |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


StructureOutputAdapter वर्ग का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | आउटपुट फ़ॉर्मेट। |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


परिणामी फ़ील्ड्स की सरणी प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.DocumentField[] - परिणामी फ़ील्ड्स की सरणी।

