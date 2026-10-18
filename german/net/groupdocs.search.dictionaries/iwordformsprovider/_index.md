---
title: "IWordFormsProvider"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Definiert die Schnittstelle eines Anbieters für Wortformen."
type: docs
weight: 470
url: /de/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

Definiert die Schnittstelle eines Anbieters für Wortformen.

```csharp
public interface IWordFormsProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | Liefert die Wortformen für das angegebene Wort. Das resultierende Array enthält das ursprüngliche Wort nicht. |

### Hinweise

**Learn more**

* [Search for different word forms](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [Word forms provider](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### Beispiele

Das folgende Beispiel zeigt, wie man einen benutzerdefinierten Wortformen‑Provider implementiert.

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // Angenommen, das Eingabewort ist im Plural, dann fügen wir die Einzahl hinzu.
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

        // Dann nehmen wir an, dass das Eingabewort in der Einzahl ist, wir fügen den Plural hinzu.
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // Alle Regeln sind in der Klasse EnglishWordFormsProvider implementiert.

        return result.ToArray();
    }
}
```

Das nächste Beispiel zeigt, wie man einen benutzerdefinierten Wortformen‑Provider für die Verwendung festlegt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);
  
// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
 
// Einstellen der benutzerdefinierten Wortformen‑Provider‑Instanz
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// Erstellen einer Suchoptionen‑Instanz
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // Enabling search for word forms
  
// Durchsuchen des Index
SearchResult result = index.Search("relative", options);
  
// Die folgenden Wörter können gefunden werden:
// relativ
// Verwandte
```

### Siehe auch

* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
