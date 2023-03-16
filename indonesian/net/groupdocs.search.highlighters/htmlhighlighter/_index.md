---
title: HtmlHighlighter
second_title: GroupDocs.Mencari Referensi .NET API
description: Mewakili penyorot hasil pencarian yang menyorot hasil pencarian di seluruh teks dokumen yang diformat dalam HTML.
type: docs
weight: 670
url: /id/net/groupdocs.search.highlighters/htmlhighlighter/
---
## HtmlHighlighter class

Mewakili penyorot hasil pencarian yang menyorot hasil pencarian di seluruh teks dokumen yang diformat dalam HTML.

```csharp
[Obsolete("Please, use the DocumentHighlighter class instead.")]
public class HtmlHighlighter : Highlighter
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Mendapatkan format keluaran. |

### Perkataan

**Belajarlah lagi**

* [Menyoroti hasil pencarian](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Contoh

Contoh ini menunjukkan penggunaan umum kelas.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Membuat indeks
Index index = new Index(indexFolder);

// Pengindeksan dokumen dari folder yang ditentukan
index.Add(documentsFolder);

// Cari fase 'Teori Relativitas'
SearchResult result = index.Search("\"Theory of Relativity\"");

// Menyoroti kata-kata yang ditemukan dalam teks dokumen
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new HtmlHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Lihat juga

* class [Highlighter](../highlighter)
* ruang nama [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* perakitan [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->