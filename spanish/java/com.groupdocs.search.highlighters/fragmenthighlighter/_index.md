---
title: "FragmentHighlighter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un resaltador de resultados de búsqueda que resalta los resultados de búsqueda en fragmentos de texto."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Representa un resaltador de resultados de búsqueda que resalta los resultados de búsqueda en fragmentos de texto.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Buscar la palabra 'Einstein'
SearchResult result = index.search("Einstein");
// Asignando opciones de resaltado
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Resaltando palabras encontradas en el texto de un documento
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Obteniendo el resultado
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Imprimiendo marcado HTML en la consola
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Inicializa una nueva instancia de la  FragmentHighlighter  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getResult()](#getResult--) | Obtiene una matriz de contenedores de fragmentos resultantes. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Inicializa una nueva instancia de la  FragmentHighlighter  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | El formato de salida. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Obtiene una matriz de contenedores de fragmentos resultantes.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Una matriz de contenedores de fragmentos resultantes.

