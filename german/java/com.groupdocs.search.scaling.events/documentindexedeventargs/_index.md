---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn die Indexierung eines Dokuments abgeschlossen ist."
type: docs
weight: 12
url: /de/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Stellt Argumente für das Ereignis dar, wenn die Indexierung eines Dokuments abgeschlossen ist.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Ermittelt den Shard-Index. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Ermittelt den Dokumentenschlüssel. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Ermittelt den Shard-Index.


**Returns:**
int - Der Shard-Index.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Ermittelt den Dokumentenschlüssel.


**Returns:**
java.lang.String - Der Dokumentenschlüssel.

