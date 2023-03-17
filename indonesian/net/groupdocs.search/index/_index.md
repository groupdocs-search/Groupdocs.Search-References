---
title: Index
second_title: GroupDocs.Mencari Referensi .NET API
description: Mewakili kelas utama untuk mengindeks dokumen dan menelusurinya.
type: docs
weight: 680
url: /id/net/groupdocs.search/index/
---
## Index class

Mewakili kelas utama untuk mengindeks dokumen dan menelusurinya.

```csharp
public class Index : IDisposable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Index](index#constructor)() | Menginisialisasi instance baru dari[`Index`](../index) kelas dalam memori. |
| [Index](index#constructor_1)(IndexSettings) | Menginisialisasi instance baru dari[`Index`](../index) kelas dalam memori dengan pengaturan indeks tertentu. |
| [Index](index#constructor_2)(string) | Menginisialisasi instance baru dari[`Index`](../index) class. Membuat baru atau membuka indeks yang ada pada disk. |
| [Index](index#constructor_3)(string, bool) | Menginisialisasi instance baru dari[`Index`](../index) class. Memuat indeks yang ada dari disk if*overwriteIfExists* adalah`PALSU`; sebaliknya membuat indeks baru pada disk. |
| [Index](index#constructor_4)(string, IndexSettings) | Menginisialisasi instance baru dari[`Index`](../index) class. Membuat indeks baru dengan pengaturan tertentu atau membuka indeks yang ada di disk. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Menginisialisasi instance baru dari[`Index`](../index) class. Memuat indeks yang ada dari disk if*overwriteIfExists* adalah`PALSU` ; membuat indeks baru pada disk dengan pengaturan indeks tertentu sebaliknya. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Mendapatkan repositori kamus. |
| [Events](../../groupdocs.search/index/events) { get; } | Mendapatkan hub acara untuk berlangganan acara. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Mendapat informasi dasar tentang indeks. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Mendapatkan pengaturan indeks. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Mendapat objek repositori indeks jika indeks terkandung di dalamnya. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan dokumen dari sistem file, aliran, atau struktur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan data yang diekstraksi ke indeks. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Menerapkan kumpulan perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa pengindeksan ulang selama operasi pembaruan. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Menghapus file atau folder yang diindeks dari indeks. Kemudian perbarui indeks tanpa jalur yang dihapus. Perhatikan bahwa setiap dokumen tidak dapat dihapus dari indeks jika ditambahkan ke indeks sebagai bagian dari folder. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Menghapus dokumen yang diindeks dari aliran atau struktur. Kemudian perbarui indeks tanpa menghapus dokumen. |
| [Dispose](../../groupdocs.search/index/dispose)() | Merilis semua sumber daya yang digunakan oleh[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Mendapat semua atribut yang terkait dengan dokumen terindeks yang ditentukan. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Menghasilkan teks berformat HTML untuk dokumen yang diindeks dan mentransfernya melalui adaptor keluaran. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Menghasilkan teks berformat HTML untuk dokumen yang diindeks dan mentransfernya melalui adaptor keluaran. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Mendapat array item bersarang dari dokumen yang ditentukan (untuk dokumen kontainer seperti ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Mendapat array dari semua dokumen yang diindeks. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Mendapat larik jalur yang diindeks - dokumen atau folder. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Mendapat laporan tentang operasi pengindeksan. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Mendapat laporan tentang operasi pencarian. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Menggabungkan indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks lain tidak akan diubah. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Menggabungkan indeks dari repositori indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks dalam repositori tidak akan diubah. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Meneruskan objek notifikasi yang ditentukan ke indeks untuk melakukan notifikasi. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu sama lain. Operasi ini meningkatkan kinerja pencarian. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu sama lain. Operasi ini meningkatkan kinerja pencarian. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Mencari di index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Mencari di index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Melakukan pencarian gambar terbalik di indeks. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Mencari di index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Mencari di index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. Menambahkan file baru yang telah ditambahkan ke folder yang diindeks. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Mengindeks ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. Menambahkan file baru yang telah ditambahkan ke folder yang diindeks. |

### Perkataan

**Belajarlah lagi**

* [Membuat indeks](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Pengindeksan](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Mencari](https://docs.groupdocs.com/display/searchnet/Searching)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchResult result = index.Search(query); // Mencari di index
```

### Lihat juga

* ruang nama [GroupDocs.Search](../../groupdocs.search)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
