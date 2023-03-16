---
title: Add
second_title: GroupDocs.Mencari Referensi .NET API
description: Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.
type: docs
weight: 70
url: /id/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur ke file atau folder yang akan diindeks. |

### Contoh

Contoh menunjukkan cara menambahkan dokumen ke indeks.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(folderPath); // Mengindeks dokumen di folder yang ditentukan
index.Add(filePath); // Mengindeks dokumen yang ditentukan
```

### Lihat juga

* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur ke file atau folder yang akan diindeks. |
| options | IndexingOptions | Opsi pengindeksan. |

### Contoh

Contoh menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Mengatur jumlah utas pengindeksan
index.Add(folderPath, options); // Mengindeks dokumen di folder yang ditentukan
index.Add(filePath, options); // Mengindeks dokumen yang ditentukan
```

### Lihat juga

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string[] paths)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| paths | String[] | Jalur ke file atau folder yang akan diindeks. |

### Contoh

Contoh menunjukkan cara menambahkan dokumen ke indeks.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Pengindeksan dokumen di jalur yang ditentukan
```

### Lihat juga

* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| paths | String[] | Jalur ke file atau folder yang akan diindeks. |
| options | IndexingOptions | Opsi pengindeksan. |

### Contoh

Contoh menunjukkan cara menambahkan dokumen ke indeks dengan opsi pengindeksan tertentu.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Mengatur jumlah utas pengindeksan
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Pengindeksan dokumen di jalur yang ditentukan
```

### Lihat juga

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Melakukan operasi pengindeksan. Menambahkan dokumen dari sistem file, aliran, atau struktur.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| documents | Document[] | Dokumen-dokumen dari sistem file, aliran atau struktur. |
| options | IndexingOptions | Opsi pengindeksan. |

### Lihat juga

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Melakukan operasi pengindeksan. Menambahkan data yang diekstraksi ke indeks.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| data | ExtractedData[] | Data yang diekstrak. |
| options | IndexingOptions | Opsi pengindeksan. |

### Lihat juga

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
