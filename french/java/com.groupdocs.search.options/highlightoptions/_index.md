---
title: "HighlightOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour la mise en évidence des termes trouvés."
type: docs
weight: 22
url: /fr/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Fournit des options pour la mise en évidence des termes trouvés.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialise une nouvelle instance de la classe  HighlightOptions . |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  TextOptions . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Obtient le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Définit le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Obtient le nombre maximal de mots dans un extrait de texte après le mot mis en évidence. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Définit le nombre maximal de mots dans un extrait de texte après le mot mis en évidence. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Obtient le nombre maximal de mots dans un extrait de texte. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Définit le nombre maximal de mots dans un extrait de texte. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Obtient une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Définit une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Obtient une couleur utilisée pour mettre en évidence les occurrences. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Définit une couleur utilisée pour mettre en évidence les occurrences. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Obtient la balise de début du surlignage du mot trouvé. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Définit la balise de début du surlignage du mot trouvé. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Obtient la balise de fin du surlignage du mot trouvé. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Définit la balise de fin du surlignage du mot trouvé. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialise une nouvelle instance de la classe  HighlightOptions .


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Initialise une nouvelle instance de la classe  TextOptions .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Obtient le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 7.


**Returns:**
int - Le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Définit le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 7.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de mots dans un extrait de texte avant le mot mis en évidence. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Obtient le nombre maximal de mots dans un extrait de texte après le mot mis en évidence. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 7.


**Returns:**
int - Le nombre maximal de mots dans un extrait de texte après le mot mis en évidence.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Définit le nombre maximal de mots dans un extrait de texte après le mot mis en évidence. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 7.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de mots dans un extrait de texte après le mot mis en évidence. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Obtient le nombre maximal de mots dans un extrait de texte. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 21.


**Returns:**
int - Le nombre maximal de mots dans un extrait de texte.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Définit le nombre maximal de mots dans un extrait de texte. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est 21.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre maximal de mots dans un extrait de texte. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Obtient une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences. La valeur par défaut est true.


**Returns:**
boolean - Une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Définit une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences. La valeur par défaut est true.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si les styles en ligne sont utilisés pour mettre en évidence les occurrences. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Obtient une couleur utilisée pour mettre en évidence les occurrences. La valeur par défaut est #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Définit une couleur utilisée pour mettre en évidence les occurrences. La valeur par défaut est #FFD800.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Une couleur utilisée pour mettre en évidence les occurrences. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Obtient la balise de début du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide.


**Returns:**
java.lang.String - La balise de début du surlignage du mot trouvé.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Définit la balise de début du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | La balise de début du surlignage du mot trouvé. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Obtient la balise de fin du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide.


**Returns:**
java.lang.String - La balise de fin du surlignage du mot trouvé.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Définit la balise de fin du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | La balise de fin du surlignage du mot trouvé. |
|

