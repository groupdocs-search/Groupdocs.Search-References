---
title: TableDiscreteFunction
second_title: .NET API Başvurusu için GroupDocs.Search
description: Yeni bir örneğini başlatır.TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction sınıf.
type: docs
weight: 10
url: /tr/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Yeni bir örneğini başlatır.[`TableDiscreteFunction`](../../tablediscretefunction) sınıf.

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| offsetOfInputs | Int32 | Tablonun ofseti, giriş değerlerine göre endekslenir. |
| tableOfOutputs | Int32[] | Çıkış değerleri tablosu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Ne zaman atıldı*tableOfOutputs* dır-dir`hükümsüz`. |
| ArgumentException | Tablo öğelerinin sayısı 0 olduğunda fırlatılır. |

### Ayrıca bakınız

* class [TableDiscreteFunction](../../tablediscretefunction)
* ad alanı [GroupDocs.Search.Options](../../tablediscretefunction)
* toplantı [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Yeni bir örneğini başlatır.[`TableDiscreteFunction`](../../tablediscretefunction) sınıf.

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| firstStepLevel | Int32 | Adım fonksiyonunun ilk adımının seviyesi. |
| steps | Step[] | Adım fonksiyonunun sonraki adımları. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | Ne zaman atıldı*steps* dır-dir`hükümsüz`. |
| ArgumentException | Adımların sınırları kesinlikle artmadığında atılır. |

### Ayrıca bakınız

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* ad alanı [GroupDocs.Search.Options](../../tablediscretefunction)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->