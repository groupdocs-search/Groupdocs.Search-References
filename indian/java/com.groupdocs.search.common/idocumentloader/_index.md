---
title: "IDocumentLoader"
second_title: "GroupDocs.Search for Java API Reference"
description: "लेज़ी दस्तावेज़ों को लोड करने के लिए उपयोग किए जाने वाले दस्तावेज़ लोडर इंटरफ़ेस को परिभाषित करता है।"
type: docs
weight: 36
url: /hi/java/com.groupdocs.search.common/idocumentloader/
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


