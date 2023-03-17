---
title: Index
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Initialiseert een nieuw exemplaar van hetIndexgroupdocs.search/index klasse in het geheugen.
type: docs
weight: 10
url: /nl/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) klasse in het geheugen.

```csharp
public Index()
```

### Voorbeelden

Het voorbeeld laat zien hoe u een index in het geheugen maakt zonder bestanden op schijf op te slaan.

```csharp
Index index = new Index(); 
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) klasse in het geheugen met bepaalde indexinstellingen.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | IndexSettings | Het object met indexinstellingen. |

### Voorbeelden

Het voorbeeld laat zien hoe u een index in het geheugen maakt zonder bestanden op schijf op te slaan met bepaalde indexinstellingen.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) class. Maakt een nieuwe of opent een bestaande index op schijf.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad naar de indexmap. |

### Voorbeelden

Het voorbeeld laat zien hoe u een index op een schijf maakt of een bestaande index opent.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) class. Maakt een nieuwe index aan met specifieke instellingen of opent een bestaande index op schijf.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad naar de indexmap. |
| settings | IndexSettings | Het object met indexinstellingen. |

### Voorbeelden

Het voorbeeld laat zien hoe u een index maakt op een schijf met bepaalde indexinstellingen.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) class. Laadt een bestaande index van schijf als*overwriteIfExists* is`vals`; maakt anders een nieuwe index op schijf.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad naar de indexmap. |
| overwriteIfExists | Boolean | De vlag van het overschrijven van de indexmap. |

### Voorbeelden

Het voorbeeld laat zien hoe u een nieuwe index maakt in een map die al een andere index bevat.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Initialiseert een nieuw exemplaar van het[`Index`](../../index) class. Laadt een bestaande index van schijf als*overwriteIfExists* is`vals` ; maakt een nieuwe index op schijf met anders bepaalde indexinstellingen.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| indexFolder | String | Het pad naar de indexmap. |
| settings | IndexSettings | Het object met indexinstellingen. |
| overwriteIfExists | Boolean | De vlag van het overschrijven van de indexmap. |

### Voorbeelden

Het voorbeeld laat zien hoe u een index maakt op een schijf met bepaalde indexinstellingen.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Zie ook

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
