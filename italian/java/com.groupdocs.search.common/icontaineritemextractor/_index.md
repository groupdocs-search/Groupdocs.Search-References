---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce metodi per estrarre elementi da documenti contenitori."
type: docs
weight: 35
url: /it/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Fornisce metodi per estrarre elementi da documenti contenitori.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Restituisce la famiglia di formati del documento. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Estrae elementi dal documento contenitore. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Estrae elementi dal documento contenitore. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Restituisce la famiglia di formati del documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Estrae elementi dal documento contenitore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Un array di elementi estratti.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Estrae elementi dal documento contenitore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Il flusso del documento. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Un array di elementi estratti.

