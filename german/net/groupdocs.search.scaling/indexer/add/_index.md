---
title: "Hinzufügen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Führt einen Indexierungsvorgang aus. Nur das Indexieren von Stream und Struktur wird unterstützt."
type: docs
weight: 20
url: /de/net/groupdocs.search.scaling/indexer/add/
---
## Add(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) {#add}

Führt einen Indexierungsvorgang aus. Nur das Indexieren von Stream und Struktur wird unterstützt.

```csharp
public void Add(IList<Document> documents, IList<string> passwords, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Dokumente | IList`1 | Die Dokumente aus dem Stream oder der Struktur. |
| Passwörter | IList`1 | Die Dokumentpasswörter. |
| Optionen | IndexingOptions | Die Hinzufügen-Optionen. |

### Siehe auch

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## Add(IList&lt;ExtractedData&gt;, IndexingOptions) {#add_1}

Führt einen Indexierungsvorgang aus. Fügt die extrahierten Daten dem Suchnetzwerk hinzu.

```csharp
public void Add(IList<ExtractedData> data, IndexingOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Daten | IList`1 | Die extrahierten Daten. |
| Optionen | IndexingOptions | Die Indexierungsoptionen. |

### Siehe auch

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
