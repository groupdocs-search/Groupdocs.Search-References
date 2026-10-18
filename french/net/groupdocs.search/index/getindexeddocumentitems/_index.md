---
title: "GetIndexedDocumentItems"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Renvoie un tableau d'éléments imbriqués du document spécifié pour les documents conteneurs tels que ZIP, OST, PST."
type: docs
weight: 160
url: /fr/net/groupdocs.search/index/getindexeddocumentitems/
---
## Index.GetIndexedDocumentItems method

Obtient un tableau d'éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST).

```csharp
public DocumentInfo[] GetIndexedDocumentItems(DocumentInfo documentInfo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| documentInfo | DocumentInfo | Les informations du document. |

### Valeur de retour

Un tableau d'éléments de document.

### Exemples

L'exemple montre comment obtenir une liste d'éléments d'un document indexé à partir d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
 
// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
 
// Obtention de la liste des documents indexés
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

### Voir aussi

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
