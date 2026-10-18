---
title: "Index"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse Indexgroupdocs.search/index im Speicher."
type: docs
weight: 10
url: /de/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse im Speicher.

```csharp
public Index()
```

### Beispiele

Das Beispiel zeigt, wie man einen Index im Speicher erstellt, ohne Dateien auf die Festplatte zu speichern.

```csharp
Index index = new Index(); 
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse im Speicher mit bestimmten Indexeinstellungen.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Einstellungen | IndexSettings | Das Indexeinstellungsobjekt. |

### Beispiele

Das Beispiel zeigt, wie man einen Index im Speicher erstellt, ohne Dateien auf die Festplatte zu speichern, und dabei bestimmte Indexeinstellungen verwendet.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse. Erstellt einen neuen Index oder öffnet einen bestehenden Index auf der Festplatte.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie man einen Index auf einer Festplatte erstellt oder einen bestehenden Index öffnet.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse. Erstellt einen neuen Index mit bestimmten Einstellungen oder öffnet einen bestehenden Index auf der Festplatte.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| Einstellungen | IndexSettings | Das Indexeinstellungsobjekt. |

### Beispiele

Das Beispiel zeigt, wie man einen Index auf einer Festplatte mit bestimmten Indexeinstellungen erstellt.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse. Lädt einen bestehenden Index von der Festplatte, wenn *overwriteIfExists* `false` ist; andernfalls wird ein neuer Index auf der Festplatte erstellt.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| overwriteIfExists | Boolean | Das Flag zum Überschreiben des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie man einen neuen Index in einem Ordner erstellt, der bereits einen anderen Index enthält.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialisiert eine neue Instanz der [`Index`](../../index)-Klasse. Lädt einen bestehenden Index von der Festplatte, wenn *overwriteIfExists* `false` ist; andernfalls wird ein neuer Index auf der Festplatte mit bestimmten Indexeinstellungen erstellt.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Pfad des Indexordners. |
| Einstellungen | IndexSettings | Das Indexeinstellungsobjekt. |
| overwriteIfExists | Boolean | Das Flag zum Überschreiben des Indexordners. |

### Beispiele

Das Beispiel zeigt, wie man einen Index auf einer Festplatte mit bestimmten Indexeinstellungen erstellt.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Siehe auch

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
