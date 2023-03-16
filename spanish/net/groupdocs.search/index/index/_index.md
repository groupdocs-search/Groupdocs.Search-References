---
title: Index
second_title: GroupDocs.Buscar referencia de API de .NET
description: Inicializa una nueva instancia delIndexgroupdocs.search/index clase en memoria.
type: docs
weight: 10
url: /es/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Inicializa una nueva instancia del[`Index`](../../index) clase en memoria.

```csharp
public Index()
```

### Ejemplos

El ejemplo demuestra cómo crear un índice en la memoria sin guardar archivos en el disco.

```csharp
Index index = new Index(); 
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Inicializa una nueva instancia del[`Index`](../../index) clase en memoria con configuración de índice particular.

```csharp
public Index(IndexSettings settings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| settings | IndexSettings | El objeto de configuración de índice. |

### Ejemplos

El ejemplo demuestra cómo crear un índice en la memoria sin guardar archivos en el disco con una configuración de índice particular.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Inicializa una nueva instancia del[`Index`](../../index) class. Crea un índice nuevo o abre uno existente en el disco.

```csharp
public Index(string indexFolder)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta de índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco o abrir un índice existente.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Inicializa una nueva instancia del[`Index`](../../index) class. Crea un nuevo índice con una configuración particular o abre un índice existente en el disco.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta de índice. |
| settings | IndexSettings | El objeto de configuración de índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco con una configuración de índice particular.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Inicializa una nueva instancia del[`Index`](../../index) class. Carga un índice existente desde el disco si*overwriteIfExists* es`FALSO`; crea un nuevo índice en el disco de lo contrario.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta de índice. |
| overwriteIfExists | Boolean | El indicador de sobrescribir la carpeta de índice. |

### Ejemplos

El ejemplo muestra cómo crear un nuevo índice en una carpeta que ya contiene otro índice.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Ver también

* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Inicializa una nueva instancia del[`Index`](../../index) class. Carga un índice existente desde el disco si*overwriteIfExists* es`FALSO` ; crea un nuevo índice en el disco con una configuración de índice particular de lo contrario.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| indexFolder | String | La ruta de la carpeta de índice. |
| settings | IndexSettings | El objeto de configuración de índice. |
| overwriteIfExists | Boolean | El indicador de sobrescribir la carpeta de índice. |

### Ejemplos

El ejemplo muestra cómo crear un índice en un disco con una configuración de índice particular.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Ver también

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* espacio de nombres [GroupDocs.Search](../../index)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
