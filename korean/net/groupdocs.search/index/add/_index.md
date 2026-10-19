---
title: "Add"
second_title: "GroupDocs.Search 용 .NET API Reference"
description: "인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다."
type: docs
weight: 80
url: /ko/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string path)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| path | String | 인덱싱할 파일 또는 폴더의 경로입니다. |

### 예제

예제는 문서를 인덱스에 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### 또 보기

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| path | String | 인덱싱할 파일 또는 폴더의 경로입니다. |
| options | 인덱싱 옵션 | 인덱싱 옵션입니다. |

### 예제

예제는 특정 인덱싱 옵션을 사용하여 문서를 인덱스에 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더들을 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| paths | String[] | 인덱싱할 파일 또는 폴더들의 경로입니다. |

### 예제

예제는 문서를 인덱스에 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### 또 보기

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더들을 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| paths | String[] | 인덱싱할 파일 또는 폴더들의 경로입니다. |
| options | 인덱싱 옵션 | 인덱싱 옵션입니다. |

### 예제

예제는 특정 인덱싱 옵션을 사용하여 문서를 인덱스에 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

인덱싱 작업을 수행합니다. 파일 시스템, 스트림 또는 구조에서 문서를 추가합니다.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 문서 | Document[] | 파일 시스템, 스트림 또는 구조에서 가져온 문서입니다. |
| options | 인덱싱 옵션 | 인덱싱 옵션입니다. |

### 또 보기

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

인덱싱 작업을 수행합니다. 추출된 데이터를 인덱스에 추가합니다.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | 설명 |
| --- | --- | --- |
| 데이터 | ExtractedData[] | 추출된 데이터입니다. |
| options | 인덱싱 옵션 | 인덱싱 옵션입니다. |

### 또 보기

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
