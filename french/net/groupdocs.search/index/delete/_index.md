---
title: "Delete"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Supprime les fichiers ou dossiers indexés de l'index. Met ensuite à jour l'index sans les chemins supprimés. Notez qu'un document individuel ne peut pas être supprimé de l'index s'il a été ajouté à l'index en tant que partie d'un dossier."
type: docs
weight: 110
url: /fr/net/groupdocs.search/index/delete/
---
## Delete(string[], UpdateOptions) {#delete_1}

Supprime les fichiers ou dossiers indexés de l'index. Met ensuite à jour l'index sans les chemins supprimés. Notez qu'un document individuel ne peut pas être supprimé de l'index s'il a été ajouté à l'index en tant que partie d'un dossier.

```csharp
public DeleteResult Delete(string[] paths, UpdateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paths | String[] | Les chemins des fichiers ou dossiers à supprimer. |
| options | UpdateOptions | Les options de mise à jour. |

### Valeur de retour

Un objet décrivant le résultat de la suppression de fichiers ou dossiers de l'index.

### Exemples

L'exemple montre comment supprimer des chemins indexés d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);

// Indexation des documents à partir des dossiers spécifiés
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Obtention des chemins indexés à partir de l'index
string[] indexedPaths1 = index.GetIndexedPaths();

// Écriture des chemins indexés dans la console
Console.WriteLine("Indexed paths:");
foreach (string path in indexedPaths1)
{
    Console.WriteLine("\t" + path);
}

// Suppression du chemin d'index de l'index
DeleteResult deleteResult = index.Delete(new string[] { documentsFolder1 }, new UpdateOptions());

// Obtention des chemins indexés après suppression
string[] indexedPaths2 = index.GetIndexedPaths();
Console.WriteLine("\nDeleted paths: " + deleteResult.SuccessCount);

Console.WriteLine("\nIndexed paths:");
foreach (string path in indexedPaths2)
{
    Console.WriteLine("\t" + path);
}
```

### Voir aussi

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Delete(UpdateOptions, string[]) {#delete}

Supprime les documents indexés provenant de flux ou de structures. Met ensuite à jour l'index sans les documents supprimés.

```csharp
public DeleteResult Delete(UpdateOptions options, string[] documentKeys)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | UpdateOptions | Les options de mise à jour. |
| documentKeys | String[] | Les clés des documents ajoutés à partir de flux ou de structures. |

### Valeur de retour

Un objet décrivant le résultat de la suppression de documents de l'index.

### Voir aussi

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
