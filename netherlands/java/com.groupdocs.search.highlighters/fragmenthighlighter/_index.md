---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoekresultaatmarkeerder voor die zoekresultaten markeert in tekstfragmenten."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Stelt een zoekresultaatmarkeerder voor die zoekresultaten markeert in tekstfragmenten.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Zoek naar het woord 'Einstein'
SearchResult result = index.search("Einstein");
// Toewijzen van markeeropties
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Markeren van gevonden woorden in de tekst van een document
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Resultaat ophalen
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Afdrukken van HTML-markup naar console
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Initialiseert een nieuw exemplaar van de  FragmentHighlighter  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getResult()](#getResult--) | Haalt een array op van resulterende fragmentcontainers. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Initialiseert een nieuw exemplaar van de  FragmentHighlighter  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Het uitvoerformaat. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Haalt een array op van resulterende fragmentcontainers.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Een array van resulterende fragmentcontainers.

