---
title: "SearchPhase"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa las fases de búsqueda."
type: docs
weight: 24
url: /es/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Representa las fases de búsqueda.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | La sustitución de alias. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | La corrección de la distribución del teclado. |
|
|  | [SpellingCorrection](#SpellingCorrection) | La corrección ortográfica. |
|
|  | [HomophoneSearch](#HomophoneSearch) | La búsqueda de homófonos. |
|
|  | [SynonymSearch](#SynonymSearch) | La búsqueda de sinónimos. |
|
|  | [WordFormsSearch](#WordFormsSearch) | La búsqueda de formas de palabras. |
|
|  | [FuzzySearch](#FuzzySearch) | La búsqueda difusa. |
|
|  | [WildcardMatching](#WildcardMatching) | La coincidencia con comodines. |
|
|  | [RegexMatching](#RegexMatching) | La coincidencia de expresiones regulares. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


La sustitución de alias.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


La corrección de la distribución del teclado.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


La corrección ortográfica.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


La búsqueda de homófonos.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


La búsqueda de sinónimos.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


La búsqueda de formas de palabras.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


La búsqueda difusa.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


La coincidencia con comodines.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


La coincidencia de expresiones regulares.


### values() {#values--}
```
public static SearchPhase[] values()
```




**Returns:**
com.groupdocs.search.events.SearchPhase[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchPhase valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
