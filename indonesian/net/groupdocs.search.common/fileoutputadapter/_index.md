---
title: FileOutputAdapter
second_title: GroupDocs.Mencari Referensi .NET API
description: Mewakili adaptor keluaran yang mengumpulkan keluaran ke dalam file.
type: docs
weight: 150
url: /id/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

Mewakili adaptor keluaran yang mengumpulkan keluaran ke dalam file.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter#constructor)(OutputFormat, string) | Menginisialisasi instance baru dari[`FileOutputAdapter`](../fileoutputadapter) kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | Mendapat jalur file keluaran. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Mendapatkan format keluaran. |

### Perkataan

**Belajarlah lagi**

* [Adaptor keluaran](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan

index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

DocumentInfo[] documents = index.GetIndexedDocuments(); // Mendapatkan informasi tentang dokumen yang diindeks

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // Membuat adaptor output file
index.GetDocumentText(documents[0], adapter); // Menghasilkan teks dokumen ke dalam file keluaran
```

### Lihat juga

* class [OutputAdapter](../outputadapter)
* ruang nama [GroupDocs.Search.Common](../../groupdocs.search.common)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->