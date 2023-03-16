---
title: Alphabet
second_title: GroupDocs..NET API 참조 검색
description: 문자 유형을 감지하기 위해 인덱싱하는 동안 사용되는 문자 사전을 나타냅니다. 각 문자는 구분 기호 문자 또는 둘 다로 처리할 수 있습니다.
type: docs
weight: 370
url: /ko/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

문자 유형을 감지하기 위해 인덱싱하는 동안 사용되는 문자 사전을 나타냅니다. 각 문자는 구분 기호, 문자 또는 둘 다로 처리할 수 있습니다.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<char>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | 에 포함된 문자 수를 가져옵니다.[`Alphabet`](../alphabet) . |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | 설정Separator 이 모든 문자에 대해 입력하십시오.[`Alphabet`](../alphabet) . |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | 지정된 이름의 파일로 사전을 내보냅니다. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype)(char) | 문자 유형을 가져옵니다. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | 컬렉션을 반복하는 열거자를 반환합니다. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | 지정된 파일에서 사전을 가져옵니다. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange)(char[], CharacterType) | 이 인스턴스에서 지정된 컬렉션의 각 문자에 대한 유형을 설정합니다.[`Alphabet`](../alphabet) . |

### 비고

**더 알아보기**

* [문자 유형](https://docs.groupdocs.com/display/searchnet/Character+types)
* [알파벳 관리](https://docs.groupdocs.com/display/searchnet/Alphabet)

### 또한보십시오

* class [DictionaryBase](../dictionarybase)
* 네임스페이스 [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->