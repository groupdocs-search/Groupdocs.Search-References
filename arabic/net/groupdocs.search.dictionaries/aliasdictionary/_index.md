---
title: AliasDictionary
second_title: GroupDocs. ابحث عن مرجع .NET API
description: يمثل قاموسًا للأسماء المستعارة .
type: docs
weight: 340
url: /ar/net/groupdocs.search.dictionaries/aliasdictionary/
---
## AliasDictionary class

يمثل قاموسًا للأسماء المستعارة .

```csharp
public class AliasDictionary : DictionaryBase, IEnumerable<string>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/aliasdictionary/count) { get; } | الحصول على عدد الأسماء المستعارة الموجودة في ملف[`AliasDictionary`](../aliasdictionary) . |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/aliasdictionary/add)(string, string) | يضيف زوجًا محددًا من الاسم المستعار والنص المرتبط به إلى مثيل ملف[`AliasDictionary`](../aliasdictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange)(AliasReplacementPair[]) | يضيف المجموعة المحددة من أزواج الاسم المستعار / الاستبدال إلى مثيل[`AliasDictionary`](../aliasdictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_1)(IEnumerable&lt;AliasReplacementPair&gt;) | يضيف المجموعة المحددة من أزواج الاسم المستعار / الاستبدال إلى مثيل[`AliasDictionary`](../aliasdictionary) . |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;string, string&gt;&gt;) | يضيف المجموعة المحددة من أزواج الاسم المستعار / الاستبدال إلى مثيل[`AliasDictionary`](../aliasdictionary) . |
| [Clear](../../groupdocs.search.dictionaries/aliasdictionary/clear)() | يزيل كافة الأسماء المستعارة من ملف[`AliasDictionary`](../aliasdictionary) الكائن . |
| [Contains](../../groupdocs.search.dictionaries/aliasdictionary/contains)(string) | يحدد ما إذا كان ملف[`AliasDictionary`](../aliasdictionary)يحتوي الكائن على الاسم المستعار المحدد. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | يصدر القاموس إلى ملف بالاسم المحدد. |
| [GetEnumerator](../../groupdocs.search.dictionaries/aliasdictionary/getenumerator)() | إرجاع عداد يتكرر خلال المجموعة. |
| [GetText](../../groupdocs.search.dictionaries/aliasdictionary/gettext)(string) | يحصل على نص مرتبط بالاسم المستعار المحدد. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | لاستيراد قاموس من الملف المحدد. |
| [Remove](../../groupdocs.search.dictionaries/aliasdictionary/remove)(string) | يزيل الاسم المستعار المحدد من ملف[`AliasDictionary`](../aliasdictionary) الكائن . |

### ملاحظات

**يتعلم أكثر**

* [استخدام الأسماء المستعارة](https://docs.groupdocs.com/display/searchnet/Using+aliases)
* [إدارة قاموس الاسم المستعار](https://docs.groupdocs.com/display/searchnet/Alias+dictionary)

### أنظر أيضا

* class [DictionaryBase](../dictionarybase)
* مساحة الاسم [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* المجسم [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->