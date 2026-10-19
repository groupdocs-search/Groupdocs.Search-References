---
title: "Ekle"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile bir dosya veya klasör ekler. Tüm alt klasörlerden belgeler indekslenecektir."
type: docs
weight: 80
url: /tr/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile bir dosya veya klasör ekler. Tüm alt klasörlerden belgeler indekslenecektir.

```csharp
public void Add(string path)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Dizine eklenecek dosya veya klasörün yolu. |

### Örnekler

Örnek, belgelere bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Ayrıca Bakınız

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile bir dosya veya klasör ekler. Tüm alt klasörlerden belgeler indekslenecektir.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Dizine eklenecek dosya veya klasörün yolu. |
| seçenekler | IndexingOptions | Dizinleme seçenekleri. |

### Örnekler

Örnek, belirli dizinleme seçenekleriyle belgelere bir dizine nasıl ekleneceğini gösterir.

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

### Ayrıca Bakınız

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile dosyalar veya klasörler ekler. Tüm alt klasörlerden belgeler indekslenecektir.

```csharp
public void Add(string[] paths)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yollar | String[] | Dizine eklenecek dosya veya klasörlerin yolları. |

### Örnekler

Örnek, belgelere bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Ayrıca Bakınız

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli bir yol ile dosyalar veya klasörler ekler. Tüm alt klasörlerden belgeler indekslenecektir.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yollar | String[] | Dizine eklenecek dosya veya klasörlerin yolları. |
| seçenekler | IndexingOptions | Dizinleme seçenekleri. |

### Örnekler

Örnek, belirli dizinleme seçenekleriyle belgelere bir dizine nasıl ekleneceğini gösterir.

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

### Ayrıca Bakınız

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

İndeksleme işlemini gerçekleştirir. Dosya sisteminden, akıştan veya yapıyıdan belgeler ekler.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| belgeler | Document[] | Dosya sisteminden, akıştan veya yapıdan gelen belgeler. |
| seçenekler | IndexingOptions | Dizinleme seçenekleri. |

### Ayrıca Bakınız

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

İndeksleme işlemini gerçekleştirir. Çıkarılan verileri indekse ekler.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | ExtractedData[] | Çıkarılan veri. |
| seçenekler | IndexingOptions | Dizinleme seçenekleri. |

### Ayrıca Bakınız

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
