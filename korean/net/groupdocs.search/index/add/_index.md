---
title: Add
second_title: GroupDocs..NET API 참조 검색
description: 인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.
type: docs
weight: 70
url: /ko/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 인덱싱할 파일 또는 폴더의 경로입니다. |

### 예

이 예제는 인덱스에 문서를 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(folderPath); // 지정된 폴더의 문서 인덱싱
index.Add(filePath); // 지정된 문서를 인덱싱
```

### 또한보십시오

* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string path, IndexingOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 인덱싱할 파일 또는 폴더의 경로입니다. |
| options | IndexingOptions | 인덱싱 옵션. |

### 예

이 예는 특정 인덱싱 옵션을 사용하여 인덱스에 문서를 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // 인덱싱 스레드 수 설정
index.Add(folderPath, options); // 지정된 폴더의 문서 인덱싱
index.Add(filePath, options); // 지정된 문서를 인덱싱
```

### 또한보십시오

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string[] paths)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| paths | String[] | 인덱싱할 파일 또는 폴더의 경로입니다. |

### 예

이 예제는 인덱스에 문서를 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // 지정된 경로에서 문서 인덱싱
```

### 또한보십시오

* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| paths | String[] | 인덱싱할 파일 또는 폴더의 경로입니다. |
| options | IndexingOptions | 인덱싱 옵션. |

### 예

이 예는 특정 인덱싱 옵션을 사용하여 인덱스에 문서를 추가하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // 인덱싱 스레드 수 설정
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // 지정된 경로에서 문서 인덱싱
```

### 또한보십시오

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

인덱싱 작업을 수행합니다. 파일 시스템, 스트림 또는 구조에서 문서를 추가합니다.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| documents | Document[] | 파일 시스템, 스트림 또는 구조의 문서. |
| options | IndexingOptions | 인덱싱 옵션. |

### 또한보십시오

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

인덱싱 작업을 수행합니다. 추출된 데이터를 인덱스에 추가합니다.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| data | ExtractedData[] | 추출된 데이터입니다. |
| options | IndexingOptions | 인덱싱 옵션. |

### 또한보십시오

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->