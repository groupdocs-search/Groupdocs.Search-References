---
title: "Index"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Mewakili kelas utama untuk mengindeks dokumen dan mencari di dalamnya."
type: docs
weight: 700
url: /id/net/groupdocs.search/index/
---
## Index class

Mewakili kelas utama untuk mengindeks dokumen dan mencari di dalamnya.

```csharp
public class Index : IDisposable
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Index](index#constructor)() | Menginisialisasi sebuah instance baru dari kelas [`Index`](../index) di memori. |
| [Index](index#constructor_1)(IndexSettings) | Menginisialisasi sebuah instance baru dari kelas [`Index`](../index) di memori dengan pengaturan indeks tertentu. |
| [Index](index#constructor_2)(string) | Menginisialisasi sebuah instance baru dari kelas [`Index`](../index). Membuat indeks baru atau membuka indeks yang sudah ada di disk. |
| [Index](index#constructor_3)(string, bool) | Menginisialisasi sebuah instance baru dari kelas [`Index`](../index). Memuat indeks yang ada dari disk jika *overwriteIfExists* adalah `false`; membuat indeks baru di disk jika tidak. |
| [Index](index#constructor_4)(string, IndexSettings) | Menginisialisasi instance baru dari kelas [`Index`](../index). Membuat indeks baru dengan pengaturan tertentu atau membuka indeks yang sudah ada di disk. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Menginisialisasi instance baru dari kelas [`Index`](../index). Memuat indeks yang sudah ada dari disk jika *overwriteIfExists* bernilai `false`; membuat indeks baru di disk dengan pengaturan indeks tertentu jika tidak. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Mendapatkan repositori kamus. |
| [Events](../../groupdocs.search/index/events) { get; } | Mendapatkan hub acara untuk berlangganan ke acara. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Mendapatkan informasi dasar tentang indeks. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Mendapatkan pengaturan indeks. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Mendapatkan objek repositori indeks jika indeks berada di dalamnya. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Mengambil seluruh indeks ke memori. Setiap perubahan pada indeks tidak secara otomatis disimpan ke folder asli. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Mengambil seluruh indeks ke memori. Setiap perubahan pada indeks tidak secara otomatis disimpan ke folder asli. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Melakukan operasi pengindeksan. Menambahkan sebuah file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan dokumen dari sistem file, aliran, atau struktur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan data yang diekstrak ke indeks. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan sebuah file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Melakukan operasi pengindeksan. Menambahkan file atau folder dengan jalur absolut atau relatif. Dokumen dari semua subfolder akan diindeks. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Menerapkan batch perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa melakukan pengindeksan ulang selama operasi pembaruan. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Memeriksa indeks untuk file segmen yang rusak pada disk. Metode ini memperbaiki fungsi indeks bila terdapat segmen yang rusak, jika *fixIndexFunctionality* bernilai true; tidak memperbaiki jika tidak. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Menghapus file atau folder yang diindeks dari indeks. Kemudian memperbarui indeks tanpa jalur yang dihapus. Perhatikan bahwa dokumen individu tidak dapat dihapus dari indeks jika ditambahkan ke indeks sebagai bagian dari sebuah folder. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Menghapus dokumen yang diindeks dari aliran atau struktur. Kemudian memperbarui indeks tanpa dokumen yang dihapus. |
| [Dispose](../../groupdocs.search/index/dispose)() | Melepaskan semua sumber daya yang digunakan oleh [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Mendapatkan semua atribut yang terkait dengan dokumen terindeks yang ditentukan. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Menghasilkan teks dari dokumen terindeks dan meneruskannya melalui adaptor output. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Menghasilkan teks berformat HTML untuk dokumen terindeks dan mentransfernya melalui adaptor output. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Mendapatkan dokumen terindeks berdasarkan kunci dokumen. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Mendapatkan array item bersarang dari dokumen yang ditentukan (untuk dokumen kontainer seperti ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Mendapatkan array semua dokumen terindeks. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Mendapatkan array jalur terindeks - dokumen atau folder. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Mendapatkan laporan tentang operasi pengindeksan. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Mendapatkan laporan tentang operasi pencarian. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Menggabungkan indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks lain tidak akan diubah. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Menggabungkan indeks dari repositori indeks yang ditentukan ke dalam indeks saat ini. Perhatikan bahwa indeks di dalam repositori tidak akan diubah. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Menyampaikan objek notifikasi yang ditentukan ke indeks untuk melakukan notifikasi. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu sama lain. Operasi ini meningkatkan kinerja pencarian. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu sama lain. Operasi ini meningkatkan kinerja pencarian. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Menyimpan indeks dalam memori ke disk. Juga menyimpan indeks reguler ke folder lain. Tidak mengubah pengaturan indeks ini. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Mencari dalam indeks. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Mencari dalam indeks. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Melakukan pencarian gambar terbalik dalam indeks. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Mencari dalam indeks. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Mencari dalam indeks. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Melanjutkan pencarian potongan yang dimulai dengan metode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Menyusun ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. Menambahkan file baru yang telah ditambahkan ke folder yang diindeks. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Menyusun ulang dokumen yang telah diubah atau dihapus sejak pembaruan terakhir. Menambahkan file baru yang telah ditambahkan ke folder yang diindeks. |

### Catatan

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Contoh

Contoh ini menunjukkan penggunaan tipikal dari kelas tersebut.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Lihat Juga

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
