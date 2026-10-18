---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που συμβαίνει όταν ένα έγγραφο προστατευμένο με κωδικό ευρετηριάζεται."
type: docs
weight: 20
url: /el/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που συμβαίνει όταν ένα έγγραφο προστατευμένο με κωδικό ευρετηριάζεται.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Λαμβάνει τη πλήρη διαδρομή του εγγράφου. |
|
|  | [getPassword()](#getPassword--) | Λαμβάνει τον κωδικό πρόσβασης για το άνοιγμα του εγγράφου. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης για το άνοιγμα του εγγράφου. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Λαμβάνει τη πλήρη διαδρομή του εγγράφου.


**Returns:**
java.lang.String - Η πλήρης διαδρομή του εγγράφου.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Λαμβάνει τον κωδικό πρόσβασης για το άνοιγμα του εγγράφου.


**Returns:**
java.lang.String - Ο κωδικός πρόσβασης για το άνοιγμα του εγγράφου.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης για το άνοιγμα του εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Ο κωδικός πρόσβασης για το άνοιγμα του εγγράφου. |
|

