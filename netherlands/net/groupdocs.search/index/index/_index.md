---
title: "Index"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de Indexgroupdocs.search/index-klasse in het geheugen."
type: docs
weight: 10
url: /nl/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialiseert een nieuw exemplaar van de [`Index`](../../index)-klasse in het geheugen.

```csharp
public Index()
```

### Voorbeelden

Het voorbeeld laat zien hoe je een index in het geheugen kunt maken zonder bestanden naar schijf op te slaan.

```csharp
Index index = new Index(); 
```

### Zie ook

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`Index`](../../index)-klasse in het geheugen met specifieke indexinstellingen.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | IndexSettings | Het indexinstellingen-object. |

### Voorbeelden

Het voorbeeld laat zien hoe je een index in het geheugen kunt maken zonder bestanden naar schijf op te slaan, met specifieke indexinstellingen.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`Index`](../../index)-klasse. Maakt een nieuwe index aan of opent een bestaande index op schijf.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad van de indexmap. |

### Voorbeelden

Het voorbeeld laat zien hoe je een index op een schijf kunt maken of een bestaande index kunt openen.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Zie ook

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialiseert een nieuw exemplaar van de [`Index`](../../index) klasse. Maakt een nieuwe index met specifieke instellingen of opent een bestaande index op schijf.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad van de indexmap. |
| settings | IndexSettings | Het indexinstellingen-object. |

### Voorbeelden

Het voorbeeld toont hoe u een index op een schijf maakt met specifieke indexinstellingen.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`Index`](../../index) klasse. Laadt een bestaande index van schijf als *overwriteIfExists* `false` is; maakt anders een nieuwe index op schijf.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad van de indexmap. |
| overwriteIfExists | Boolean | De vlag voor het overschrijven van de indexmap. |

### Voorbeelden

Het voorbeeld toont hoe u een nieuwe index maakt in een map die al een andere index bevat.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Zie ook

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialiseert een nieuw exemplaar van de [`Index`](../../index) klasse. Laadt een bestaande index van schijf als *overwriteIfExists* `false` is; maakt anders een nieuwe index op schijf met specifieke indexinstellingen.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad van de indexmap. |
| settings | IndexSettings | Het indexinstellingen-object. |
| overwriteIfExists | Boolean | De vlag voor het overschrijven van de indexmap. |

### Voorbeelden

Het voorbeeld toont hoe u een index op een schijf maakt met specifieke indexinstellingen.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
