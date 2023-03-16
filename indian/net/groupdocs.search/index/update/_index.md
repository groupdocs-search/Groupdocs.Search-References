---
title: Update
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: उन दस्तवेज़ं क पुन अनुक्रमत करत है जन्हें पछले अपडेट के बद से बदल दय गय है य हट दय गय है उन नई फ़इलं क जड़त है जन्हें अनुक्रमत फ़ल्डर में जड़ गय है
type: docs
weight: 240
url: /hi/net/groupdocs.search/index/update/
---
## Update() {#update}

उन दस्तावेज़ों को पुन: अनुक्रमित करता है जिन्हें पिछले अपडेट के बाद से बदल दिया गया है या हटा दिया गया है। उन नई फ़ाइलों को जोड़ता है जिन्हें अनुक्रमित फ़ोल्डर में जोड़ा गया है।

```csharp
public void Update()
```

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स को कैसे अपडेट किया जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएं या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें

index.Update(); // इंडेक्स को अपडेट करना
```

### यह सभी देखें

* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

उन दस्तावेज़ों को पुन: अनुक्रमित करता है जिन्हें पिछले अपडेट के बाद से बदल दिया गया है या हटा दिया गया है। उन नई फ़ाइलों को जोड़ता है जिन्हें अनुक्रमित फ़ोल्डर में जोड़ा गया है।

```csharp
public void Update(UpdateOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | UpdateOptions | अद्यतन विकल्प। |

### उदाहरण

उदाहरण दर्शाता है कि किसी इंडेक्स को विशेष अपडेट विकल्पों के साथ कैसे अपडेट किया जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएं या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // इंडेक्सिंग थ्रेड्स की संख्या निर्धारित करना
index.Update(options); // इंडेक्स को अपडेट करना
```

### यह सभी देखें

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->