---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans le texte complet d'un document."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans le texte complet d'un document.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Rechercher la phase 'Theory of Relativity'
SearchResult result = index.search(\"\\\"Theory of Relativity\\\"\");
// Mettre en surbrillance les mots trouvés dans le texte d'un document
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, \"Highlighted.html\");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Initialise une nouvelle instance de la classe  DocumentHighlighter  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Obtient l'adaptateur de sortie passé au constructeur. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Initialise une nouvelle instance de la classe  DocumentHighlighter  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | L'adaptateur de sortie transférant un résultat de la mise en évidence. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Obtient l'adaptateur de sortie passé au constructeur.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

