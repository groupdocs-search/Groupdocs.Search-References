---
title: "Delete"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Löscht indexierte Dateien oder Ordner aus dem Index. Aktualisiert anschließend den Index ohne die gelöschten Pfade. Hinweis: Ein einzelnes Dokument kann nicht aus dem Index gelöscht werden, wenn es als Teil eines Ordners zum Index hinzugefügt wurde."
type: docs
weight: 110
url: /de/net/groupdocs.search/index/delete/
---
## Delete(string[], UpdateOptions) {#delete_1}

Löscht indexierte Dateien oder Ordner aus dem Index. Aktualisiert anschließend den Index ohne die gelöschten Pfade. Hinweis: Ein einzelnes Dokument kann nicht aus dem Index gelöscht werden, wenn es als Teil eines Ordners zum Index hinzugefügt wurde.

```csharp
public DeleteResult Delete(string[] paths, UpdateOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| paths | String[] | Die Pfade zu Dateien oder Ordnern, die gelöscht werden sollen. |
| Optionen | UpdateOptions | Die Aktualisierungsoptionen. |

### Rückgabewert

Ein Objekt, das das Ergebnis des Löschens von Dateien oder Ordnern aus dem Index beschreibt.

### Beispiele

Das Beispiel zeigt, wie indizierte Pfade aus einem Index gelöscht werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);

// Dokumente aus den angegebenen Ordnern indizieren
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Abrufen indizierter Pfade aus dem Index
string[] indexedPaths1 = index.GetIndexedPaths();

// Schreiben indizierter Pfade in die Konsole
Console.WriteLine("Indexed paths:");
foreach (string path in indexedPaths1)
{
    Console.WriteLine("\t" + path);
}

// Löschen des Indexpfads aus dem Index
DeleteResult deleteResult = index.Delete(new string[] { documentsFolder1 }, new UpdateOptions());

// Abrufen indizierter Pfade nach dem Löschen
string[] indexedPaths2 = index.GetIndexedPaths();
Console.WriteLine("\nDeleted paths: " + deleteResult.SuccessCount);

Console.WriteLine("\nIndexed paths:");
foreach (string path in indexedPaths2)
{
    Console.WriteLine("\t" + path);
}
```

### Siehe auch

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Delete(UpdateOptions, string[]) {#delete}

Löscht aus Streams oder Strukturen indexierte Dokumente. Aktualisiert anschließend den Index ohne die gelöschten Dokumente.

```csharp
public DeleteResult Delete(UpdateOptions options, string[] documentKeys)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Optionen | UpdateOptions | Die Aktualisierungsoptionen. |
| documentKeys | String[] | Die Schlüssel der aus Streams oder Strukturen hinzugefügten Dokumente. |

### Rückgabewert

Ein Objekt, das das Ergebnis des Löschens von Dokumenten aus dem Index beschreibt.

### Siehe auch

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
