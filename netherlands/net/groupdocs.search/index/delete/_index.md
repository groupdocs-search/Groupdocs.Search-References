---
title: Delete
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Verwijdert geïndexeerde bestanden of mappen uit de index. Werkt vervolgens de index bij zonder verwijderde paden. Houd er rekening mee dat een afzonderlijk document niet uit de index kan worden verwijderd als het aan de index is toegevoegd als onderdeel van een map.
type: docs
weight: 90
url: /nl/net/groupdocs.search/index/delete/
---
## Delete(string[], UpdateOptions) {#delete_1}

Verwijdert geïndexeerde bestanden of mappen uit de index. Werkt vervolgens de index bij zonder verwijderde paden. Houd er rekening mee dat een afzonderlijk document niet uit de index kan worden verwijderd als het aan de index is toegevoegd als onderdeel van een map.

```csharp
public DeleteResult Delete(string[] paths, UpdateOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| paths | String[] | De paden naar bestanden of mappen die moeten worden verwijderd. |
| options | UpdateOptions | De update-opties. |

### Winstwaarde

Een object dat het resultaat beschrijft van het verwijderen van bestanden of mappen uit de index.

### Voorbeelden

Het voorbeeld laat zien hoe geïndexeerde paden uit een index kunnen worden verwijderd.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Een index maken in de opgegeven map
Index index = new Index(indexFolder);

// Indexeren van documenten uit de opgegeven mappen
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Geïndexeerde paden ophalen uit de index
string[] indexedPaths1 = index.GetIndexedPaths();

// Schrijven van geïndexeerde paden naar de console
Console.WriteLine("Indexed paths:");
foreach (string path in indexedPaths1)
{
    Console.WriteLine("\t" + path);
}

// Indexpad verwijderen uit de index
DeleteResult deleteResult = index.Delete(new string[] { documentsFolder1 }, new UpdateOptions());

// Geïndexeerde paden ophalen na verwijdering
string[] indexedPaths2 = index.GetIndexedPaths();
Console.WriteLine("\nDeleted paths: " + deleteResult.SuccessCount);

Console.WriteLine("\nIndexed paths:");
foreach (string path in indexedPaths2)
{
    Console.WriteLine("\t" + path);
}
```

### Zie ook

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Delete(UpdateOptions, string[]) {#delete}

Verwijdert documenten die zijn geïndexeerd uit streams of structuren. Werkt vervolgens de index bij zonder verwijderde documenten.

```csharp
public DeleteResult Delete(UpdateOptions options, string[] documentKeys)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | UpdateOptions | De update-opties. |
| documentKeys | String[] | De sleutels van documenten die zijn toegevoegd vanuit streams of structuren. |

### Winstwaarde

Een object dat het resultaat beschrijft van het verwijderen van documenten uit de index.

### Zie ook

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
