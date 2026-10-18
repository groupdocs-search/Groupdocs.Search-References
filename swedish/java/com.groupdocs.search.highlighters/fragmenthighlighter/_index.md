---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en sökresultatmarkerare som markerar sökresultat i textfragment."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Representerar en sökresultatmarkerare som markerar sökresultat i textfragment.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Sök efter ordet 'Einstein'
SearchResult result = index.search("Einstein");
// Tilldelar markeringsalternativ
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Markering av hittade ord i texten i ett dokument
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Hämtar resultatet
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Skriver ut HTML-markup till konsolen
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Initierar en ny instans av  FragmentHighlighter  klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getResult()](#getResult--) | Hämtar en array av resulterande fragmentbehållare. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Initierar en ny instans av  FragmentHighlighter  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Utdataformatet. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Hämtar en array av resulterande fragmentbehållare.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - En array av resulterande fragmentbehållare.

