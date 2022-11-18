---
title: Add
second_title: .NET API Başvurusu için GroupDocs.Search
description: İndeksleme işlemini gerçekleştirir. Mutlak veya göreli yolla bir dosya veya klasör ekler. Tüm alt klasörlerdeki belgeler indekslenir.
type: docs
weight: 70
url: /tr/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli yolla bir dosya veya klasör ekler. Tüm alt klasörlerdeki belgeler indekslenir.

```csharp
public void Add(string path)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Dizine eklenecek bir dosya veya klasörün yolu. |

### Örnekler

Örnek, belgelerin bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(folderPath); //Belirtilen klasördeki belgeleri indeksleme
index.Add(filePath); // Belirtilen belgeyi indeksleme
```

### Ayrıca bakınız

* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

İndeksleme işlemini gerçekleştirir. Mutlak veya göreli yolla bir dosya veya klasör ekler. Tüm alt klasörlerdeki belgeler indekslenir.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Dizine eklenecek bir dosya veya klasörün yolu. |
| options | IndexingOptions | İndeksleme seçenekleri. |

### Örnekler

Örnek, belgelerin belirli dizin oluşturma seçenekleriyle bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // İndeksleme dizilerinin sayısını ayarlama
index.Add(folderPath, options); //Belirtilen klasördeki belgeleri indeksleme
index.Add(filePath, options); // Belirtilen belgeyi indeksleme
```

### Ayrıca bakınız

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

İndeksleme işlemini gerçekleştirir. Dosyaları veya klasörleri mutlak veya göreli bir yolla ekler. Tüm alt klasörlerdeki belgeler indekslenir.

```csharp
public void Add(string[] paths)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| paths | String[] | Dizinlenecek dosya veya klasörlerin yolları. |

### Örnekler

Örnek, belgelerin bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Belgeleri belirtilen yollarda indeksleme
```

### Ayrıca bakınız

* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

İndeksleme işlemini gerçekleştirir. Dosyaları veya klasörleri mutlak veya göreli bir yolla ekler. Tüm alt klasörlerdeki belgeler indekslenir.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| paths | String[] | Dizinlenecek dosya veya klasörlerin yolları. |
| options | IndexingOptions | İndeksleme seçenekleri. |

### Örnekler

Örnek, belgelerin belirli dizin oluşturma seçenekleriyle bir dizine nasıl ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // İndeksleme dizilerinin sayısını ayarlama
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Belgeleri belirtilen yollarda indeksleme
```

### Ayrıca bakınız

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

İndeksleme işlemini gerçekleştirir. Dosya sisteminden, akıştan veya yapıdan belgeler ekler.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| documents | Document[] | Dosya sisteminden, akıştan veya yapıdan belgeler. |
| options | IndexingOptions | İndeksleme seçenekleri. |

### Ayrıca bakınız

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

İndeksleme işlemini gerçekleştirir. Ayıklanan verileri indekse ekler.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| data | ExtractedData[] | Çıkarılan veriler. |
| options | IndexingOptions | İndeksleme seçenekleri. |

### Ayrıca bakınız

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ad alanı [GroupDocs.Search](../../index)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
