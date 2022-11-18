---
title: Index
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Inizializza una nuova istanza diIndexgroupdocs.search/index classe in memoria.
type: docs
weight: 10
url: /it/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Inizializza una nuova istanza di[`Index`](../../index) classe in memoria.

```csharp
public Index()
```

### Esempi

L'esempio mostra come creare un indice in memoria senza salvare i file su disco.

```csharp
Index index = new Index(); 
```

### Guarda anche

* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Inizializza una nuova istanza di[`Index`](../../index) classe in memoria con particolari impostazioni di indice.

```csharp
public Index(IndexSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |

### Esempi

L'esempio mostra come creare un indice in memoria senza salvare i file su disco con particolari impostazioni di indice.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Guarda anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Inizializza una nuova istanza di[`Index`](../../index) class. Crea un nuovo o apre un indice esistente su disco.

```csharp
public Index(string indexFolder)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |

### Esempi

L'esempio mostra come creare un indice su un disco o aprire un indice esistente.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Guarda anche

* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Inizializza una nuova istanza di[`Index`](../../index) class. Crea un nuovo indice con impostazioni particolari o apre un indice esistente su disco.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |

### Esempi

L'esempio mostra come creare un indice su un disco con particolari impostazioni di indice.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Guarda anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Inizializza una nuova istanza di[`Index`](../../index) class. Carica un indice esistente dal disco se*overwriteIfExists* è`falso`; crea un nuovo indice su disco altrimenti.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| overwriteIfExists | Boolean | Il flag di sovrascrittura della cartella index. |

### Esempi

L'esempio mostra come creare un nuovo indice in una cartella che contiene già un altro indice.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Guarda anche

* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Inizializza una nuova istanza di[`Index`](../../index) class. Carica un indice esistente dal disco se*overwriteIfExists* è`falso` ; crea un nuovo indice su disco con particolari impostazioni di indice altrimenti.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indexFolder | String | Il percorso della cartella dell'indice. |
| settings | IndexSettings | L'oggetto delle impostazioni dell'indice. |
| overwriteIfExists | Boolean | Il flag di sovrascrittura della cartella index. |

### Esempi

L'esempio mostra come creare un indice su un disco con particolari impostazioni di indice.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Guarda anche

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
