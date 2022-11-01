---
title: Index
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Initialisiert eine neue Instanz vonIndexgroupdocs.search/index Klasse im Gedächtnis.
type: docs
weight: 10
url: /de/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialisiert eine neue Instanz von[`Index`](../../index) Klasse im Gedächtnis.

```csharp
public Index()
```

### Beispiele

Das Beispiel zeigt, wie ein Index im Arbeitsspeicher erstellt wird, ohne Dateien auf der Festplatte zu speichern.

```csharp
Index index = new Index(); 
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialisiert eine neue Instanz von[`Index`](../../index) Klasse im Speicher mit bestimmten Indexeinstellungen.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | IndexSettings | Das Indexeinstellungsobjekt. |

### Beispiele

Das Beispiel zeigt, wie Sie einen Index im Arbeitsspeicher erstellen, ohne Dateien mit bestimmten Indexeinstellungen auf der Festplatte zu speichern.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialisiert eine neue Instanz von[`Index`](../../index) class. Erstellt einen neuen oder öffnet einen vorhandenen Index auf der Festplatte.

```csharp
public Index(string indexFolder)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie Sie einen Index auf einem Datenträger erstellen oder einen vorhandenen Index öffnen.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialisiert eine neue Instanz von[`Index`](../../index) class. Erstellt einen neuen Index mit bestimmten Einstellungen oder öffnet einen bestehenden Index auf der Festplatte.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| settings | IndexSettings | Das Indexeinstellungsobjekt. |

### Beispiele

Das Beispiel zeigt, wie ein Index auf einem Datenträger mit bestimmten Indexeinstellungen erstellt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialisiert eine neue Instanz von[`Index`](../../index) class. Lädt einen vorhandenen Index von der Festplatte, wenn*overwriteIfExists* ist`FALSCH`; erstellt andernfalls einen neuen Index auf der Festplatte.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| overwriteIfExists | Boolean | Das Flag zum Überschreiben des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie Sie einen neuen Index in einem Ordner erstellen, der bereits einen anderen Index enthält.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialisiert eine neue Instanz von[`Index`](../../index) class. Lädt einen vorhandenen Index von der Festplatte, wenn*overwriteIfExists* ist`FALSCH` ; erstellt andernfalls einen neuen Index auf der Festplatte mit bestimmten Indexeinstellungen.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| settings | IndexSettings | Das Indexeinstellungsobjekt. |
| overwriteIfExists | Boolean | Das Flag zum Überschreiben des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie ein Index auf einem Datenträger mit bestimmten Indexeinstellungen erstellt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
