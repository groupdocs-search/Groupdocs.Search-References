---
title: "NodeEventHub"
second_title: "GroupDocs.Search for Java API Reference"
description: "सदस्यता के लिए नोड घटनाएँ प्रदान करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search.scaling.events/nodeeventhub/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeEventHub
```

सदस्यता के लिए नोड घटनाएँ प्रदान करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NodeEventHub()](#NodeEventHub--) |  |
## Fields

| Field | विवरण |
| --- | --- |
|  | [ConfigurationCompleted](#ConfigurationCompleted) | जब खोज नेटवर्क कॉन्फ़िगरेशन प्रक्रिया समाप्त हो जाती है, तब होता है। |
|
|  | [IndexingCompleted](#IndexingCompleted) | जब सभी कतारबद्ध दस्तावेज़ों का अनुक्रमण समाप्त हो जाता है, तब होता है। |
|
|  | [DeletionCompleted](#DeletionCompleted) | जब सभी कतारबद्ध दस्तावेज़ों की हटाने की प्रक्रिया समाप्त हो जाती है, तब होता है। |
|
|  | [OptimizationCompleted](#OptimizationCompleted) | जब सभी नोड्स का अनुकूलन समाप्त हो जाता है, तब होता है। |
|
|  | [SynchronizationCompleted](#SynchronizationCompleted) | जब सभी नोड्स के साथ समन्वय समाप्त हो जाता है, तब होता है। |
|
|  | [AttributeChangesCompleted](#AttributeChangesCompleted) | जब सभी कतारबद्ध गुण परिवर्तन समाप्त हो जाते हैं, तब होता है। |
|
|  | [StatusChanged](#StatusChanged) | जब खोज नेटवर्क की स्थिति बदलती है, तब होता है। |
|
|  | [DataExtracted](#DataExtracted) | जब दस्तावेज़ से डेटा निकाला गया है, तब होता है। |
|
|  | [DocumentIndexed](#DocumentIndexed) | जब एक दस्तावेज़ का अनुक्रमण किया गया है, तब होता है। |
|
|  | [DocumentDeleted](#DocumentDeleted) | जब एक दस्तावेज़ को हटाया गया है, तब होता है। |
|
|  | [ErrorOccurred](#ErrorOccurred) | जब खोज नेटवर्क के किसी नोड में त्रुटि होती है, तब होता है। |
|
|  | [IndexingProgressChanged](#IndexingProgressChanged) | जब अनुक्रमण ऑपरेशन की प्रगति बदलती है, तब होता है। |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | जब अनुकूलन ऑपरेशन की प्रगति बदलती है, तब होता है। |
|
### NodeEventHub() {#NodeEventHub--}
```
public NodeEventHub()
```


### ConfigurationCompleted {#ConfigurationCompleted}
```
public final Event<EventHandler> ConfigurationCompleted
```


जब खोज नेटवर्क कॉन्फ़िगरेशन प्रक्रिया समाप्त हो जाती है, तब होता है।


### IndexingCompleted {#IndexingCompleted}
```
public final Event<EventHandler> IndexingCompleted
```


जब सभी कतारबद्ध दस्तावेज़ों का अनुक्रमण समाप्त हो जाता है, तब होता है।


### DeletionCompleted {#DeletionCompleted}
```
public final Event<EventHandler> DeletionCompleted
```


जब सभी कतारबद्ध दस्तावेज़ों की हटाने की प्रक्रिया समाप्त हो जाती है, तब होता है।


### OptimizationCompleted {#OptimizationCompleted}
```
public final Event<EventHandler> OptimizationCompleted
```


जब सभी नोड्स का अनुकूलन समाप्त हो जाता है, तब होता है।


### SynchronizationCompleted {#SynchronizationCompleted}
```
public final Event<EventHandler> SynchronizationCompleted
```


जब सभी नोड्स के साथ समन्वय समाप्त हो जाता है, तब होता है।


### AttributeChangesCompleted {#AttributeChangesCompleted}
```
public final Event<EventHandler> AttributeChangesCompleted
```


जब सभी कतारबद्ध गुण परिवर्तन समाप्त हो जाते हैं, तब होता है।


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<StatusChangedEventArgs>> StatusChanged
```


जब खोज नेटवर्क की स्थिति बदलती है, तब होता है।


### DataExtracted {#DataExtracted}
```
public final Event<EventHandler<DataExtractedEventArgs>> DataExtracted
```


जब दस्तावेज़ से डेटा निकाला गया है, तब होता है।


### DocumentIndexed {#DocumentIndexed}
```
public final Event<EventHandler<DocumentIndexedEventArgs>> DocumentIndexed
```


जब एक दस्तावेज़ का अनुक्रमण किया गया है, तब होता है।


### DocumentDeleted {#DocumentDeleted}
```
public final Event<EventHandler<DocumentDeletedEventArgs>> DocumentDeleted
```


जब एक दस्तावेज़ को हटाया गया है, तब होता है।


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<ErrorOccurredEventArgs>> ErrorOccurred
```


जब खोज नेटवर्क के किसी नोड में त्रुटि होती है, तब होता है।


### IndexingProgressChanged {#IndexingProgressChanged}
```
public final Event<EventHandler<NetworkIndexingProgressEventArgs>> IndexingProgressChanged
```


जब अनुक्रमण ऑपरेशन की प्रगति बदलती है, तब होता है।


### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<NetworkOptimizationProgressEventArgs>> OptimizationProgressChanged
```


जब अनुकूलन ऑपरेशन की प्रगति बदलती है, तब होता है।


