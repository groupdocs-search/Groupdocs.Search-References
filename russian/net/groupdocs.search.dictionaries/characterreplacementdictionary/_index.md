---
title: "CharacterReplacementDictionary"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Представляет словарь замены символов, используемый в процессе индексирования. Замена символов может использоваться, например, для удаления диакритических знаков с символов с акцентами или для создания регистронезависимого индекса."
type: docs
weight: 390
url: /ru/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Представляет словарь замены символов, используемый в процессе индексации. Замена символов может использоваться, например, для удаления диакритических знаков с символов с акцентами или для создания нечувствительного к регистру индекса.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Properties

| Name | Описание |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Получает количество кодовых точек Unicode, содержащихся в этом [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Получает тип словаря. |

## Methods

| Name | Описание |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Добавляет указанную коллекцию замен символов в этот экземпляр [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Добавляет указанную коллекцию замен символов в этот экземпляр [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Добавляет указанную коллекцию замен символов в этот экземпляр [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Добавляет указанную коллекцию замен кодовых точек Unicode в этот экземпляр [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Удаляет все замены символов из объекта [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Определяет, содержит ли объект [`CharacterReplacementDictionary`](../characterreplacementdictionary) замену для указанной кодовой точки Unicode. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Экспортирует словарь в файл с указанным именем. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Возвращает перечислитель, который проходит по коллекции. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Получает замену для указанной точки кода Unicode. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Импортирует словарь из указанного файла. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Удаляет указанную коллекцию замен символов из этого экземпляра [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Удаляет указанную коллекцию замен символов из этого экземпляра [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Удаляет указанную коллекцию замен точек кода Unicode из этого экземпляра [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Удаляет указанную коллекцию замен точек кода Unicode из этого экземпляра [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Примечания

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### См. также

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
