---
title: "ExtractorSettings"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Contiene le impostazioni per l'estrattore di dati del documento."
type: docs
weight: 19
url: /it/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Contiene le impostazioni per l'estrattore di dati del documento.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Ottiene il tipo di indice per cui viene utilizzato l'estrattore. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Imposta il tipo di indice per cui viene utilizzato l'estrattore. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Ottiene il tipo di indice per cui viene utilizzato l'estrattore. Il valore predefinito è  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Imposta il tipo di indice per cui viene utilizzato l'estrattore. Il valore predefinito è  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Il tipo di indice per cui viene utilizzato l'estrattore. |
|

