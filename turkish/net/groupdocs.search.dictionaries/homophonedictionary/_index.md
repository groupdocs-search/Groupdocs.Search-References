---
title: HomophoneDictionary
second_title: .NET API Başvurusu için GroupDocs.Search
description: Heterografik sesteş sözcüklerin bir sözlüğünü temsil eder.
type: docs
weight: 440
url: /tr/net/groupdocs.search.dictionaries/homophonedictionary/
---
## HomophoneDictionary class

Heterografik sesteş sözcüklerin bir sözlüğünü temsil eder.

```csharp
public class HomophoneDictionary : DictionaryBase, IEnumerable<string>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/homophonedictionary/count) { get; } | Bu dosyada bulunan kelime sayısını alır.[`HomophoneDictionary`](../homophonedictionary) . |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Belirtilen eş sesli grup koleksiyonunu bu örneğine ekler.[`HomophoneDictionary`](../homophonedictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange_1)(string[][]) | Belirtilen eş sesli grup koleksiyonunu bu örneğine ekler.[`HomophoneDictionary`](../homophonedictionary) . |
| [Clear](../../groupdocs.search.dictionaries/homophonedictionary/clear)() | Bir dosyadan tüm sözcükleri kaldırır.[`HomophoneDictionary`](../homophonedictionary) nesne. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Sözlüğü belirtilen ada sahip bir dosyaya aktarır. |
| [GetAllHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/getallhomophonegroups)() | Bu sözlükte bulunan tüm homofon gruplarını alır. |
| [GetEnumerator](../../groupdocs.search.dictionaries/homophonedictionary/getenumerator)() | Koleksiyon boyunca yinelenen bir numaralandırıcı döndürür. |
| [GetHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/gethomophonegroups)(string) | Belirtilen kelimenin ait olduğu tüm homofon gruplarını alır. |
| [GetHomophones](../../groupdocs.search.dictionaries/homophonedictionary/gethomophones)(string) | Belirtilen kelime için sesteş sözcükleri alır. Ortaya çıkan dizi, orijinal kelimeyi içermez. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Belirtilen dosyadan bir sözlük alır. |

### Notlar

**Daha fazla bilgi edin**

* [homofon arama](https://docs.groupdocs.com/display/searchnet/Homophone+search)
* [Homofon sözlüğünü yönetme](https://docs.groupdocs.com/display/searchnet/Homophone+dictionary)

### Ayrıca bakınız

* class [DictionaryBase](../dictionarybase)
* ad alanı [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
