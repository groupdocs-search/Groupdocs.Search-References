---
title: "FragmentHighlighter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مبرز نتائج البحث الذي يسلط الضوء على نتائج البحث في مقاطع النص."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

يمثل مبرز نتائج البحث الذي يسلط الضوء على نتائج البحث في مقاطع النص.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// ابحث عن الكلمة 'Einstein'
SearchResult result = index.search("Einstein");
// تعيين خيارات التمييز
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// تمييز الكلمات الموجودة في نص المستند
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// الحصول على النتيجة
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// طباعة ترميز HTML إلى وحدة التحكم
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | تهيئة نسخة جديدة من الفئة  FragmentHighlighter  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getResult()](#getResult--) | يحصل على مصفوفة من حاويات القطع الناتجة. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


تهيئة نسخة جديدة من الفئة  FragmentHighlighter  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | تنسيق الإخراج. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


يحصل على مصفوفة من حاويات القطع الناتجة.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - مصفوفة من حاويات القطع الناتجة.

