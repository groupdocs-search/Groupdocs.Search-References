---
title: "Ajouter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Effectue une opération d'indexation. L'indexation uniquement à partir du flux et de la structure est prise en charge."
type: docs
weight: 20
url: /fr/net/groupdocs.search.scaling/indexer/add/
---
## Add(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) {#add}

Effectue une opération d'indexation. L'indexation uniquement à partir du flux et de la structure est prise en charge.

```csharp
public void Add(IList<Document> documents, IList<string> passwords, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documents | IList`1 | Les documents provenant du flux ou de la structure. |
| mots de passe | IList`1 | Les mots de passe du document. |
| options | IndexingOptions | Les options d'ajout. |

### Voir aussi

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## Add(IList&lt;ExtractedData&gt;, IndexingOptions) {#add_1}

Effectue une opération d'indexation. Ajoute les données extraites au réseau de recherche.

```csharp
public void Add(IList<ExtractedData> data, IndexingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| données | IList`1 | Les données extraites. |
| options | IndexingOptions | Les options d'indexation. |

### Voir aussi

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
