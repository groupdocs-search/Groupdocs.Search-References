---
title: "HighlightOptions"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Menyediakan opsi untuk menyorot istilah yang ditemukan."
type: docs
weight: 910
url: /id/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Menyediakan opsi untuk menyorot istilah yang ditemukan.

```csharp
public class HighlightOptions : TextOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Menginisialisasi instance baru dari kelas [`HighlightOptions`](../highlightoptions). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Mendapatkan atau mengatur bidang dokumen tambahan yang digunakan untuk pengindeksan. Nilai default adalah `null`. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan mendeteksi pengkodean secara otomatis atau tidak. Nilai default adalah `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Mendapatkan atau mengatur objek pembatalan. Nilai default adalah `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Mendapatkan atau mengatur ekstraktor teks khusus yang digunakan untuk pengindeksan. Nilai default adalah `null`. Perhatikan bahwa nilai ini hanya digunakan jika teks dokumen tidak disimpan ke dalam indeks. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Mendapatkan atau mengatur pengkodean yang digunakan untuk mengekstrak teks dari dokumen teks. Nilai default adalah `null`, yang berarti pengkodean default UTF-8 digunakan. Jika AutoDetectEncoding `true` maka nilai ini digunakan sebagai pengkodean default. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tag Head dihasilkan dalam HTML output. Nilai default adalah `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Mendapatkan atau mengatur warna yang digunakan untuk menyorot kemunculan. Nilai default adalah #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Mendapatkan opsi pengindeksan gambar untuk pencarian gambar terbalik. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Mendapatkan opsi untuk mengindeks bidang metadata. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Mendapatkan opsi untuk pemrosesan OCR dan pengindeksan teks yang dikenali. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Mendapatkan atau mengatur tag akhir penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Mendapatkan atau mengatur tag awal penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Mendapatkan atau mengatur jumlah maksimum kata dalam fragmen teks setelah kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Mendapatkan atau mengatur jumlah maksimum kata dalam fragmen teks sebelum kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Mendapatkan atau mengatur jumlah maksimum kata dalam fragmen teks. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah proses harus menggunakan SeBackupPrivilege dan FILE_FLAG_BACKUP_SEMANTICS untuk mengakses file dan direktori. Nilai default adalah `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. Nilai default adalah `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah mode mentah digunakan untuk ekstraksi teks bila memungkinkan. Nilai default adalah `false`. Mode mentah dapat secara signifikan meningkatkan kecepatan pengindeksan, tetapi mode normal meningkatkan pemformatan teks yang diekstrak. |

### Catatan

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Lihat Juga

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
