---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός έναρξης προετοιμασίας εικόνας."
type: docs
weight: 15
url: /el/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός έναρξης προετοιμασίας εικόνας.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Λαμβάνει το κλειδί του εγγράφου. |
|
|  | [getInnerPath()](#getInnerPath--) | Λαμβάνει τη εσωτερική διαδρομή ενός ενσωματωμένου εγγράφου. |
|
|  | [getImageIndex()](#getImageIndex--) | Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο. |
|
|  | [getImageFrames()](#getImageFrames--) | Λαμβάνει τα πλαίσια της εικόνας. |
|
|  | [getImageStream()](#getImageStream--) | Λαμβάνει τη ροή της εικόνας. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Λαμβάνει το κλειδί του εγγράφου.


**Returns:**
java.lang.String - Το κλειδί του εγγράφου.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Λαμβάνει τη εσωτερική διαδρομή ενός ενσωματωμένου εγγράφου.


**Returns:**
java.lang.String[] - Η εσωτερική διαδρομή ενός ενσωματωμένου εγγράφου.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Λαμβάνει τον διαδοχικό αριθμό της εικόνας στο έγγραφο.


**Returns:**
int - Ο διαδοχικός αριθμός της εικόνας στο έγγραφο.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Λαμβάνει τα πλαίσια της εικόνας.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Τα πλαίσια της εικόνας.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Λαμβάνει τη ροή της εικόνας.


**Returns:**
java.io.InputStream - Η ροή της εικόνας.

