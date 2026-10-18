---
title: "DocumentDeletedEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer een documentverwijdering is voltooid."
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

Stelt de argumenten voor het evenement voor wanneer een documentverwijdering is voltooid.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Haalt de shard-index op. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Haalt de document-sleutel op. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Haalt de shard-index op.


**Returns:**
int - De shard-index.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Haalt de document-sleutel op.


**Returns:**
java.lang.String - De document-sleutel.

