---
title: "SpellingCorrector"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Rechtschreibkorrekturs für Begriffe in einer Abfrage."
type: docs
weight: 21
url: /de/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Definiert die Schnittstelle eines Rechtschreibkorrekturs für Begriffe in einer Abfrage.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Ermittelt die Anzahl der Wörter, die in diesem  SpellingCorrector  enthalten sind. |
|
|  | [getWords()](#getWords--) | Ermittelt die Sammlung von Wörtern, die derzeit in diesem  SpellingCorrector  enthalten ist. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des SpellingCorrector hinzu. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des SpellingCorrector hinzu. |
|
|  | [clear()](#clear--) | Entfernt alle Wörter aus einem SpellingCorrector-Objekt. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ermittelt die Anzahl der Wörter, die in diesem  SpellingCorrector  enthalten sind.


**Returns:**
int - Die Anzahl der Wörter, die in diesem SpellingCorrector enthalten sind.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Ermittelt die Sammlung von Wörtern, die derzeit in diesem  SpellingCorrector  enthalten ist.


**Returns:**
java.lang.String[] - Die Sammlung von Wörtern.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des SpellingCorrector hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.Iterable<java.lang.String> | Die Sammlung von Wörtern, die dem Wörterbuch hinzugefügt werden sollen. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des SpellingCorrector hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.String[] | Die Sammlung von Wörtern, die dem Wörterbuch hinzugefügt werden sollen. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Wörter aus einem SpellingCorrector-Objekt.


