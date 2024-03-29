---
title: IndexRepository
second_title: .NET API Başvurusu için GroupDocs.Search
description: Birden çok dizini birleştirmek ve bunlar üzerinde ortak işlemler gerçekleştirmek için bir kapsayıcıyı temsil eder.
type: docs
weight: 690
url: /tr/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Birden çok dizini birleştirmek ve bunlar üzerinde ortak işlemler gerçekleştirmek için bir kapsayıcıyı temsil eder.

```csharp
public class IndexRepository : IDisposable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [IndexRepository](indexrepository)() | Yeni bir örneğini başlatır.[`IndexRepository`](../indexrepository) sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Olaylara abone olmak için olay merkezini alır. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Bunun içerdiği dizinleri alır[`IndexRepository`](../indexrepository) . |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Dizin deposuna bir dizin ekler. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Açar ve dizin deposuna bir dizin ekler. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Bellekte yeni bir dizin oluşturur. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Bellekte yeni bir dizin oluşturur. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Diskte yeni bir dizin oluşturur. Dizin klasörü, dizin oluşturmadan önce temizlenecektir. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Diskte yeni bir dizin oluşturur. Dizin klasörü, dizin oluşturmadan önce temizlenecektir. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | tarafından kullanılan tüm kaynakları serbest bırakır.[`IndexRepository`](../indexrepository) . |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Deponun tüm dizinlerinde arama yapar. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Deponun tüm dizinlerinde arama yapar. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Deponun tüm dizinlerinde arama yapar. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Deponun tüm dizinlerinde arama yapar. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Depodaki tüm dizinleri günceller. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Depodaki tüm dizinleri günceller. |

### Notlar

**Daha fazla bilgi edin**

* [Arama dizin deposu](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Örnekler

Örnek, sınıfın tipik bir kullanımını göstermektedir.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Varolan bir dizini yüklemek
repository.AddToRepository(indexFolder2); // Başka bir mevcut indeks yükleniyor

SearchResult result = repository.Search(query); // Deponun dizinlerinde arama
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Search](../../groupdocs.search)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
