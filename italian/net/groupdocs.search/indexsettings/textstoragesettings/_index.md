---
title: "TextStorageSettings"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene o imposta le impostazioni di archiviazione del testo. Il valore predefinito è null, il che significa che i testi dei documenti non vengono archiviati."
type: docs
weight: 100
url: /it/net/groupdocs.search/indexsettings/textstoragesettings/
---
## IndexSettings.TextStorageSettings property

Ottiene o imposta le impostazioni di archiviazione del testo. Il valore predefinito è `null`, il che significa che i testi dei documenti non vengono memorizzati.

```csharp
public TextStorageSettings TextStorageSettings { get; set; }
```

### Property Value

Le impostazioni di archiviazione del testo.

### Esempi

L'esempio dimostra come impostare le impostazioni di archiviazione del testo.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione dell'istanza delle impostazioni dell'indice
IndexSettings settings = new IndexSettings();
settings.TextStorageSettings = new TextStorageSettings(Compression.High); // Setting high compression level for the index text storage

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);

// Indicizzazione dei documenti
index.Add(documentsFolder);

// Ricerca
SearchResult result = index.Search("Einstein");
```

### Vedi anche

* class [TextStorageSettings](../../../groupdocs.search.options/textstoragesettings)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
