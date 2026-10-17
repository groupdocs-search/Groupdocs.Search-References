---
title: "IDocumentLoader"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يعرف واجهة تحميل المستندات التي تُستخدم لتحميل المستندات المؤجلة."
type: docs
weight: 36
url: /ar/java/com.groupdocs.search.common/idocumentloader/
---```
public interface IDocumentLoader
```

Defines the document loader interface that is used to load lazy documents.

## Methods

| Method | Description |
| --- | --- |
| [loadDocument()](#loadDocument--) | Loads a document.
 |
| [closeDocument()](#closeDocument--) | Closes the loaded document.
 |
### loadDocument() {#loadDocument--}
```
public abstract Document loadDocument()
```


Loads a document. This method is called by the index when it is ready for processing the document.


**Returns:**
[Document](../../com.groupdocs.search/document) - The loaded document.

### closeDocument() {#closeDocument--}
```
public abstract void closeDocument()
```


Closes the loaded document. This method is called by the index when it has finished processing the document.


