---
title: "IWordFormsProvider"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Definisce l'interfaccia di un provider di forme di parole."
type: docs
weight: 470
url: /it/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

Definisce l'interfaccia di un provider di forme di parole.

```csharp
public interface IWordFormsProvider
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | Ottiene le forme della parola per la parola specificata. L'array risultante non contiene la parola originale. |

### Osservazioni

**Learn more**

* [Search for different word forms](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [Word forms provider](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### Esempi

Il seguente esempio dimostra come implementare un provider personalizzato di forme di parole.

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // Supponiamo che la parola di input sia al plurale, quindi aggiungiamo il singolare.
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

        // Supponiamo ora che la parola di input sia al singolare, aggiungiamo il plurale.
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // Tutte le regole sono implementate nella classe EnglishWordFormsProvider.

        return result.ToArray();
    }
}
```

Il prossimo esempio dimostra come impostare un provider personalizzato di forme di parole per l'utilizzo.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
  
// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
 
// Impostazione dell'istanza del provider personalizzato di forme di parole
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// Creazione di un'istanza di opzioni di ricerca
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // Enabling search for word forms
  
// Ricerca nell'indice
SearchResult result = index.Search("relative", options);
  
// Le seguenti parole possono essere trovate:
// relativo
// parenti
```

### Vedi anche

* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
