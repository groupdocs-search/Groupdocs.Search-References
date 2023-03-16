---
title: AddRange
second_title: GroupDocs.Mencari Referensi .NET API
description: Menambahkan kumpulan grup sinonim yang ditentukan ke instance dariSynonymDictionarygroupdocs.search.dictionaries/synonymdictionary .
type: docs
weight: 20
url: /id/net/groupdocs.search.dictionaries/synonymdictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Menambahkan kumpulan grup sinonim yang ditentukan ke instance dari[`SynonymDictionary`](../../synonymdictionary) .

```csharp
public void AddRange(IEnumerable<string[]> synonyms)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| synonyms | IEnumerable`1 | Koleksi grup sinonim untuk ditambahkan ke kamus. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Dilempar kapan*synonyms* adalah`batal`. |
| ArgumentException | Dilempar ketika jumlah sinonim dalam grup kurang dari 2. |

### Lihat juga

* class [SynonymDictionary](../../synonymdictionary)
* ruang nama [GroupDocs.Search.Dictionaries](../../synonymdictionary)
* perakitan [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Menambahkan kumpulan grup sinonim yang ditentukan ke instance dari[`SynonymDictionary`](../../synonymdictionary) .

```csharp
public void AddRange(string[][] synonyms)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| synonyms | String[][] | Koleksi grup sinonim untuk ditambahkan ke kamus. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | Dilempar kapan*synonyms* adalah`batal`. |
| ArgumentException | Dilempar ketika jumlah sinonim dalam grup kurang dari 2. |

### Lihat juga

* class [SynonymDictionary](../../synonymdictionary)
* ruang nama [GroupDocs.Search.Dictionaries](../../synonymdictionary)
* perakitan [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->