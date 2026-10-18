---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Container für Attributänderungen dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Stellt einen Container für Attributänderungen dar.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Initialisiert eine neue Instanz der Klasse AttributeChangeBatch. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Initialisiert eine neue Instanz der Klasse AttributeChangeBatch. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Fügt die angegebenen Attribute dem angegebenen indizierten Dokument hinzu. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Fügt die angegebenen Attribute den angegebenen indizierten Dokumenten hinzu. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Fügt die angegebenen Attribute allen Dokumenten im Index hinzu. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Entfernt die angegebenen Attribute aus dem angegebenen indizierten Dokument. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Entfernt die angegebenen Attribute aus den angegebenen indizierten Dokumenten. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Entfernt alle Attribute aus dem angegebenen indizierten Dokument. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Entfernt alle Attribute aus den angegebenen indizierten Dokumenten. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Entfernt die angegebenen Attribute aus allen Dokumenten im Index. |
|
|  | [clear()](#clear--) | Entfernt alle Attribute aus allen Dokumenten im Index. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Initialisiert eine neue Instanz der Klasse AttributeChangeBatch.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Initialisiert eine neue Instanz der Klasse AttributeChangeBatch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Fügt die angegebenen Attribute dem angegebenen indizierten Dokument hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Dokumentpfad. |
|
|  | Attribute | java.lang.String[] | Die hinzuzufügenden Attribute. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Fügt die angegebenen Attribute den angegebenen indizierten Dokumenten hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade der Dokumente. |
|
|  | Attribute | java.lang.String[] | Die hinzuzufügenden Attribute. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Fügt die angegebenen Attribute allen Dokumenten im Index hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Attribute | java.lang.String[] | Die hinzuzufügenden Attribute. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Entfernt die angegebenen Attribute aus dem angegebenen indizierten Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Dokumentpfad. |
|
|  | Attribute | java.lang.String[] | Die zu entfernenden Attribute. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Entfernt die angegebenen Attribute aus den angegebenen indizierten Dokumenten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade der Dokumente. |
|
|  | Attribute | java.lang.String[] | Die zu entfernenden Attribute. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Entfernt alle Attribute aus dem angegebenen indizierten Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Dokumentpfad. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Entfernt alle Attribute aus den angegebenen indizierten Dokumenten.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade der Dokumente. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Entfernt die angegebenen Attribute aus allen Dokumenten im Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Attribute | java.lang.String[] | Die zu entfernenden Attribute. |
|

### clear() {#clear--}
```
public void clear()
```


Entfernt alle Attribute aus allen Dokumenten im Index.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
