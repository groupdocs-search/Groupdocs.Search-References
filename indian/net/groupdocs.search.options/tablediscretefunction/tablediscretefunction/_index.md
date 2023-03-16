---
title: TableDiscreteFunction
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: क एक नय उदहरण प्ररंभ करत हैTableDiscreteFunctiongroupdocs.search.options/tablediscretefunction वर्ग.
type: docs
weight: 10
url: /hi/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`TableDiscreteFunction`](../../tablediscretefunction) वर्ग.

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| offsetOfInputs | Int32 | तालिका का ऑफसेट इनपुट मानों के सापेक्ष होता है। |
| tableOfOutputs | Int32[] | आउटपुट मानों की तालिका। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | कब फेंका*tableOfOutputs* है`व्यर्थ`. |
| ArgumentException | तालिका तत्वों की संख्या 0 होने पर फेंक दिया गया। |

### यह सभी देखें

* class [TableDiscreteFunction](../../tablediscretefunction)
* नाम स्थान [GroupDocs.Search.Options](../../tablediscretefunction)
* सभा [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`TableDiscreteFunction`](../../tablediscretefunction) वर्ग.

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| firstStepLevel | Int32 | स्टेप फंक्शन के पहले चरण का स्तर। |
| steps | Step[] | स्टेप फंक्शन के अगले चरण। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | कब फेंका*steps* है`व्यर्थ`. |
| ArgumentException | कदमों की सीमा सख्ती से नहीं बढ़ने पर फेंका गया। |

### यह सभी देखें

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* नाम स्थान [GroupDocs.Search.Options](../../tablediscretefunction)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->