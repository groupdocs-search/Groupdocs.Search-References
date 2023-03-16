---
title: IWordFormsProvider
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: एक शब्द प्रपत्र प्रदत के इंटरफ़ेस क परभषत करत है
type: docs
weight: 450
url: /hi/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

एक शब्द प्रपत्र प्रदाता के इंटरफ़ेस को परिभाषित करता है।

```csharp
public interface IWordFormsProvider
```

## तरीकों

| नाम | विवरण |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | निर्दिष्ट शब्द के लिए शब्द रूप प्राप्त करता है। परिणामी सरणी में मूल शब्द नहीं है। |

### टिप्पणियों

**और अधिक जानें**

* [विभिन्न शब्द रूपों की खोज करें](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [शब्द प्रपत्र प्रदाता](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि कस्टम शब्द प्रपत्र प्रदाता को कैसे लागू किया जाए।

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // मान लें कि इनपुट शब्द बहुवचन में है, तो हम एकवचन जोड़ते हैं
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

        // फिर मान लें कि इनपुट शब्द एकवचन में है, हम बहुवचन जोड़ते हैं
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // सभी नियम EnglishWordFormsProvider क्लास में लागू किए गए हैं

        return result.ToArray();
    }
}
```

अगला उदाहरण प्रदर्शित करता है कि उपयोग करने के लिए एक कस्टम शब्द प्रपत्र प्रदाता कैसे सेट करें.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// निर्दिष्ट फ़ोल्डर में एक इंडेक्स बनाना
Index index = new Index(indexFolder);
  
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण
index.Add(documentsFolder);
 
// कस्टम वर्ड फॉर्म प्रोवाइडर इंस्टेंस सेट करना
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// एक खोज विकल्प उदाहरण बनाना
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // शब्द रूपों की खोज को सक्षम करना
  
// इंडेक्स में खोजा जा रहा है
SearchResult result = index.Search("relative", options);
  
// निम्नलिखित शब्द मिल सकते हैं:
// रिश्तेदार
// रिश्तेदारs
```

### यह सभी देखें

* नाम स्थान [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* सभा [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->