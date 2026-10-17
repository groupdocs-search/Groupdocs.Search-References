---
title: "EventHub"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر أحداث الفهرس للاشتراك."
type: docs
weight: 12
url: /ar/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

يوفر أحداث الفهرس للاشتراك.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// البحث في الفهرس
SearchResult result = index.search(query);
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | يحدث عندما تنتهي عملية الفهرسة. |
|
|  | [ErrorOccurred](#ErrorOccurred) | يحدث عندما يحدث خطأ أثناء عملية الفهرسة. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | يحدث عندما يتغير تقدم عملية الفهرسة أو التحديث. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | يحدث عندما يتغير تقدم عملية التحسين. |
|
|  | [PasswordRequired](#PasswordRequired) | يحدث عندما يتطلب المستند كلمة مرور للفتح. |
|
|  | [FileIndexing](#FileIndexing) | يحدث عندما يتم فهرسة مستند. |
|
|  | [ImagePreparing](#ImagePreparing) | يحدث عندما يتم إعداد صورة للفهرسة. |
|
|  | [StatusChanged](#StatusChanged) | يحدث عندما تتغير حالة الفهرس. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | يحدث عندما تكتمل مرحلة البحث. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


يحدث عندما تنتهي عملية الفهرسة.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Message: " + args.getMessage());
System.out.println("Index folder: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(args.getTime()));
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


يحدث عندما يحدث خطأ أثناء عملية الفهرسة.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// البحث في الفهرس
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


يحدث عندما يتغير تقدم عملية الفهرسة أو التحديث.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Last processed: " + args.getLastDocumentPath());
System.out.println("النتيجة: " + args.getLastDocumentStatus());
System.out.println("المستندات المعالجة: " + args.getTotalDocuments());
System.out.println("نسبة التقدم: " + args.getProgressPercentage());
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


يحدث عندما يتغير تقدم عملية التحسين.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


يحدث عندما يتطلب المستند كلمة مرور للفتح.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


يحدث عندما يتم فهرسة مستند.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("الوسوم", "محمي")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("important")) {
args.setSkipIndexing(true);
}
}
});
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


يحدث عندما يتم إعداد صورة للفهرسة.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


يحدث عندما تتغير حالة الفهرس.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// الاشتراك في الحدث
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// إشعار بإكمال العملية يجب أن يكون هنا
}
}
});
// تعيين العلامة للفهرسة غير المتزامنة
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// فهرسة المستندات بشكل غير متزامن من المجلد المحدد
// تنتهي الطريقة قبل إكمال العملية
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


يحدث عندما تكتمل مرحلة البحث.

يوضح المثال كيفية استخدام الحدث.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// الاشتراك في الحدث
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("مرحلة البحث: " + args.getSearchPhase());
System.out.println("الكلمات: " + args.getWords().length);
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



