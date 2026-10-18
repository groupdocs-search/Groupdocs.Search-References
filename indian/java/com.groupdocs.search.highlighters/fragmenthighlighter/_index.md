---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज परिणाम हाईलाइटर का प्रतिनिधित्व करता है जो पाठ अंशों में खोज परिणामों को उजागर करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

एक खोज परिणाम हाईलाइटर का प्रतिनिधित्व करता है जो पाठ अंशों में खोज परिणामों को उजागर करता है।


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// शब्द 'Einstein' के लिए खोजें
SearchResult result = index.search("Einstein");
// हाइलाइट विकल्प असाइन करना
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// दस्तावेज़ के पाठ में पाए गए शब्दों को हाइलाइट करना
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// परिणाम प्राप्त करना
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// कंसोल में HTML मार्कअप प्रिंट कर रहा है
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | FragmentHighlighter क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getResult()](#getResult--) | परिणामी फ्रैगमेंट कंटेनरों की एक एरे प्राप्त करता है। |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


FragmentHighlighter क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | आउटपुट फ़ॉर्मेट। |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


परिणामी फ्रैगमेंट कंटेनरों की एक एरे प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - परिणामी फ्रैगमेंट कंटेनरों की एक एरे।

