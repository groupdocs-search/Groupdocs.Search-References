---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Informationen zu einem Container-Element dar."
type: docs
weight: 18
url: /de/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Stellt Informationen zu einem Container-Element dar.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Initialisiert eine neue Instanz der Klasse ExtractedItemInfo. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Gibt einen Dokumenttyp zurück. |
|
|  | [getFields()](#getFields--) | Gibt extrahierte Felder zurück. |
|
|  | [getItemInfo()](#getItemInfo--) | Ruft eine Elementinformation ab. |
|
|  | [getInnerPath()](#getInnerPath--) | Ruft einen inneren Pfad ab. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Initialisiert eine neue Instanz der Klasse ExtractedItemInfo.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Die Dokumentformatfamilie. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Die extrahierten Felder. |
|
|  | itemInfo | java.lang.String | Die Elementinformation. |
|
|  | innerPath | java.lang.String | Der Pfad zum Element im Container. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Gibt einen Dokumenttyp zurück.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Gibt extrahierte Felder zurück.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Die extrahierten Felder.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Ruft eine Elementinformation ab.


**Returns:**
java.lang.String - Die Elementinformation.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Ruft einen inneren Pfad ab.


**Returns:**
java.lang.String - Der innere Pfad.

