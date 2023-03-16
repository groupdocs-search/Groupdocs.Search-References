---
title: IndexRepository
second_title: GroupDocs.Mencari Referensi .NET API
description: Merupakan wadah untuk menggabungkan beberapa indeks dan melakukan operasi umum padanya.
type: docs
weight: 690
url: /id/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Merupakan wadah untuk menggabungkan beberapa indeks dan melakukan operasi umum padanya.

```csharp
public class IndexRepository : IDisposable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [IndexRepository](indexrepository)() | Menginisialisasi instance baru dari[`IndexRepository`](../indexrepository) kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Mendapatkan hub acara untuk berlangganan acara. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Mendapat indeks yang terkandung di dalamnya[`IndexRepository`](../indexrepository) . |

## Metode

| Nama | Keterangan |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Menambahkan indeks ke repositori indeks. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Membuka dan menambahkan indeks ke repositori indeks. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Membuat indeks baru di memori. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Membuat indeks baru di memori. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Membuat indeks baru pada disk. Folder indeks akan dibersihkan sebelum pembuatan indeks. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Membuat indeks baru pada disk. Folder indeks akan dibersihkan sebelum pembuatan indeks. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Merilis semua sumber daya yang digunakan oleh[`IndexRepository`](../indexrepository) . |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Mencari di semua indeks repositori. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Mencari di semua indeks repositori. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Mencari di semua indeks repositori. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Mencari di semua indeks repositori. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Memperbarui semua indeks di repositori. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Memperbarui semua indeks di repositori. |

### Perkataan

**Belajarlah lagi**

* [Cari repositori indeks](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Memuat indeks yang ada
repository.AddToRepository(indexFolder2); // Memuat indeks lain yang ada

SearchResult result = repository.Search(query); // Mencari di indeks repositori
```

### Lihat juga

* ruang nama [GroupDocs.Search](../../groupdocs.search)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->