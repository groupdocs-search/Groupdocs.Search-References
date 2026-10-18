---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta le informazioni di un elemento del contenitore."
type: docs
weight: 18
url: /it/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Rappresenta le informazioni di un elemento del contenitore.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Inizializza una nuova istanza della classe  ExtractedItemInfo  . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Restituisce un tipo di documento. |
|
|  | [getFields()](#getFields--) | Restituisce i campi estratti. |
|
|  | [getItemInfo()](#getItemInfo--) | Ottiene le informazioni dell'elemento. |
|
|  | [getInnerPath()](#getInnerPath--) | Ottiene un percorso interno. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Inizializza una nuova istanza della classe  ExtractedItemInfo  .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | La famiglia di formati del documento. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | I campi estratti. |
|
|  | itemInfo | java.lang.String | Le informazioni dell'elemento. |
|
|  | innerPath | java.lang.String | Il percorso all'elemento nel contenitore. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Restituisce un tipo di documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Restituisce i campi estratti.


**Returns:**
com.groupdocs.search.common.DocumentField[] - I campi estratti.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Ottiene le informazioni dell'elemento.


**Returns:**
java.lang.String - Le informazioni dell'elemento.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Ottiene un percorso interno.


**Returns:**
java.lang.String - Il percorso interno.

