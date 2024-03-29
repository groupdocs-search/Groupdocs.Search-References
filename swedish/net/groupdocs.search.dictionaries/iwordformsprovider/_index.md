---
title: IWordFormsProvider
second_title: GroupDocs.Search efter .NET API Reference
description: Definierar gränssnittet för en ordformsleverantör.
type: docs
weight: 450
url: /sv/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

Definierar gränssnittet för en ordformsleverantör.

```csharp
public interface IWordFormsProvider
```

## Metoder

| namn | Beskrivning |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | Hämtar ordformerna för det angivna ordet. Den resulterande arrayen innehåller inte det ursprungliga ordet. |

### Anmärkningar

**Läs mer**

* [Sök efter olika ordformer](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [Ordformulärsleverantör](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### Exempel

Följande exempel visar hur man implementerar en anpassad ordformsleverantör.

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // Antag att inmatningsordet är i plural, då lägger vi till singular
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

        // Antag sedan att inmatningsordet är i singular, vi lägger till plural
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // Alla regler är implementerade i klassen EnglishWordFormsProvider

        return result.ToArray();
    }
}
```

Nästa exempel visar hur man ställer in en anpassad ordformsleverantör för användning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
  
// Indexering av dokument från den angivna mappen
index.Add(documentsFolder);
 
// Ställa in den anpassade ordformsleverantörsinstansen
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// Skapar en sökalternativsinstans
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // Möjliggör sökning efter ordformer
  
// Söker i indexet
SearchResult result = index.Search("relative", options);
  
// Följande ord kan hittas:
// relativ
// relativs
```

### Se även

* namnutrymme [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
