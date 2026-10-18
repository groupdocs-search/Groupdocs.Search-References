---
title: "IndexStatus"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Specificeert een indexstatus."
type: docs
weight: 41
url: /nl/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Specificeert een indexstatus.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Ready](#Ready) | Index is vrij en klaar om te wijzigen. |
|
|  | [Failed](#Failed) | Index moet opnieuw worden geladen vanwege een fout. |
|
|  | [Indexing](#Indexing) | Index voert een indexeerbewerking uit. |
|
|  | [Updating](#Updating) | Index voert een updatebewerking uit. |
|
|  | [Merging](#Merging) | Index voert een samenvoegingsbewerking uit. |
|
|  | [Optimizing](#Optimizing) | Index voert een optimalisatiebewerking uit. |
|
|  | [Deleting](#Deleting) | Index voert een verwijderingsbewerking uit. |
|
|  | [Renaming](#Renaming) | Index voert een hernoembewerking uit. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Index wijzigt attributen. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Index is vrij en klaar om te wijzigen.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Index moet opnieuw worden geladen vanwege een fout.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Index voert een indexeerbewerking uit.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Index voert een updatebewerking uit.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Index voert een samenvoegingsbewerking uit.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Index voert een optimalisatiebewerking uit.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Index voert een verwijderingsbewerking uit.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Index voert een hernoembewerking uit.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Index wijzigt attributen.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
