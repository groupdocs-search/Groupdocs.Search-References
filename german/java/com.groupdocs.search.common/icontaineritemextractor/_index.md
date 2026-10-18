---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Methoden zum Extrahieren von Elementen aus Containerdokumenten bereit."
type: docs
weight: 35
url: /de/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Stellt Methoden zum Extrahieren von Elementen aus Containerdokumenten bereit.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Liefert die Dokumentformatfamilie. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extrahiert Elemente aus dem Containerdokument. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extrahiert Elemente aus dem Containerdokument. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Liefert die Dokumentformatfamilie.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extrahiert Elemente aus dem Containerdokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Ein Array extrahierter Elemente.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extrahiert Elemente aus dem Containerdokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Der Dokumenten-Stream. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Ein Array extrahierter Elemente.

