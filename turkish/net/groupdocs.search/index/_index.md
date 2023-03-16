---
title: Index
second_title: .NET API Başvurusu için GroupDocs.Search
description: Belgeleri indekslemek ve bunlar arasında arama yapmak için ana sınıfı temsil eder.
type: docs
weight: 680
url: /tr/net/groupdocs.search/index/
---
## Index class

Belgeleri indekslemek ve bunlar arasında arama yapmak için ana sınıfı temsil eder.

```csharp
public class Index : IDisposable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Index](index#constructor)() | Yeni bir örneğini başlatır.[`Index`](../index) bellekteki sınıf. |
| [Index](index#constructor_1)(IndexSettings) | Yeni bir örneğini başlatır.[`Index`](../index) belirli dizin ayarlarıyla bellekteki sınıf. |
| [Index](index#constructor_2)(string) | Yeni bir örneğini başlatır.[`Index`](../index) class. Diskte yeni bir dizin oluşturur veya mevcut bir dizini açar. |
| [Index](index#constructor_3)(string, bool) | Yeni bir örneğini başlatır.[`Index`](../index) class. Aşağıdaki durumlarda diskten mevcut bir dizini yükler*overwriteIfExists* dır-dir`YANLIŞ`; aksi takdirde diskte yeni bir dizin oluşturur. |
| [Index](index#constructor_4)(string, IndexSettings) | Yeni bir örneğini başlatır.[`Index`](../index) class. Belirli ayarlarla yeni bir dizin oluşturur veya diskte mevcut bir dizini açar. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Yeni bir örneğini başlatır.[`Index`](../index) class. Aşağıdaki durumlarda diskten mevcut bir dizini yükler*overwriteIfExists* dır-dir`YANLIŞ` ; , aksi takdirde belirli dizin ayarlarıyla diskte yeni bir dizin oluşturur. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Sözlük deposunu alır. |
| [Events](../../groupdocs.search/index/events) { get; } | Olaylara abone olmak için olay merkezini alır. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Dizin hakkında temel bilgileri alır. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Dizin ayarlarını alır. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Dizin içinde yer alıyorsa, dizin deposu nesnesini alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli yolla bir dosya veya klasör ekler. Tüm alt klasörlerdeki belgeler indekslenir. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | İndeksleme işlemini gerçekleştirir. Dosyaları veya klasörleri mutlak veya göreli bir yolla ekler. Tüm alt klasörlerdeki belgeler indekslenir. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Dosya sisteminden, akıştan veya yapıdan belgeler ekler. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Ayıklanan verileri indekse ekler. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | İndeksleme işlemini gerçekleştirir. Mutlak veya göreli yolla bir dosya veya klasör ekler. Tüm alt klasörlerdeki belgeler indekslenir. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | İndeksleme işlemini gerçekleştirir. Dosyaları veya klasörleri mutlak veya göreli bir yolla ekler. Tüm alt klasörlerdeki belgeler indekslenir. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Güncelleme işlemi sırasında yeniden dizin oluşturmadan, belirtilen öznitelik değişikliklerini dizinlenmiş belgelere uygular. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Dizinlenmiş dosyaları veya klasörleri dizinden siler. Ardından, silinmiş yollar olmadan dizini günceller. Bir klasörün parçası olarak dizine eklenmişse tek bir belgenin dizinden silinemeyeceğini unutmayın. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Dizinlenen belgeleri akışlardan veya yapılardan siler. Ardından, silinmiş belgeler olmadan dizini günceller. |
| [Dispose](../../groupdocs.search/index/dispose)() | tarafından kullanılan tüm kaynakları serbest bırakır.[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Belirtilen dizinlenmiş belgeyle ilişkili tüm öznitelikleri alır. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Dizinlenmiş belge için HTML biçimli metin oluşturur ve bunu çıkış adaptörü aracılığıyla aktarır. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Dizinlenmiş belge için HTML biçimli metin oluşturur ve bunu çıkış adaptörü aracılığıyla aktarır. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Belirtilen belgenin iç içe geçmiş öğelerinin bir dizisini alır (ZIP, OST, PST gibi kapsayıcı belgeler için). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Dizine alınan tüm belgelerin bir dizisini alır. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Belgeler veya klasörler gibi dizinlenmiş yollardan oluşan bir dizi alır. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | İndeksleme işlemleri ile ilgili raporları alır. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Arama işlemleriyle ilgili raporları alır. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Vurgulanan bulunan terimlerle HTML biçimli metin oluşturur. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Vurgulanan bulunan terimlerle HTML biçimli metin oluşturur. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Belirtilen dizini geçerli dizinde birleştirir. Diğer dizinin değişmeyeceğini unutmayın. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Belirtilen dizin deposundaki dizinleri geçerli dizine birleştirir. Depodaki dizinlerin değişmeyeceğini unutmayın. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Bildirimi gerçekleştirmek için belirtilen bildirim nesnesini dizine iletir. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Dizin segmentlerini birbiriyle birleştirerek sayısını en aza indirir. Bu işlem, arama performansını artırır. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Dizin segmentlerini birbiriyle birleştirerek sayısını en aza indirir. Bu işlem, arama performansını artırır. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | index. içinde arama yapar |
| [Search](../../groupdocs.search/index/search#search_3)(string) | index. içinde arama yapar |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Dizinde ters görüntü araması gerçekleştirir. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | index. içinde arama yapar |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | index. içinde arama yapar |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Search. yöntemiyle başlatılan yığın aramasına devam eder |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Search. yöntemiyle başlatılan yığın aramasına devam eder |
| [Update](../../groupdocs.search/index/update#update)() | Son güncellemeden sonra değiştirilen veya silinen belgeleri yeniden indeksler. İndekslenen klasörlere eklenen yeni dosyaları ekler. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Son güncellemeden sonra değiştirilen veya silinen belgeleri yeniden indeksler. İndekslenen klasörlere eklenen yeni dosyaları ekler. |

### Notlar

**Daha fazla bilgi edin**

* [indeks oluşturma](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [indeksleme](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Aranıyor](https://docs.groupdocs.com/display/searchnet/Searching)

### Örnekler

Örnek, sınıfın tipik bir kullanımını göstermektedir.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); //Belirtilen klasörde indeks oluşturma
index.Add(documentsFolder); // Belgeleri belirtilen klasörden indeksleme

SearchResult result = index.Search(query); // Dizinde arama
```

### Ayrıca bakınız

* ad alanı [GroupDocs.Search](../../groupdocs.search)
* toplantı [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
