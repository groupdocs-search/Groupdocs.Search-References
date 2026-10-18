---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Suchergebnis-Hervorheber dar, der Suchergebnisse in Textfragmenten hervorhebt."
type: docs
weight: 11
url: /de/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Stellt einen Suchergebnis-Hervorheber dar, der Suchergebnisse in Textfragmenten hervorhebt.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Suche nach dem Wort 'Einstein'
SearchResult result = index.search("Einstein");
// Zuweisen von Hervorhebungsoptionen
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Hervorheben gefundener Wörter im Text eines Dokuments
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Abrufen des Ergebnisses
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// HTML-Markup in die Konsole ausgeben
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Initialisiert eine neue Instanz der  FragmentHighlighter  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getResult()](#getResult--) | Gibt ein Array der resultierenden Fragmentcontainer zurück. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Initialisiert eine neue Instanz der  FragmentHighlighter  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Das Ausgabeformat. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Gibt ein Array der resultierenden Fragmentcontainer zurück.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Ein Array der resultierenden Fragmentcontainer.

