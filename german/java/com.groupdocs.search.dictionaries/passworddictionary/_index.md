---
title: "PasswordDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Wörterbuchs für Dokumentpasswörter."
type: docs
weight: 20
url: /de/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Definiert die Schnittstelle eines Wörterbuchs für Dokumentpasswörter.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Liest die Anzahl der im Wörterbuch enthaltenen Elemente. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Liest das Passwort für die Datei. |
|
|  | [clear()](#clear--) | Entfernt alle Passwörter aus diesem  PasswordDictionary  Objekt. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Bestimmt, ob das Wörterbuch ein Passwort für das angegebene Dokument enthält. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Fügt dem Wörterbuch ein Passwort für ein Dokument hinzu. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Entfernt ein Passwort des angegebenen Dokuments aus dem Wörterbuch. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Liest die Anzahl der im Wörterbuch enthaltenen Elemente.


**Returns:**
int - Die Anzahl der im Wörterbuch enthaltenen Elemente.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Liest das Passwort für die Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad. |
|

**Returns:**
java.lang.String - Das Passwort für die Datei.

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Passwörter aus diesem  PasswordDictionary  Objekt.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Bestimmt, ob das Wörterbuch ein Passwort für das angegebene Dokument enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad des Dokuments. |
|

**Returns:**
boolean -  true  wenn das Wörterbuch ein Passwort für das Dokument enthält; andernfalls  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Fügt dem Wörterbuch ein Passwort für ein Dokument hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad des Dokuments. |
|
|  | Passwort | java.lang.String | Das Dokumentenpasswort. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Entfernt ein Passwort des angegebenen Dokuments aus dem Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Dateipfad des Dokuments. |
|

**Returns:**
boolean -  true  wenn das Passwort erfolgreich entfernt wurde; andernfalls  false . Diese Methode gibt außerdem  false  zurück, wenn  filePath  im Wörterbuch nicht gefunden wurde.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.String> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

