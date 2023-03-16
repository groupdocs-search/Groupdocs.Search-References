---
title: Add
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: इंडेक्संग ऑपरेशन करत है एक फ़इल य फ़ल्डर क एक पूर्ण य सपेक्ष पथ से जड़त है सभ सबफ़ल्डर्स के दस्तवेज़ं क अनुक्रमत कय जएग
type: docs
weight: 70
url: /hi/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

इंडेक्सिंग ऑपरेशन करता है। एक फ़ाइल या फ़ोल्डर को एक पूर्ण या सापेक्ष पथ से जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा।

```csharp
public void Add(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | अनुक्रमित की जाने वाली फ़ाइल या फ़ोल्डर का पथ। |

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़े जाते हैं।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(folderPath); // निर्दिष्ट फ़ोल्डर में दस्तावेज़ अनुक्रमण
index.Add(filePath); // निर्दिष्ट दस्तावेज़ को अनुक्रमणित करना
```

### यह सभी देखें

* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

इंडेक्सिंग ऑपरेशन करता है। एक फ़ाइल या फ़ोल्डर को एक पूर्ण या सापेक्ष पथ से जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा।

```csharp
public void Add(string path, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | अनुक्रमित की जाने वाली फ़ाइल या फ़ोल्डर का पथ। |
| options | IndexingOptions | अनुक्रमण विकल्प। |

### उदाहरण

उदाहरण दर्शाता है कि विशेष इंडेक्सिंग विकल्पों के साथ इंडेक्स में दस्तावेज़ कैसे जोड़े जाते हैं।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // इंडेक्सिंग थ्रेड्स की संख्या निर्धारित करना
index.Add(folderPath, options); // निर्दिष्ट फ़ोल्डर में दस्तावेज़ अनुक्रमण
index.Add(filePath, options); // निर्दिष्ट दस्तावेज़ को अनुक्रमणित करना
```

### यह सभी देखें

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

इंडेक्सिंग ऑपरेशन करता है। एक पूर्ण या सापेक्ष पथ से फ़ाइलें या फ़ोल्डर जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा।

```csharp
public void Add(string[] paths)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| paths | String[] | अनुक्रमित की जाने वाली फ़ाइलों या फ़ोल्डरों के पथ। |

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़े जाते हैं।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // निर्दिष्ट पथ पर अनुक्रमणिका दस्तावेज़
```

### यह सभी देखें

* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

इंडेक्सिंग ऑपरेशन करता है। एक पूर्ण या सापेक्ष पथ से फ़ाइलें या फ़ोल्डर जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा।

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| paths | String[] | अनुक्रमित की जाने वाली फ़ाइलों या फ़ोल्डरों के पथ। |
| options | IndexingOptions | अनुक्रमण विकल्प। |

### उदाहरण

उदाहरण दर्शाता है कि विशेष इंडेक्सिंग विकल्पों के साथ इंडेक्स में दस्तावेज़ कैसे जोड़े जाते हैं।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // इंडेक्सिंग थ्रेड्स की संख्या निर्धारित करना
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // निर्दिष्ट पथ पर अनुक्रमणिका दस्तावेज़
```

### यह सभी देखें

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

इंडेक्सिंग ऑपरेशन करता है। फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़ जोड़ता है।

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| documents | Document[] | फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़। |
| options | IndexingOptions | अनुक्रमण विकल्प। |

### यह सभी देखें

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

इंडेक्सिंग ऑपरेशन करता है। निकाले गए डेटा को इंडेक्स में जोड़ता है।

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| data | ExtractedData[] | निकाला गया डेटा। |
| options | IndexingOptions | अनुक्रमण विकल्प। |

### यह सभी देखें

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
