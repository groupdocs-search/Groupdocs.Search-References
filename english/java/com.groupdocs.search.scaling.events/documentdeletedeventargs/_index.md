---
title: DocumentDeletedEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of a document deletion is finished.
type: docs
weight: 11
url: /java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

Represents arguments for the event of a document deletion is finished.
## Methods

| Method | Description |
| --- | --- |
| [getShardIndex()](#getShardIndex--) | Gets the shard index. |
| [getDocumentKey()](#getDocumentKey--) | Gets the document key. |
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Gets the shard index.

**Returns:**
int - The shard index.
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Gets the document key.

**Returns:**
java.lang.String - The document key.
