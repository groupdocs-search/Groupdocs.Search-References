---
title: "Add"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Melakukan operasi pengindeksan. Menambahkan sebuah file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks."
type: docs
weight: 80
url: /id/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Melakukan operasi pengindeksan. Menambahkan sebuah file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string path)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file atau folder yang akan diindeks. |

### Contoh

Contoh ini menunjukkan cara menambahkan dokumen ke indeks.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Lihat Juga

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Melakukan operasi pengindeksan. Menambahkan sebuah file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file atau folder yang akan diindeks. |
| opsi | IndexingOptions | Opsi pengindeksan. |

### Contoh

Contoh ini menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

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

### Lihat Juga

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| jalur | String[] | Jalur ke file atau folder yang akan diindeks. |

### Contoh

Contoh ini menunjukkan cara menambahkan dokumen ke indeks.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Lihat Juga

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| jalur | String[] | Jalur ke file atau folder yang akan diindeks. |
| opsi | IndexingOptions | Opsi pengindeksan. |

### Contoh

Contoh ini menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

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

### Lihat Juga

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Melakukan operasi pengindeksan. Menambahkan dokumen dari sistem file, aliran, atau struktur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Document[] | Dokumen dari sistem file, stream, atau struktur. |
| opsi | IndexingOptions | Opsi pengindeksan. |

### Lihat Juga

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Melakukan operasi pengindeksan. Menambahkan data yang diekstrak ke indeks.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| data | ExtractedData[] | Data yang diekstrak. |
| opsi | IndexingOptions | Opsi pengindeksan. |

### Lihat Juga

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
