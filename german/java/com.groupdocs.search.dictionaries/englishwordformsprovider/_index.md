---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Anbieter für englische Wortformen dar."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Stellt einen Anbieter für englische Wortformen dar.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Initialisiert eine neue Instanz von |
EnglishWordFormsProvider
Klasse.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Liefert die Wortformen für das angegebene Wort. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Initialisiert eine neue Instanz von
EnglishWordFormsProvider
Klasse.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Liefert die Wortformen für das angegebene Wort.
Das resultierende Array enthält das Originalwort nicht.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort, für das die Wortformen vorgeschlagen werden. |
|

**Returns:**
java.lang.String[] - Die Wortformen für das angegebene Wort oder ein leeres Array, wenn der IWordFormsProvider keine Wortformen für das angegebene Wort bereitstellt.

