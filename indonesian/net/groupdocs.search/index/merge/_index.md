---
title: Merge
second_title: GroupDocs.Mencari Referensi .NET API
description: Menggabungkan indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks lain tidak akan diubah.
type: docs
weight: 190
url: /id/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Menggabungkan indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks lain tidak akan diubah.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| index | Index | Indeks yang akan digabungkan. |
| options | MergeOptions | Opsi penggabungan. |

### Perkataan

Jika indeks lain memiliki versi sebelumnya, itu harus diperbarui sebelum digabungkan[`IndexUpdater`](../../indexupdater) .

### Contoh

Contoh menunjukkan cara menggabungkan indeks ke dalam indeks saat ini.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

Index index1 = new Index(indexFolder1); // Membuat indeks1
index1.Add(documentsFolder1); // Pengindeksan dokumen

Index index2 = new Index(indexFolder2); // Membuat indeks2
index2.Add(documentsFolder2); // Pengindeksan dokumen

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Membuat objek pembatalan

// Menggabungkan indeks2 ke dalam indeks1. Perhatikan bahwa file index2 tidak akan diubah.
index1.Merge(index2, options);
```

### Lihat juga

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Menggabungkan indeks dari repositori indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks dalam repositori tidak akan diubah.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| repository | IndexRepository | Repositori indeks untuk digabungkan. |
| options | MergeOptions | Opsi penggabungan. |

### Perkataan

Jika indeks lain memiliki versi sebelumnya, mereka harus diperbarui sebelum digabungkan[`IndexUpdater`](../../indexupdater) .

### Contoh

Contoh menunjukkan cara menggabungkan repositori indeks ke dalam indeks saat ini.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string indexFolder3 = @"c:\MyIndex3\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index1 = new Index(indexFolder1); // Membuat indeks1
index1.Add(documentsFolder1); // Pengindeksan dokumen

IndexRepository repository = new IndexRepository(); // Membuat repositori indeks

Index index2 = repository.Create(indexFolder2); // Membuat indeks2
index2.Add(documentsFolder2); // Pengindeksan dokumen

Index index3 = repository.Create(indexFolder3); // Membuat indeks3
index3.Add(documentsFolder3); // Pengindeksan dokumen

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Membuat objek pembatalan

// Menggabungkan semua indeks dalam repositori indeks ke dalam indeks1. Perhatikan bahwa index2 dan index3 tidak akan diubah.
index1.Merge(repository, options);
```

### Lihat juga

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->