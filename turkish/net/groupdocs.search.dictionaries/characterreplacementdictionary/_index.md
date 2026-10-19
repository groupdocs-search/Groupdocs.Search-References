---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search için .NET API Referansı"
description: "Dizinleme sürecinde kullanılan bir karakter değiştirme sözlüğünü temsil eder. Karakter değiştirme, örneğin aksanlı karakterlerden aksanları kaldırmak veya büyük/küçük harfe duyarsız bir indeks oluşturmak için kullanılabilir."
type: docs
weight: 390
url: /tr/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Dizinleme sürecinde kullanılan bir karakter değiştirme sözlüğünü temsil eder. Karakter değiştirme, örneğin aksanlı karakterlerden aksanları kaldırmak veya büyük/küçük harfe duyarsız bir indeks oluşturmak için kullanılabilir.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Bu [`CharacterReplacementDictionary`](../characterreplacementdictionary) içinde bulunan Unicode kod noktası sayısını alır. |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Sözlüğün türünü alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Belirtilen karakter değiştirme koleksiyonunu bu [`CharacterReplacementDictionary`](../characterreplacementdictionary) örneğine ekler. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Belirtilen karakter değiştirme koleksiyonunu bu [`CharacterReplacementDictionary`](../characterreplacementdictionary) örneğine ekler. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Belirtilen karakter değiştirme koleksiyonunu bu [`CharacterReplacementDictionary`](../characterreplacementdictionary) örneğine ekler. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Belirtilen Unicode kod noktası değiştirme koleksiyonunu bu [`CharacterReplacementDictionary`](../characterreplacementdictionary) örneğine ekler. |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Bir [`CharacterReplacementDictionary`](../characterreplacementdictionary) nesnesinden tüm karakter değişikliklerini kaldırır. |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Bir [`CharacterReplacementDictionary`](../characterreplacementdictionary) nesnesinin belirtilen Unicode kod noktası için bir değiştirme içerip içermediğini belirler. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Sözlüğü belirtilen adla bir dosyaya dışa aktarır. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Koleksiyon içinde yineleme yapan bir enumerator döndürür. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Belirtilen Unicode kod noktasına ait bir değiştirme alır. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Belirtilen dosyadan bir sözlük içe aktarır. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Bu örnekten, belirtilen karakter değiştirmeleri koleksiyonunu [`CharacterReplacementDictionary`](../characterreplacementdictionary) içinden kaldırır. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Bu örnekten, belirtilen karakter değiştirmeleri koleksiyonunu [`CharacterReplacementDictionary`](../characterreplacementdictionary) içinden kaldırır. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Bu örnekten, belirtilen Unicode kod noktası değiştirmeleri koleksiyonunu [`CharacterReplacementDictionary`](../characterreplacementdictionary) içinden kaldırır. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Bu örnekten, belirtilen Unicode kod noktası değiştirmeleri koleksiyonunu [`CharacterReplacementDictionary`](../characterreplacementdictionary) içinden kaldırır. |

### Açıklamalar

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Ayrıca Bakınız

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
