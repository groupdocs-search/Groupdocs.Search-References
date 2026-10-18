---
title: "DocumentDeletedEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när en dokumentradering är slutförd."
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

Representerar argument för händelsen när en dokumentradering är slutförd.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Hämtar fragmentets index. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Hämtar dokumentnyckeln. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Hämtar fragmentets index.


**Returns:**
int - Fragmentets index.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Hämtar dokumentnyckeln.


**Returns:**
java.lang.String - Dokumentnyckeln.

