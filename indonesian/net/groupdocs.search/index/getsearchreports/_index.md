---
title: GetSearchReports
second_title: GroupDocs.Mencari Referensi .NET API
description: Mendapat laporan tentang operasi pencarian.
type: docs
weight: 170
url: /id/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

Mendapat laporan tentang operasi pencarian.

```csharp
public SearchReport[] GetSearchReports()
```

### Nilai Pengembalian

Laporan pencarian.

### Contoh

Contoh menunjukkan cara mendapatkan laporan penelusuran.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query1 = "Einstein";
string query2 = "Newton";

Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.Add(documentsFolder); // Pengindeksan dokumen dari folder yang ditentukan

SearchResult result1 = index.Search(query1); // Mencari
SearchResult result2 = index.Search(query2);
SearchResult result3 = index.Search(query1 + " & " + query2);

SearchReport[] reports = index.GetSearchReports(); // Mendapatkan laporan pencarian
```

### Lihat juga

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* ruang nama [GroupDocs.Search](../../index)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
