---
title: "GetIndexedDocuments"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Gibt ein Array aller indizierten Dokumente zurück."
type: docs
weight: 170
url: /de/net/groupdocs.search/index/getindexeddocuments/
---
## Index.GetIndexedDocuments method

Gibt ein Array aller indizierten Dokumente zurück.

```csharp
public DocumentInfo[] GetIndexedDocuments()
```

### Rückgabewert

Ein Array aller indizierten Dokumente.

### Beispiele

Das Beispiel zeigt, wie man eine Liste indizierter Dokumente aus einem Index erhält.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);
 
// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
 
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.GetIndexedDocuments();
```

### Siehe auch

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
