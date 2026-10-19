---
title: "Index"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Inizializza una nuova istanza della classe Indexgroupdocs.search/index in memoria."
type: docs
weight: 10
url: /it/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Inizializza una nuova istanza della classe [`Index`](../../index) in memoria.

```csharp
public Index()
```

### Esempi

L'esempio dimostra come creare un indice in memoria senza salvare i file su disco.

```csharp
Index index = new Index(); 
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Inizializza una nuova istanza della classe [`Index`](../../index) in memoria con impostazioni di indice specifiche.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |

### Esempi

L'esempio dimostra come creare un indice in memoria senza salvare i file su disco con impostazioni di indice specifiche.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Vedi anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Inizializza una nuova istanza della classe [`Index`](../../index). Crea un nuovo indice o apre un indice esistente su disco.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |

### Esempi

L'esempio dimostra come creare un indice su disco o aprire un indice esistente.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Inizializza una nuova istanza della classe [`Index`](../../index). Crea un nuovo indice con impostazioni particolari o apre un indice esistente su disco.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |

### Esempi

L'esempio dimostra come creare un indice su disco con impostazioni di indice particolari.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Vedi anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Inizializza una nuova istanza della classe [`Index`](../../index). Carica un indice esistente da disco se *overwriteIfExists* è `false`; altrimenti crea un nuovo indice su disco.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| overwriteIfExists | Boolean | Il flag per sovrascrivere la cartella dell'indice. |

### Esempi

L'esempio dimostra come creare un nuovo indice in una cartella che contiene già un altro indice.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Inizializza una nuova istanza della classe [`Index`](../../index). Carica un indice esistente da disco se *overwriteIfExists* è `false`; altrimenti crea un nuovo indice su disco con impostazioni di indice particolari.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |
| overwriteIfExists | Boolean | Il flag per sovrascrivere la cartella dell'indice. |

### Esempi

L'esempio dimostra come creare un indice su disco con impostazioni di indice particolari.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Vedi anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
