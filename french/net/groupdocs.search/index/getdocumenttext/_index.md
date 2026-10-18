---
title: "GetDocumentText"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Génère le texte d'un document indexé et le transmet via un adaptateur de sortie."
type: docs
weight: 140
url: /fr/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

Génère le texte d'un document indexé et le transmet via un adaptateur de sortie.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | DocumentInfo | Les informations du document indexé. |
| adapter | OutputAdapter | L'adaptateur de sortie. |

### Exemples

L'exemple montre comment obtenir le texte d'un document indexé à partir d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
 
// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
 
// Obtention de la liste des documents indexés
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// Obtention du texte d'un document
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### Voir aussi

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

Génère du texte formaté en HTML pour le document indexé et le transfère via l'adaptateur de sortie.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | DocumentInfo | Les informations du document indexé. |
| adapter | OutputAdapter | L'adaptateur de sortie. |
| options | TextOptions | Les options de récupération du texte. |

### Voir aussi

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
