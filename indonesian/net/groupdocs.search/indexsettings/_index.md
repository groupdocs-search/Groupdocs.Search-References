---
title: IndexSettings
second_title: GroupDocs.Mencari Referensi .NET API
description: Merupakan pengaturan indeks yang memungkinkan untuk menyesuaikan operasi pengindeksan.
type: docs
weight: 700
url: /id/net/groupdocs.search/indexsettings/
---
## IndexSettings class

Merupakan pengaturan indeks yang memungkinkan untuk menyesuaikan operasi pengindeksan.

```csharp
public class IndexSettings
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [IndexSettings](indexsettings)() | Menginisialisasi instance baru dari[`IndexSettings`](../indexsettings) kelas. |

## Properti

| Nama | Keterangan |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search/indexsettings/autodetectencoding) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah akan mendeteksi penyandian secara otomatis atau tidak. Nilai defaultnya adalah`PALSU` . |
| [CustomExtractors](../../groupdocs.search/indexsettings/customextractors) { get; } | Mendapat koleksi ekstraktor khusus. |
| [DocumentFilter](../../groupdocs.search/indexsettings/documentfilter) { get; set; } | Mendapat atau menyetel filter dokumen. The[`DocumentFilter`](./documentfilter) bekerja pada logika inklusi. Gunakan[`DocumentFilter`](../../groupdocs.search.options/documentfilter) kelas untuk pembuatan instance filter dokumen. Nilai defaultnya adalah`batal` , artinya semua dokumen yang ditambahkan akan diindeks. |
| [IndexType](../../groupdocs.search/indexsettings/indextype) { get; set; } | Mendapat atau menetapkan jenis indeks. Nilai defaultnya adalahNormalIndex . |
| [InMemoryIndex](../../groupdocs.search/indexsettings/inmemoryindex) { get; } | Mendapat nilai yang menunjukkan apakah indeks disimpan di memori atau di disk. |
| [Logger](../../groupdocs.search/indexsettings/logger) { get; set; } | Mendapat atau menyetel logger yang digunakan untuk mencatat peristiwa dan kesalahan dalam indeks. Perhatikan bahwa logger tidak disimpan dan harus dibuat dan ditetapkan setiap kali indeks dibuat atau dimuat. |
| [MaxIndexingReportCount](../../groupdocs.search/indexsettings/maxindexingreportcount) { get; set; } | Mendapat atau menetapkan jumlah maksimum laporan pengindeksan. Nilai defaultnya adalah`5` . |
| [MaxSearchReportCount](../../groupdocs.search/indexsettings/maxsearchreportcount) { get; set; } | Mendapatkan atau menyetel jumlah maksimum laporan pencarian. Nilai defaultnya adalah`10` . |
| [SearchThreads](../../groupdocs.search/indexsettings/searchthreads) { get; set; } | Mendapat atau menetapkan jumlah utas yang digunakan untuk pencarian. Nilai defaultnya adalahDefault , artinya pencarian akan dilakukan dengan menggunakan jumlah thread yang sama dengan jumlah core prosesor. |
| [TextStorageSettings](../../groupdocs.search/indexsettings/textstoragesettings) { get; set; } | Mendapat atau mengatur pengaturan penyimpanan teks. Nilai defaultnya adalah`batal` , artinya teks dokumen tidak disimpan. |
| [UseCharacterReplacements](../../groupdocs.search/indexsettings/usecharacterreplacements) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah akan menggunakan penggantian karakter atau tidak. Nilai defaultnya adalah`PALSU` . |
| [UseRawTextExtraction](../../groupdocs.search/indexsettings/userawtextextraction) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks jika memungkinkan. Nilai defaultnya adalah`BENAR` . Mode mentah dapat meningkatkan kecepatan pengindeksan secara signifikan, tetapi mode normal meningkatkan pemformatan teks yang diekstraksi. |
| [UseStopWords](../../groupdocs.search/indexsettings/usestopwords) { get; set; } | Mendapat atau menetapkan nilai yang menunjukkan apakah akan menggunakan kata berhenti atau tidak. Nilai defaultnya adalah`BENAR` . |

### Perkataan

**Belajarlah lagi**

* [Pengaturan indeks pencarian](https://docs.groupdocs.com/display/searchnet/Search+index+settings)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex; // Mengatur tipe indeks

Index index = new Index(indexFolder, settings); // Membuat indeks
```

### Lihat juga

* ruang nama [GroupDocs.Search](../../groupdocs.search)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
