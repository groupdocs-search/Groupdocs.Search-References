---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Enthält eine Sammlung benutzerdefinierter Extraktoren."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält, die von integrierten Extraktoren abgedeckt wird, wird dieser Extraktor anstelle des integrierten verwendet.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [size()](#size--) | Liefert die Anzahl der in der Sammlung enthaltenen Extraktoren. |
|
|  | [isReadOnly()](#isReadOnly--) | Gibt einen Wert zurück, der angibt, ob die Sammlung schreibgeschützt ist. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator für diese Sammlung zurück. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Fügt einen Extraktor zur Sammlung hinzu. |
|
|  | [clear()](#clear--) | Entfernt alle Extraktoren aus der Sammlung. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Bestimmt, ob die Sammlung einen bestimmten Extraktor enthält. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Kopiert die Elemente der Sammlung in ein Array, beginnend bei einem bestimmten Array-Index. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Entfernt einen Extraktor aus der Sammlung. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Liefert die Anzahl der in der Sammlung enthaltenen Extraktoren.


**Returns:**
int - Die Anzahl der in der Sammlung enthaltenen Extraktoren.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Gibt einen Wert zurück, der angibt, ob die Sammlung schreibgeschützt ist.


**Returns:**
boolean - Ein Wert, der angibt, ob die Sammlung schreibgeschützt ist.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Gibt einen Iterator für diese Sammlung zurück.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Ein Iterator-Objekt, das verwendet werden kann, um durch die Sammlung zu iterieren.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Fügt einen Extraktor zur Sammlung hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der Extraktor, der zur Sammlung hinzugefügt werden soll. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Extraktoren aus der Sammlung.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Bestimmt, ob die Sammlung einen bestimmten Extraktor enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der Extraktor, der in der Sammlung gesucht werden soll. |
|

**Returns:**
boolean -  true  wenn  das  Element  in der Sammlung gefunden wird; andernfalls  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Kopiert die Elemente der Sammlung in ein Array, beginnend bei einem bestimmten Array-Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Das eindimensionale Array, das das Ziel der aus der Sammlung kopierten Elemente ist. Das Array muss nullbasierte Indizierung haben. |
|
|  | arrayIndex | int | Der nullbasierte Index im Array, an dem das Kopieren beginnt. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Entfernt einen Extraktor aus der Sammlung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der Extraktor, der aus der Sammlung entfernt werden soll. |
|

**Returns:**
boolean -  true  wenn  der  Extraktor  erfolgreich aus der Sammlung entfernt wurde; andernfalls  false . Diese Methode gibt ebenfalls  false  zurück, wenn  der  Extraktor  in der ursprünglichen Sammlung nicht gefunden wird.

