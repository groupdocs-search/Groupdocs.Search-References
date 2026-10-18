---
title: "EventHub"
second_title: "GroupDocs.Search for Java API Reference"
description: "सदस्यता के लिए इंडेक्स घटनाएँ प्रदान करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

सदस्यता के लिए इंडेक्स घटनाएँ प्रदान करता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// इंडेक्स में खोज करना
SearchResult result = index.search(query);
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Fields

| Field | विवरण |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | जब एक इंडेक्स ऑपरेशन समाप्त हो जाता है, तब होता है। |
|
|  | [ErrorOccurred](#ErrorOccurred) | जब एक इंडेक्स ऑपरेशन के दौरान त्रुटि होती है, तब होता है। |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | जब अनुक्रमण या अद्यतन ऑपरेशन की प्रगति बदलती है, तब होता है। |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | जब अनुकूलन ऑपरेशन की प्रगति बदलती है, तब होता है। |
|
|  | [PasswordRequired](#PasswordRequired) | दस्तावेज़ को खोलने के लिए पासवर्ड चाहिए होने पर होता है। |
|
|  | [FileIndexing](#FileIndexing) | जब कोई दस्तावेज़ अनुक्रमित किया जाने वाला हो, तब होता है। |
|
|  | [ImagePreparing](#ImagePreparing) | इंडेक्सिंग के लिए छवि तैयार होने पर होता है। |
|
|  | [StatusChanged](#StatusChanged) | जब इंडेक्स की स्थिति बदलती है, तब होता है। |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | जब खोज चरण पूर्ण हो जाता है, तब होता है। |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


जब एक इंडेक्स ऑपरेशन समाप्त हो जाता है, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println(\"संदेश: \" + args.getMessage());
System.out.println(\"इंडेक्स फ़ोल्डर: \" + args.getIndexFolder());
DateFormat df = new SimpleDateFormat(\"MM/dd/yyyy HH:mm:ss\");
System.out.println(\"समय: \" + df.format(args.getTime()));
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


जब एक इंडेक्स ऑपरेशन के दौरान त्रुटि होती है, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// इंडेक्स में खोज करना
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


जब अनुक्रमण या अद्यतन ऑपरेशन की प्रगति बदलती है, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println(\"अंतिम प्रोसेस किया गया: \" + args.getLastDocumentPath());
System.out.println(\"परिणाम: \" + args.getLastDocumentStatus());
System.out.println(\"प्रोसेस किए गए दस्तावेज़: \" + args.getTotalDocuments());
System.out.println(\"प्रगति प्रतिशत: \" + args.getProgressPercentage());
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


जब अनुकूलन ऑपरेशन की प्रगति बदलती है, तब होता है।


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


दस्तावेज़ को खोलने के लिए पासवर्ड चाहिए होने पर होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith(\"ProtectedDocument.pdf\")) {
args.setPassword(\"123456\");
}
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


जब कोई दस्तावेज़ अनुक्रमित किया जाने वाला हो, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith(\"Protected.pdf\")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField(\"टैग्स\", \"सुरक्षित\")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains(\"महत्वपूर्ण\")) {
args.setSkipIndexing(true);
}
}
});
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


इंडेक्सिंग के लिए छवि तैयार होने पर होता है।


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


जब इंडेक्स की स्थिति बदलती है, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// ऑपरेशन पूर्ण होने की सूचना यहाँ होनी चाहिए
}
}
});
// असिंक्रोनस इंडेक्सिंग के लिए फ़्लैग सेट करना
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों की असिंक्रोनस इंडेक्सिंग
// ऑपरेशन पूर्ण होने से पहले मेथड समाप्त हो जाता है
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


जब खोज चरण पूर्ण हो जाता है, तब होता है।

यह उदाहरण दिखाता है कि इवेंट का उपयोग कैसे किया जाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// इवेंट को सब्सक्राइब करना
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Search phase: " + args.getSearchPhase());
System.out.println("Words: " + args.getWords().length);
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



