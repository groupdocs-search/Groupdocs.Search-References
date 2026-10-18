---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज परिणाम हाईलाइटर का प्रतिनिधित्व करता है जो पूरे दस्तावेज़ के पाठ में खोज परिणामों को उजागर करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

एक खोज परिणाम हाईलाइटर का प्रतिनिधित्व करता है जो पूरे दस्तावेज़ के पाठ में खोज परिणामों को उजागर करता है।


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// 'Theory of Relativity' के लिए वाक्यांश खोजें
SearchResult result = index.search("\"Theory of Relativity\"");
// दस्तावेज़ के पाठ में पाए गए शब्दों को हाइलाइट करना
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | DocumentHighlighter वर्ग की नई इंस्टेंस को इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | कंस्ट्रक्टर में पास किए गए आउटपुट एडाप्टर को प्राप्त करता है। |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


DocumentHighlighter वर्ग की नई इंस्टेंस को इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | हाइलाइटिंग के परिणाम को स्थानांतरित करने वाला आउटपुट एडाप्टर। |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


कंस्ट्रक्टर में पास किए गए आउटपुट एडाप्टर को प्राप्त करता है।


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

