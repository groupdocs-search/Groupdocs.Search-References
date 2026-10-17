---
title: "NodeEventHub"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر أحداث العقد للاشتراك."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

يوفر أحداث العقد للاشتراك.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | يحدث عندما تنتهي عملية تكوين شبكة البحث. |
|
|  | [IndexingCompleted](#IndexingCompleted) | يحدث عندما ينتهي فهرسة جميع المستندات المعلقة. |
|
|  | [DeletionCompleted](#DeletionCompleted) | يحدث عندما يتم الانتهاء من جميع عمليات حذف المستندات المعلقة في الطابور. |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | يحدث عندما يتم الانتهاء من تحسين جميع العقد. |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | يحدث عندما يتم الانتهاء من المزامنة مع جميع العقد. |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | يحدث عندما يتم الانتهاء من جميع تغييرات السمات المعلقة في الطابور. |
|
|  | [StatusChanged](#StatusChanged) | يحدث عندما تتغير حالة شبكة البحث. |
|
|  | [DataExtracted](#DataExtracted) | يحدث عندما يتم استخراج البيانات من مستند. |
|
|  | [DocumentIndexed](#DocumentIndexed) | يحدث عندما يتم فهرسة مستند. |
|
|  | [DocumentDeleted](#DocumentDeleted) | يحدث عندما يتم حذف مستند. |
|
|  | [ErrorOccurred](#ErrorOccurred) | يحدث عندما يحدث خطأ في أحد عقد شبكة البحث. |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | يحدث عندما يتغير تقدم عملية الفهرسة. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | يحدث عندما يتغير تقدم عملية التحسين. |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


يحدث عندما تنتهي عملية تكوين شبكة البحث.


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


يحدث عندما ينتهي فهرسة جميع المستندات المعلقة.


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


يحدث عندما يتم الانتهاء من جميع عمليات حذف المستندات المعلقة في الطابور.


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


يحدث عندما يتم الانتهاء من تحسين جميع العقد.


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


يحدث عندما يتم الانتهاء من المزامنة مع جميع العقد.


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


يحدث عندما يتم الانتهاء من جميع تغييرات السمات المعلقة في الطابور.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


يحدث عندما تتغير حالة شبكة البحث.


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


يحدث عندما يتم استخراج البيانات من مستند.


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


يحدث عندما يتم فهرسة مستند.


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


يحدث عندما يتم حذف مستند.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


يحدث عندما يحدث خطأ في أحد عقد شبكة البحث.


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


يحدث عندما يتغير تقدم عملية الفهرسة.


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


يحدث عندما يتغير تقدم عملية التحسين.


