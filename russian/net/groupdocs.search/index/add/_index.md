---
title: "Add"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы."
type: docs
weight: 80
url: /ru/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string path)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| path | String | Путь к файлу или папке, которые будут проиндексированы. |

### Примеры

В примере демонстрируется, как добавить документы в индекс.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### См. также

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| path | String | Путь к файлу или папке, которые будут проиндексированы. |
| опции | IndexingOptions | Параметры индексации. |

### Примеры

В примере демонстрируется, как добавить документы в индекс с определёнными параметрами индексации.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### См. также

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Выполняет операцию индексации. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| paths | String[] | Пути к файлам или папкам, которые будут проиндексированы. |

### Примеры

В примере демонстрируется, как добавить документы в индекс.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### См. также

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Выполняет операцию индексации. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| paths | String[] | Пути к файлам или папкам, которые будут проиндексированы. |
| опции | IndexingOptions | Параметры индексации. |

### Примеры

В примере демонстрируется, как добавить документы в индекс с определёнными параметрами индексации.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### См. также

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Выполняет операцию индексации. Добавляет документы из файловой системы, потока или структуры.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| документы | Document[] | Документы из файловой системы, потока или структуры. |
| опции | IndexingOptions | Параметры индексации. |

### См. также

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Выполняет операцию индексации. Добавляет извлечённые данные в индекс.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| данные | ExtractedData[] | Извлечённые данные. |
| опции | IndexingOptions | Параметры индексации. |

### См. также

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
