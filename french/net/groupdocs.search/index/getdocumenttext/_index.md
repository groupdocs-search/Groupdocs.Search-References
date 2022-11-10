---
title: GetDocumentText
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Génère du texte au format HTML pour le document indexé et le transfère via ladaptateur de sortie.
type: docs
weight: 120
url: /fr/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

Génère du texte au format HTML pour le document indexé et le transfère via l'adaptateur de sortie.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| documentInfo | DocumentInfo | Les informations sur le document indexé. |
| adapter | OutputAdapter | L'adaptateur de sortie. |

### Exemples

L'exemple montre comment obtenir le texte d'un document indexé à partir d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
 
// Indexation des documents du dossier spécifié
index.Add(documentsFolder);
 
// Récupère la liste des documents indexés
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// Obtenir un texte de document
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### Voir également

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

Génère du texte au format HTML pour le document indexé et le transfère via l'adaptateur de sortie.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| documentInfo | DocumentInfo | Les informations sur le document indexé. |
| adapter | OutputAdapter | L'adaptateur de sortie. |
| options | TextOptions | Les options de récupération de texte. |

### Voir également

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->