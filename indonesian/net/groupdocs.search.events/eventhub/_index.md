---
title: EventHub
second_title: GroupDocs.Mencari Referensi .NET API
description: Menyediakan peristiwa indeks untuk berlangganan.
type: docs
weight: 510
url: /id/net/groupdocs.search.events/eventhub/
---
## EventHub class

Menyediakan peristiwa indeks untuk berlangganan.

```csharp
public class EventHub
```

## Acara

| Nama | Keterangan |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search.events/eventhub/erroroccurred) | Terjadi ketika kesalahan terjadi selama operasi indeks. |
| event [FileIndexing](../../groupdocs.search.events/eventhub/fileindexing) | Terjadi saat dokumen akan diindeks. |
| event [ImagePreparing](../../groupdocs.search.events/eventhub/imagepreparing) | Terjadi saat gambar akan disiapkan untuk pengindeksan. |
| event [OperationFinished](../../groupdocs.search.events/eventhub/operationfinished) | Terjadi saat operasi indeks selesai. |
| event [OperationProgressChanged](../../groupdocs.search.events/eventhub/operationprogresschanged) | Terjadi saat kemajuan operasi pengindeksan atau pembaruan diubah. |
| event [PasswordRequired](../../groupdocs.search.events/eventhub/passwordrequired) | Terjadi ketika dokumen membutuhkan kata sandi untuk dibuka. |
| event [SearchPhaseCompleted](../../groupdocs.search.events/eventhub/searchphasecompleted) | Terjadi saat fase pencarian selesai. |
| event [StatusChanged](../../groupdocs.search.events/eventhub/statuschanged) | Terjadi saat status indeks berubah. |

### Perkataan

**Belajarlah lagi**

* [Cari indeks acara](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Contoh

Contoh menunjukkan penggunaan umum antarmuka.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Membuat indeks
Index index = new Index(indexFolder);

// Berlangganan ke acara tersebut
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Pengindeksan dokumen dari folder yang ditentukan
index.Add(documentsFolder);

// Mencari di index
SearchResult result = index.Search(query);
```

### Lihat juga

* ruang nama [GroupDocs.Search.Events](../../groupdocs.search.events)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->