---
title: "Create"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt einen neuen Index im Speicher."
type: docs
weight: 50
url: /de/net/groupdocs.search/indexrepository/create/
---
## Create() {#create}

Erstellt einen neuen Index im Speicher.

```csharp
public Index Create()
```

### Rückgabewert

Der erstellte Index.

### Beispiele

Das Beispiel demonstriert, wie man einen Index im Speicher über das Index-Repository erstellt.

```csharp
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create();
```

### Siehe auch

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(IndexSettings) {#create_1}

Erstellt einen neuen Index im Speicher.

```csharp
public Index Create(IndexSettings settings)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Einstellungen | IndexSettings | Die Indexeinstellungen. |

### Rückgabewert

Der erstellte Index.

### Beispiele

Das Beispiel demonstriert, wie man einen Index im Speicher über das Index-Repository erstellt.

```csharp
IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(settings);
```

### Siehe auch

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string) {#create_2}

Erstellt einen neuen Index auf der Festplatte. Der Indexordner wird vor der Erstellung des Index bereinigt.

```csharp
public Index Create(string indexFolder)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Indexordner. |

### Rückgabewert

Der erstellte Index.

### Beispiele

Das Beispiel demonstriert, wie man einen Index auf der Festplatte über das Index-Repository erstellt.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.Create(indexFolder);
```

### Siehe auch

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Create(string, IndexSettings) {#create_3}

Erstellt einen neuen Index auf der Festplatte. Der Indexordner wird vor der Erstellung des Index bereinigt.

```csharp
public Index Create(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Indexordner. |
| Einstellungen | IndexSettings | Die Indexeinstellungen. |

### Rückgabewert

Der erstellte Index.

### Beispiele

Das Beispiel demonstriert, wie man einen Index auf der Festplatte über das Index-Repository erstellt.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

IndexSettings settings = new IndexSettings();
settings.UseStopWords = false; // Disabling use of stop words during indexing

Index index = indexRepository.Create(indexFolder, settings);
```

### Siehe auch

* class [Index](../../index)
* class [IndexSettings](../../indexsettings)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
