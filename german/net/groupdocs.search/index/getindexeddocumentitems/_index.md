---
title: "GetIndexedDocumentItems"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Gibt ein Array verschachtelter Elemente des angegebenen Dokuments für Container‑Dokumente wie ZIP, OST, PST zurück."
type: docs
weight: 160
url: /de/net/groupdocs.search/index/getindexeddocumentitems/
---
## Index.GetIndexedDocumentItems method

Gibt ein Array verschachtelter Elemente des angegebenen Dokuments zurück (für Container-Dokumente wie ZIP, OST, PST).

```csharp
public DocumentInfo[] GetIndexedDocumentItems(DocumentInfo documentInfo)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| documentInfo | DocumentInfo | Die Dokumentinformationen. |

### Rückgabewert

Ein Array von Dokumentelementen.

### Beispiele

Das Beispiel zeigt, wie eine Liste von Elementen eines indizierten Dokuments aus einem Index abgerufen wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);
 
// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
 
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.GetIndexedDocuments();
for (int i = 0; i < documents.Length; i++)
{
    DocumentInfo document = documents[i];
    Console.WriteLine(document.FilePath);
    DocumentInfo[] items = index.GetIndexedDocumentItems(document); // Getting list of document items
    for (int j = 0; j < items.Length; j++)
    {
        DocumentInfo item = items[j];
        Console.WriteLine("\t" + item.InnerPath);
    }
}
```

### Siehe auch

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
