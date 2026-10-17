---
title: "DocumentHighlighter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مبرز نتائج البحث الذي يسلط الضوء على نتائج البحث في نص المستند بالكامل."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

يمثل مبرز نتائج البحث الذي يسلط الضوء على نتائج البحث في نص المستند بالكامل.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// ابحث عن العبارة 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// تمييز الكلمات الموجودة في نص المستند
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | يقوم بتهيئة نسخة جديدة من الفئة DocumentHighlighter. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | يحصل على محول الإخراج الممرّر في المُنشئ. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


يقوم بتهيئة نسخة جديدة من الفئة DocumentHighlighter.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | محول الإخراج ينقل نتيجة التمييز. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


يحصل على محول الإخراج الممرّر في المُنشئ.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

