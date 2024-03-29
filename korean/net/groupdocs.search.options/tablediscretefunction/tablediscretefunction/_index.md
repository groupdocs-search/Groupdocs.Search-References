---
title: TableDiscreteFunction
second_title: GroupDocs..NET API 참조 검색
description: 의 새 인스턴스를 초기화합니다.TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction 클래스.
type: docs
weight: 10
url: /ko/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`TableDiscreteFunction`](../../tablediscretefunction) 클래스.

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| offsetOfInputs | Int32 | 입력 값을 기준으로 테이블 인덱스의 오프셋입니다. |
| tableOfOutputs | Int32[] | 출력 값 테이블입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | 언제 던져*tableOfOutputs* ~이다`없는`. |
| ArgumentException | 테이블 요소의 수가 0일 때 발생합니다. |

### 또한보십시오

* class [TableDiscreteFunction](../../tablediscretefunction)
* 네임스페이스 [GroupDocs.Search.Options](../../tablediscretefunction)
* 집회 [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

의 새 인스턴스를 초기화합니다.[`TableDiscreteFunction`](../../tablediscretefunction) 클래스.

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| firstStepLevel | Int32 | 단계 함수의 첫 번째 단계 수준입니다. |
| steps | Step[] | 단계 기능의 다음 단계. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | 언제 던져*steps* ~이다`없는`. |
| ArgumentException | 단계 제한이 엄격하게 증가하지 않을 때 발생합니다. |

### 또한보십시오

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* 네임스페이스 [GroupDocs.Search.Options](../../tablediscretefunction)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
