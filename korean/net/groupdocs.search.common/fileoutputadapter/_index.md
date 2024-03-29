---
title: FileOutputAdapter
second_title: GroupDocs..NET API 참조 검색
description: 출력을 파일로 수집하는 출력 어댑터를 나타냅니다.
type: docs
weight: 150
url: /ko/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

출력을 파일로 수집하는 출력 어댑터를 나타냅니다.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter#constructor)(OutputFormat, string) | 의 새 인스턴스를 초기화합니다.[`FileOutputAdapter`](../fileoutputadapter) 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | 출력 파일 경로를 가져옵니다. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | 출력 형식을 가져옵니다. |

### 비고

**더 알아보기**

* [출력 어댑터](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### 예

이 예제는 클래스의 일반적인 사용법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성

index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

DocumentInfo[] documents = index.GetIndexedDocuments(); // 색인된 문서에 대한 정보 가져오기

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // 파일 출력 어댑터 생성
index.GetDocumentText(documents[0], adapter); // 출력 파일에 문서 텍스트 생성
```

### 또한보십시오

* class [OutputAdapter](../outputadapter)
* 네임스페이스 [GroupDocs.Search.Common](../../groupdocs.search.common)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
