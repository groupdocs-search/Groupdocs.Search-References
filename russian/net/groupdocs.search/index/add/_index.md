---
title: Add
second_title: GroupDocs.Search для справочника API .NET
description: Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.
type: docs
weight: 70
url: /ru/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу или папке для индексации. |

### Примеры

Пример демонстрирует, как добавлять документы в индекс.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(folderPath); // Индексация документов в указанной папке
index.Add(filePath); // Индексация указанного документа
```

### Смотрите также

* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string path, IndexingOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| path | String | Путь к файлу или папке для индексации. |
| options | IndexingOptions | Параметры индексации. |

### Примеры

Пример демонстрирует, как добавлять документы в индекс с определенными параметрами индексации.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Создание индекса в указанной папке

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Установка количества потоков индексации
index.Add(folderPath, options); // Индексация документов в указанной папке
index.Add(filePath, options); // Индексация указанного документа
```

### Смотрите также

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Выполняет операцию индексирования. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string[] paths)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| paths | String[] | Пути к файлам или папкам для индексации. |

### Примеры

Пример демонстрирует, как добавлять документы в индекс.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Создание индекса в указанной папке

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Индексация документов по указанным путям
```

### Смотрите также

* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Выполняет операцию индексирования. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| paths | String[] | Пути к файлам или папкам для индексации. |
| options | IndexingOptions | Параметры индексации. |

### Примеры

Пример демонстрирует, как добавлять документы в индекс с определенными параметрами индексации.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Создание индекса в указанной папке

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Установка количества потоков индексации
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Индексация документов по указанным путям
```

### Смотрите также

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Выполняет операцию индексирования. Добавляет документы из файловой системы, потока или структуры.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| documents | Document[] | Документы из файловой системы, потока или структуры. |
| options | IndexingOptions | Параметры индексации. |

### Смотрите также

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Выполняет операцию индексирования. Добавляет извлеченные данные в индекс.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| data | ExtractedData[] | Извлеченные данные. |
| options | IndexingOptions | Параметры индексации. |

### Смотрите также

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
