---
title: "MergeOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für den Zusammenführungsvorgang bereit."
type: docs
weight: 28
url: /de/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Stellt Optionen für den Zusammenführungsvorgang bereit.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Initialisiert eine neue Instanz der MergeOptions-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isAsync()](#isAsync--) | Liest das Flag für die asynchrone Ausführung der Operation. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Setzt das Flag für die asynchrone Ausführung der Operation. |
|
|  | [getCancellation()](#getCancellation--) | Liest das Abbruchobjekt der Operation. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Setzt das Abbruchobjekt der Operation. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Initialisiert eine neue Instanz der MergeOptions-Klasse.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Gibt das Flag für die asynchrone Ausführung der Operation zurück. Der Standardwert ist  false .


**Returns:**
boolean - Das Flag für die asynchrone Ausführung der Operation.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Legt das Flag für die asynchrone Ausführung der Operation fest. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die asynchrone Ausführung der Operation. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Gibt das Abbruchobjekt der Operation zurück. Der Standardwert ist  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Legt das Abbruchobjekt der Operation fest. Der Standardwert ist  null .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Das Abbruchobjekt der Operation. |
|

