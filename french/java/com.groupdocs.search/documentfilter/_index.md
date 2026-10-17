---
title: "DocumentFilter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente la classe de base pour les filtres de documents."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Représente la classe de base pour les filtres de documents. Contient des méthodes pour la création d'instances de filtres de documents.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [toString()](#toString--) | Renvoie la représentation sous forme de chaîne d'un filtre de document. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de création est antérieure à la limite inférieure. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de création est postérieure à la limite supérieure. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de création est hors de la plage spécifiée. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de modification est antérieure à la limite inférieure. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de modification est postérieure à la limite supérieure. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Crée un filtre pour ignorer les documents dont la date de modification est hors de la plage spécifiée. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Crée un filtre pour ignorer les documents dont la longueur est inférieure à la limite inférieure. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Crée un filtre pour ignorer les documents dont la longueur est supérieure à la limite supérieure. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Crée un filtre pour ignorer les documents hors de la plage de longueur de document spécifiée. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Crée un filtre pour ignorer les documents qui n'ont pas d'extension autorisée. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Crée un filtre dont la logique est inverse par rapport au filtre interne spécifié. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Crée une conjonction logique des filtres spécifiés. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Crée une disjonction logique des filtres spécifiés. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Renvoie la représentation sous forme de chaîne d'un filtre de document.


**Returns:**
java.lang.String - Représentation sous forme de chaîne d'un filtre de document.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Crée un filtre pour ignorer les documents dont la date de création est antérieure à la limite inférieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | java.util.Date | La limite inférieure du moment de création du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Crée un filtre pour ignorer les documents dont la date de création est postérieure à la limite supérieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | upperBound | java.util.Date | La limite supérieure du moment de création du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Crée un filtre pour ignorer les documents dont la date de création est hors de la plage spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | java.util.Date | La limite inférieure du moment de création du document. |
|
|  | upperBound | java.util.Date | La limite supérieure du moment de création du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Crée un filtre pour ignorer les documents dont la date de modification est antérieure à la limite inférieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | java.util.Date | La limite inférieure du moment de modification du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Crée un filtre pour ignorer les documents dont la date de modification est postérieure à la limite supérieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | upperBound | java.util.Date | La limite supérieure du moment de modification du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Crée un filtre pour ignorer les documents dont la date de modification est hors de la plage spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | java.util.Date | La limite inférieure du moment de modification du document. |
|
|  | upperBound | java.util.Date | La limite supérieure du moment de modification du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le motif de l'expression régulière. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | motif | java.lang.String | Le motif de l'expression régulière. |
|
|  | options | int | Les options de l'expression régulière. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Crée un filtre pour ignorer les documents dont la longueur est inférieure à la limite inférieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | long | La limite inférieure de la longueur du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Crée un filtre pour ignorer les documents dont la longueur est supérieure à la limite supérieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | upperBound | long | La limite supérieure de la longueur du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Crée un filtre pour ignorer les documents hors de la plage de longueur de document spécifiée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | lowerBound | long | La limite inférieure de la longueur du document. |
|
|  | upperBound | long | La limite supérieure de la longueur du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Crée un filtre pour ignorer les documents qui n'ont pas d'extension autorisée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | extensions | java.lang.String[] | La liste des extensions autorisées. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Crée un filtre dont la logique est inverse par rapport au filtre interne spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Le filtre interne du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Crée une conjonction logique des filtres spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Les filtres du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Crée une disjonction logique des filtres spécifiés.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Les filtres du document. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

