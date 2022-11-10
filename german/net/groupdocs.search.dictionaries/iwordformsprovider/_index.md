---
title: IWordFormsProvider
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Definiert die Schnittstelle eines Wortformanbieters.
type: docs
weight: 440
url: /de/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

Definiert die Schnittstelle eines Wortformanbieters.

```csharp
public interface IWordFormsProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | Ruft die Wortformen für das angegebene Wort ab. Das resultierende Array enthält nicht das ursprüngliche Wort. |

### Bemerkungen

**Mehr erfahren**

* [Suchen Sie nach verschiedenen Wortformen](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [Anbieter von Word-Formularen](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### Beispiele

Das folgende Beispiel zeigt, wie ein benutzerdefinierter Wortformanbieter implementiert wird.

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // Angenommen, das eingegebene Wort steht im Plural, dann fügen wir den Singular hinzu
        if (word.Length > 2 &&
            word.EndsWith("es", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 2));
        }
        if (word.Length > 1 &&
            word.EndsWith("s", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1));
        }

        // Dann nehmen wir an, dass das Eingabewort im Singular steht, wir fügen den Plural hinzu
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // Alle Regeln sind in der Klasse EnglishWordFormsProvider implementiert

        return result.ToArray();
    }
}
```

Das nächste Beispiel zeigt, wie Sie einen benutzerdefinierten Wortformanbieter für die Verwendung festlegen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// Index im angegebenen Ordner erstellen
Index index = new Index(indexFolder);
  
// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
 
// Festlegen der Instanz des Anbieters für benutzerdefinierte Wortformen
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// Erstellen einer Suchoptionsinstanz
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // Suche nach Wortformen aktivieren
  
// Suche im Index
SearchResult result = index.Search("relative", options);
  
// Die folgenden Wörter können gefunden werden:
// relativ
// relativs
```

### Siehe auch

* namensraum [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* Montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->