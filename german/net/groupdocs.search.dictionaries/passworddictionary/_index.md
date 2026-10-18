---
title: "PasswordDictionary"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Wörterbuch für Dokumentenpasswörter dar."
type: docs
weight: 480
url: /de/net/groupdocs.search.dictionaries/passworddictionary/
---
## PasswordDictionary class

Stellt ein Wörterbuch für Dokumentenpasswörter dar.

```csharp
public class PasswordDictionary : DictionaryBase, IEnumerable<string>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/passworddictionary/count) { get; } | Ruft die Anzahl der im Wörterbuch enthaltenen Elemente ab. |
| override [DictionaryType](../../groupdocs.search.dictionaries/passworddictionary/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/passworddictionary/add)(string, string) | Fügt dem Wörterbuch ein Passwort für ein Dokument hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/passworddictionary/clear)() | Entfernt alle Passwörter aus diesem [`PasswordDictionary`](../passworddictionary)-Objekt. |
| [Contains](../../groupdocs.search.dictionaries/passworddictionary/contains)(string) | Bestimmt, ob das Wörterbuch ein Passwort für das angegebene Dokument enthält. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetEnumerator](../../groupdocs.search.dictionaries/passworddictionary/getenumerator)() | Gibt einen Enumerator zurück, der die Sammlung durchläuft. |
| [GetPassword](../../groupdocs.search.dictionaries/passworddictionary/getpassword)(string) | Ruft das Passwort für die Datei ab. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |
| [Remove](../../groupdocs.search.dictionaries/passworddictionary/remove)(string) | Entfernt das Passwort des angegebenen Dokuments aus dem Wörterbuch. |

### Hinweise

**Learn more**

* [Indexing password protected documents](https://docs.groupdocs.com/display/searchnet/Indexing+password+protected+documents)
* [Managing document passwords](https://docs.groupdocs.com/display/searchnet/Document+passwords)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
