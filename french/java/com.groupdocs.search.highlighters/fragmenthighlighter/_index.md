---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans des fragments de texte."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans des fragments de texte.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Rechercher le mot 'Einstein'
SearchResult result = index.search("Einstein");
// Assignation des options de mise en évidence
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Mettre en surbrillance les mots trouvés dans le texte d'un document
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Obtention du résultat
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Impression du balisage HTML dans la console
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Initialise une nouvelle instance de la classe  FragmentHighlighter . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getResult()](#getResult--) | Obtient un tableau de conteneurs de fragments résultants. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Initialise une nouvelle instance de la classe  FragmentHighlighter .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Le format de sortie. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Obtient un tableau de conteneurs de fragments résultants.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Un tableau de conteneurs de fragments résultants.

