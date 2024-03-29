---
title: DocumentFilter
second_title: GroupDocs.Mencari Referensi .NET API
description: Mendapat atau menyetel filter dokumen. TheDocumentFiltergroupdocs.search/indexsettings/documentfilter bekerja pada logika inklusi. GunakanDocumentFiltergroupdocs.search.options/documentfilter kelas untuk pembuatan instance filter dokumen. Nilai defaultnya adalahbatal  artinya semua dokumen yang ditambahkan akan diindeks.
type: docs
weight: 40
url: /id/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

Mendapat atau menyetel filter dokumen. The`DocumentFilter` bekerja pada logika inklusi. Gunakan[`DocumentFilter`](../../../groupdocs.search.options/documentfilter) kelas untuk pembuatan instance filter dokumen. Nilai defaultnya adalah`batal` , artinya semua dokumen yang ditambahkan akan diindeks.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### Nilai properti

Penyaring dokumen.

### Contoh

Contoh menunjukkan cara menyetel filter dokumen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Membuat filter yang melewatkan dokumen dengan ekstensi '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Membuat filter ekstensi file
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // Membalik filter ekstensi file
settings.DocumentFilter = invertedFilter;

// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder, settings);

// Pengindeksan dokumen
index.Add(documentsFolder);

// Mencari
SearchResult result = index.Search("Einstein");
```

### Lihat juga

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* ruang nama [GroupDocs.Search](../../indexsettings)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
