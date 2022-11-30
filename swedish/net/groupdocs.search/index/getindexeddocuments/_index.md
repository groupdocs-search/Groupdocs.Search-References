---
title: GetIndexedDocuments
second_title: GroupDocs.Search efter .NET API Reference
description: Får en uppsättning av alla indexerade dokument.
type: docs
weight: 140
url: /sv/net/groupdocs.search/index/getindexeddocuments/
---
## Index.GetIndexedDocuments method

Får en uppsättning av alla indexerade dokument.

```csharp
public DocumentInfo[] GetIndexedDocuments()
```

### Returvärde

En uppsättning av alla indexerade dokument.

### Exempel

Exemplet visar hur man får en lista över indexerade dokument från ett index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
 
// Indexering av dokument från den angivna mappen
index.Add(documentsFolder);
 
// Hämta lista över indexerade dokument
DocumentInfo[] documents = index.GetIndexedDocuments();
```

### Se även

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->