---
title: "CharacterReplacementDictionary"
second_title: "Referensi API GroupDocs.Search untuk .NET"
description: "Mewakili kamus penggantian karakter yang digunakan selama proses pengindeksan. Penggantian karakter dapat digunakan, misalnya, untuk menghapus aksen dari karakter beraksen atau untuk membuat indeks tidak sensitif huruf besar/kecil."
type: docs
weight: 390
url: /id/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Mewakili kamus penggantian karakter yang digunakan selama proses pengindeksan. Penggantian karakter dapat digunakan, misalnya, untuk menghapus aksen dari karakter beraksen atau untuk membuat indeks tidak sensitif huruf besar/kecil.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Mendapatkan jumlah titik kode Unicode yang terdapat dalam [`CharacterReplacementDictionary`](../characterreplacementdictionary) ini. |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Mendapatkan tipe kamus. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Menambahkan koleksi penggantian karakter yang ditentukan ke instance [`CharacterReplacementDictionary`](../characterreplacementdictionary) ini. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Menambahkan koleksi penggantian karakter yang ditentukan ke instance [`CharacterReplacementDictionary`](../characterreplacementdictionary) ini. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Menambahkan koleksi penggantian karakter yang ditentukan ke instance [`CharacterReplacementDictionary`](../characterreplacementdictionary) ini. |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Menambahkan koleksi penggantian titik kode Unicode yang ditentukan ke instance [`CharacterReplacementDictionary`](../characterreplacementdictionary) ini. |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Menghapus semua penggantian karakter dari objek [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Menentukan apakah objek [`CharacterReplacementDictionary`](../characterreplacementdictionary) berisi penggantian untuk titik kode Unicode yang ditentukan. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Mengekspor kamus ke file dengan nama yang ditentukan. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Mengembalikan enumerator yang mengiterasi koleksi. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Mendapatkan pengganti untuk titik kode Unicode yang ditentukan. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Mengimpor kamus dari file yang ditentukan. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Menghapus koleksi penggantian karakter yang ditentukan dari instance ini dari [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Menghapus koleksi penggantian karakter yang ditentukan dari instance ini dari [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Menghapus koleksi penggantian titik kode Unicode yang ditentukan dari instance ini dari [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Menghapus koleksi penggantian titik kode Unicode yang ditentukan dari instance ini dari [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Catatan

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Lihat Juga

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
