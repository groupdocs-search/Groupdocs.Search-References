---
title: Create
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: मेमर में एक नय इंडेक्स बनत है
type: docs
weight: 50
url: /hi/net/groupdocs.search/indexrepository/create/
---
## Create() {#create}

मेमोरी में एक नया इंडेक्स बनाता है।

```csharp
public Index Create()
```

### प्रतिलाभ की मात्रा

बनाया गया सूचकांक।

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से मेमोरी में इंडेक्स कैसे बनाया जाए।

```csharp
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create();
```

### यह सभी देखें

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* नाम स्थान [GroupDocs.Search](../../indexrepository)
* सभा [GroupDocs.Search](../../../)

---

## Create(IndexSettings) {#create_1}

मेमोरी में एक नया इंडेक्स बनाता है।

```csharp
public Index Create(IndexSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | IndexSettings | सूचकांक सेटिंग्स। |

### प्रतिलाभ की मात्रा

बनाया गया सूचकांक।

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से मेमोरी में इंडेक्स कैसे बनाया जाए।

```csharp
IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // अनुक्रमण के दौरान स्टॉप शब्दों के उपयोग को अक्षम करना

Index index = indexRepository.Create(settings);
```

### यह सभी देखें

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* नाम स्थान [GroupDocs.Search](../../indexrepository)
* सभा [GroupDocs.Search](../../../)

---

## Create(string) {#create_2}

डिस्क पर एक नया इंडेक्स बनाता है। इंडेक्स बनाने से पहले इंडेक्स फोल्डर को साफ कर दिया जाएगा।

```csharp
public Index Create(string indexFolder)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| indexFolder | String | अनुक्रमणिका फ़ोल्डर। |

### प्रतिलाभ की मात्रा

बनाया गया सूचकांक।

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से डिस्क पर इंडेक्स कैसे बनाया जाए।

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create(indexFolder);
```

### यह सभी देखें

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* नाम स्थान [GroupDocs.Search](../../indexrepository)
* सभा [GroupDocs.Search](../../../)

---

## Create(string, IndexSettings) {#create_3}

डिस्क पर एक नया इंडेक्स बनाता है। इंडेक्स बनाने से पहले इंडेक्स फोल्डर को साफ कर दिया जाएगा।

```csharp
public Index Create(string indexFolder, IndexSettings settings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| indexFolder | String | अनुक्रमणिका फ़ोल्डर। |
| settings | IndexSettings | सूचकांक सेटिंग्स। |

### प्रतिलाभ की मात्रा

बनाया गया सूचकांक।

### उदाहरण

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से डिस्क पर इंडेक्स कैसे बनाया जाए।

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // अनुक्रमण के दौरान स्टॉप शब्दों के उपयोग को अक्षम करना

Index index = indexRepository.Create(indexFolder, settings);
```

### यह सभी देखें

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* नाम स्थान [GroupDocs.Search](../../indexrepository)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
