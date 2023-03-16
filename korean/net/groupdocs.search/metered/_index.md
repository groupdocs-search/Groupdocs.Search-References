---
title: Metered
second_title: GroupDocs..NET API 참조 검색
description: 측정된 라이선스로 제품을 활성화하고 처리된 MB 양을 검색할 수 있는 방법을 제공합니다. 측정된 라이선스에 대해 자세히 알아보기여기https//purchase.groupdocs.com/faqs/licensing/metered .
type: docs
weight: 730
url: /ko/net/groupdocs.search/metered/
---
## Metered class

측정된 라이선스로 제품을 활성화하고 처리된 MB 양을 검색할 수 있는 방법을 제공합니다. 측정된 라이선스에 대해 자세히 알아보기[여기](https://purchase.groupdocs.com/faqs/licensing/metered) .

```csharp
public class Metered
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Metered](metered)() | 의 새 인스턴스를 초기화합니다.[`Metered`](../metered) 클래스. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [SetMeteredKey](../../groupdocs.search/metered/setmeteredkey)(string, string) | 측정된 공개 및 개인 키를 설정합니다. |
| static [GetConsumptionCredit](../../groupdocs.search/metered/getconsumptioncredit)() | 소비 크레딧을 가져옵니다. |
| static [GetConsumptionQuantity](../../groupdocs.search/metered/getconsumptionquantity)() | 소비 수량을 가져옵니다. |

### 비고

**더 알아보기**

* [평가 제한 및 라이선스](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### 예

이 예는 측정된 공개 및 개인 키를 설정하는 방법을 보여줍니다.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Search](../../groupdocs.search)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->