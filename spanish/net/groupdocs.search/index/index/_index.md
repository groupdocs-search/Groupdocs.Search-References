---
title: "Index"
second_title: "Referencia de la API de GroupDocs.Search para .NET"
description: "Inicializa una nueva instancia de la clase Indexgroupdocs.search/index en memoria."
type: docs
weight: 10
url: /es/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Inicializa una nueva instancia de la clase [`Index`](../../index) en memoria.

```csharp
public Index()
```

### Ejemplos

El ejemplo muestra cómo crear un índice en memoria sin guardar archivos en disco.

```csharp
Index index = new Index(); 
```

### Ver también

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Inicializa una nueva instancia de la clase [`Index`](../../index) en memoria con configuraciones de índice particulares.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| settings | IndexSettings | El objeto de configuración del índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en memoria sin guardar archivos en disco con configuraciones de índice particulares.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Inicializa una nueva instancia de la clase [`Index`](../../index). Crea un nuevo índice o abre uno existente en disco.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta del índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco o abrir un índice existente.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Ver también

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Inicializa una nueva instancia de la clase [`Index`](../../index). Crea un nuevo índice con configuraciones particulares o abre un índice existente en el disco.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta del índice. |
| settings | IndexSettings | El objeto de configuración del índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco con configuraciones de índice particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Inicializa una nueva instancia de la clase [`Index`](../../index). Carga un índice existente del disco si *overwriteIfExists* es `false`; de lo contrario, crea un nuevo índice en el disco.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta del índice. |
| overwriteIfExists | Boolean | La bandera de sobrescribir la carpeta del índice. |

### Ejemplos

El ejemplo muestra cómo crear un nuevo índice en una carpeta que ya contiene otro índice.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Ver también

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Inicializa una nueva instancia de la clase [`Index`](../../index). Carga un índice existente del disco si *overwriteIfExists* es `false`; de lo contrario, crea un nuevo índice en el disco con configuraciones de índice particulares.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta del índice. |
| settings | IndexSettings | El objeto de configuración del índice. |
| overwriteIfExists | Boolean | La bandera de sobrescribir la carpeta del índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco con configuraciones de índice particulares.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
