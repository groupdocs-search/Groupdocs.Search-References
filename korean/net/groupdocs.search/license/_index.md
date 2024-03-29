---
title: License
second_title: GroupDocs..NET API 참조 검색
description: 라이선스 적용 방법을 제공합니다.
type: docs
weight: 720
url: /ko/net/groupdocs.search/license/
---
## License class

라이선스 적용 방법을 제공합니다.

```csharp
public sealed class License
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [License](license)() | 의 새 인스턴스를 초기화합니다.[`License`](../license) 클래스. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense)(Stream) | 구성 요소에 라이선스를 부여합니다. |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense_1)(string) | 구성 요소에 라이선스를 부여합니다. |

### 비고

**더 알아보기**

* [평가 제한 및 라이선스](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### 예

예제는 라이센스를 설정하는 방법을 보여줍니다.

```csharp
License license = new License();
license.SetLicense("C:\\GroupDocs.Search.lic");
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Search](../../groupdocs.search)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
