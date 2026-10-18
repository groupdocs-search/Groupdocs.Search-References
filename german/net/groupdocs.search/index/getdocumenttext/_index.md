---
title: "GetDocumentText"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erzeugt den Text eines indexierten Dokuments und leitet ihn über einen Ausgabeadapter weiter."
type: docs
weight: 140
url: /de/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

Erzeugt den Text eines indexierten Dokuments und leitet ihn über einen Ausgabeadapter weiter.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| documentInfo | DocumentInfo | Die Informationen des indizierten Dokuments. |
| adapter | OutputAdapter | Der Ausgabeadapter. |

### Beispiele

Das Beispiel zeigt, wie der Text eines indizierten Dokuments aus einem Index abgerufen wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);
 
// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
 
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// Abrufen eines Dokumenttexts
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### Siehe auch

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

Erzeugt HTML-formatierten Text für ein indexiertes Dokument und überträgt ihn über den Ausgabeadapter.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| documentInfo | DocumentInfo | Die Informationen des indizierten Dokuments. |
| adapter | OutputAdapter | Der Ausgabeadapter. |
| Optionen | TextOptions | Die Optionen zum Abrufen des Textes. |

### Siehe auch

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
