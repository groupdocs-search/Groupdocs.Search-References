---
title: "EventHub"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan peristiwa indeks untuk berlangganan."
type: docs
weight: 12
url: /id/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Menyediakan peristiwa indeks untuk berlangganan.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mencari di indeks
SearchResult result = index.search(query);
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | Deskripsi |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Terjadi ketika operasi indeks selesai. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Terjadi ketika terjadi kesalahan selama operasi indeks. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Terjadi ketika kemajuan proses pengindeksan atau pembaruan berubah. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Terjadi ketika kemajuan operasi optimasi berubah. |
|
|  | [PasswordRequired](#PasswordRequired) | Terjadi ketika sebuah dokumen memerlukan kata sandi untuk dibuka. |
|
|  | [FileIndexing](#FileIndexing) | Terjadi ketika sebuah dokumen akan diindeks. |
|
|  | [ImagePreparing](#ImagePreparing) | Terjadi ketika sebuah gambar akan dipersiapkan untuk pengindeksan. |
|
|  | [StatusChanged](#StatusChanged) | Terjadi ketika status indeks berubah. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Terjadi ketika fase pencarian selesai. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Terjadi ketika operasi indeks selesai.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Pesan: " + args.getMessage());
System.out.println("Folder indeks: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Waktu: " + df.format(args.getTime()));
}
});
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Terjadi ketika terjadi kesalahan selama operasi indeks.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mencari di indeks
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Terjadi ketika kemajuan proses pengindeksan atau pembaruan berubah.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Terakhir diproses: " + args.getLastDocumentPath());
System.out.println("Hasil: " + args.getLastDocumentStatus());
System.out.println("Dokumen yang diproses: " + args.getTotalDocuments());
System.out.println("Persentase kemajuan: " + args.getProgressPercentage());
}
});
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Terjadi ketika kemajuan operasi optimasi berubah.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Terjadi ketika sebuah dokumen memerlukan kata sandi untuk dibuka.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Terjadi ketika sebuah dokumen akan diindeks.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
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
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Terjadi ketika sebuah gambar akan dipersiapkan untuk pengindeksan.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Terjadi ketika status indeks berubah.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Berlangganan ke acara
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Sebuah notifikasi tentang penyelesaian operasi seharusnya ada di sini
}
}
});
// Mengatur flag untuk pengindeksan asinkron
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Mengindeks dokumen secara asinkron dari folder yang ditentukan
// Metode ini berakhir sebelum operasi selesai
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Terjadi ketika fase pencarian selesai.

Contoh ini menunjukkan cara menggunakan acara.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Berlangganan ke acara
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Tahap pencarian: " + args.getSearchPhase());
System.out.println("Kata: " + args.getWords().length);
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



