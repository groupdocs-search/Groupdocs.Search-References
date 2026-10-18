---
title: "ExtractorSettings"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Contiene configuraciones para el extractor de datos del documento."
type: docs
weight: 19
url: /es/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Contiene configuraciones para el extractor de datos del documento.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Obtiene el tipo de índice para el que se utiliza el extractor. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Establece el tipo de índice para el que se utiliza el extractor. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Obtiene el tipo de índice para el que se utiliza el extractor. El valor predeterminado es  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Establece el tipo de índice para el que se utiliza el extractor. El valor predeterminado es  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | El tipo de índice para el que se utiliza el extractor. |
|

