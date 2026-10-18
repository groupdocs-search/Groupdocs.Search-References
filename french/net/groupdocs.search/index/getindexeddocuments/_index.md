---
title: "GetIndexedDocuments"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient un tableau de tous les documents indexés."
type: docs
weight: 170
url: /fr/net/groupdocs.search/index/getindexeddocuments/
---
## Index.GetIndexedDocuments method

Obtient un tableau de tous les documents indexés.

```csharp
public DocumentInfo[] GetIndexedDocuments()
```

### Valeur de retour

Un tableau de tous les documents indexés.

### Exemples

L'exemple montre comment obtenir une liste de documents indexés à partir d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
 
// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
 
// Obtention de la liste des documents indexés
DocumentInfo[] documents = index.GetIndexedDocuments();
```

### Voir aussi

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
