---
title: "MergeOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'opération de fusion."
type: docs
weight: 28
url: /fr/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Fournit des options pour l'opération de fusion.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Initialise une nouvelle instance de la classe  MergeOptions. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [isAsync()](#isAsync--) | Obtient le drapeau d'exécution asynchrone de l'opération. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Définit le drapeau d'exécution asynchrone de l'opération. |
|
|  | [getCancellation()](#getCancellation--) | Obtient l'objet d'annulation de l'opération. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Définit l'objet d'annulation de l'opération. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Initialise une nouvelle instance de la classe  MergeOptions.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Obtient le drapeau d'exécution asynchrone de l'opération. La valeur par défaut est false.


**Returns:**
boolean - Le drapeau d'exécution asynchrone de l'opération.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Définit le drapeau d'exécution asynchrone de l'opération. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau d'exécution asynchrone de l'opération. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Obtient l'objet d'annulation de l'opération. La valeur par défaut est null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Définit l'objet d'annulation de l'opération. La valeur par défaut est null.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'objet d'annulation de l'opération. |
|

