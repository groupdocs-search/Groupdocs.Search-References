---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nei frammenti di testo."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Rappresenta un evidenziatore di risultati di ricerca che evidenzia i risultati di ricerca nei frammenti di testo.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Cerca la parola 'Einstein'
SearchResult result = index.search("Einstein");
// Assegna le opzioni di evidenziazione
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Evidenzia le parole trovate nel testo di un documento
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Ottieni il risultato
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Stampa del markup HTML sulla console
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Inizializza una nuova istanza della classe  FragmentHighlighter . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getResult()](#getResult--) | Ottiene un array di contenitori di frammenti risultanti. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Inizializza una nuova istanza della classe  FragmentHighlighter .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Il formato di output. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Ottiene un array di contenitori di frammenti risultanti.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Un array di contenitori di frammenti risultanti.

