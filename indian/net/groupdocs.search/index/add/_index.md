---
title: "जोड़ें"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा।"
type: docs
weight: 80
url: /hi/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा।

```csharp
public void Add(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | इंडेक्स करने के लिए फ़ाइल या फ़ोल्डर का पथ। |

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़ें।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### संबंधित देखें

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा।

```csharp
public void Add(string path, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | इंडेक्स करने के लिए फ़ाइल या फ़ोल्डर का पथ। |
| विकल्प | IndexingOptions | इंडेक्सिंग विकल्प। |

### उदाहरण

उदाहरण दर्शाता है कि विशेष इंडेक्सिंग विकल्पों के साथ इंडेक्स में दस्तावेज़ कैसे जोड़ें।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### संबंधित देखें

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा।

```csharp
public void Add(string[] paths)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| paths | String[] | इंडेक्स करने के लिए फ़ाइलों या फ़ोल्डरों के पथ। |

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़ें।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### संबंधित देखें

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा।

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| paths | String[] | इंडेक्स करने के लिए फ़ाइलों या फ़ोल्डरों के पथ। |
| विकल्प | IndexingOptions | इंडेक्सिंग विकल्प। |

### उदाहरण

उदाहरण दर्शाता है कि विशेष इंडेक्सिंग विकल्पों के साथ इंडेक्स में दस्तावेज़ कैसे जोड़ें।

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### संबंधित देखें

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

इंडेक्सिंग ऑपरेशन करता है। फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़ जोड़ता है।

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Document[] | फ़ाइल सिस्टम, स्ट्रीम या संरचना से प्राप्त दस्तावेज़। |
| विकल्प | IndexingOptions | इंडेक्सिंग विकल्प। |

### संबंधित देखें

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

इंडेक्सिंग ऑपरेशन करता है। निकाले गए डेटा को इंडेक्स में जोड़ता है।

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डेटा | ExtractedData[] | निकाले गए डेटा। |
| विकल्प | IndexingOptions | इंडेक्सिंग विकल्प। |

### संबंधित देखें

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
