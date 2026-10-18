---
title: "EventHub"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Abonelik için indeks olayları sağlar."
type: docs
weight: 12
url: /tr/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Abonelik için indeks olayları sağlar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// Dizinde arama
SearchResult result = index.search(query);
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Bir indeks işlemi tamamlandığında oluşur. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Bir indeks işlemi sırasında bir hata oluştuğunda oluşur. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Dizinleme veya güncelleme işleminin ilerlemesi değiştiğinde oluşur. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Optimizasyon işleminin ilerlemesi değiştiğinde oluşur. |
|
|  | [PasswordRequired](#PasswordRequired) | Bir belge açmak için şifre gerektirdiğinde meydana gelir. |
|
|  | [FileIndexing](#FileIndexing) | Bir belge indekslenecek olduğunda oluşur. |
|
|  | [ImagePreparing](#ImagePreparing) | Bir görüntü indeksleme için hazırlanırken meydana gelir. |
|
|  | [StatusChanged](#StatusChanged) | İndeks durumu değiştiğinde oluşur. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Arama aşaması tamamlandığında oluşur. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Bir indeks işlemi tamamlandığında oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Message: " + args.getMessage());
System.out.println("Index folder: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(args.getTime()));
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Bir indeks işlemi sırasında bir hata oluştuğunda oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// Dizinde arama
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Dizinleme veya güncelleme işleminin ilerlemesi değiştiğinde oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Last processed: " + args.getLastDocumentPath());
System.out.println("Sonuç: " + args.getLastDocumentStatus());
System.out.println("İşlenen belgeler: " + args.getTotalDocuments());
System.out.println("İlerleme yüzdesi: " + args.getProgressPercentage());
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Optimizasyon işleminin ilerlemesi değiştiğinde oluşur.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Bir belge açmak için şifre gerektirdiğinde meydana gelir.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Bir belge indekslenecek olduğunda oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Tags", "Protected")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("important")) {
args.setSkipIndexing(true);
}
}
});
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Bir görüntü indeksleme için hazırlanırken meydana gelir.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


İndeks durumu değiştiğinde oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Olayı abone olma
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// İşlemin tamamlanmasıyla ilgili bir bildirim burada olmalı
}
}
});
// Asenkron indeksleme için bayrağı ayarlama
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Belirtilen klasörden asenkron belge indeksleme
// Yöntem, işlem tamamlanmadan önce sonlandırılır
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Arama aşaması tamamlandığında oluşur.

Bu örnek, olayın nasıl kullanılacağını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// Olayı abone olma
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Arama aşaması: " + args.getSearchPhase());
System.out.println("Kelimeler: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



