---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "इंडेक्सिंग प्रक्रिया के दौरान उपयोग की जाने वाली अक्षर प्रतिस्थापन शब्दकोश को दर्शाता है। अक्षर प्रतिस्थापन का उपयोग उदाहरण के लिए उच्चारित अक्षरों से एक्सेंट हटाने या केस-इनसेंसिटिव इंडेक्स बनाने के लिए किया जा सकता है।"
type: docs
weight: 390
url: /hi/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

इंडेक्सिंग प्रक्रिया के दौरान उपयोग किए जाने वाले अक्षर प्रतिस्थापन शब्दकोश को दर्शाता है। उदाहरण के लिए, अक्षर प्रतिस्थापन का उपयोग उच्चारण चिह्न हटाने या केस-इंसेंसिटिव इंडेक्स बनाने के लिए किया जा सकता है।

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | इस [`CharacterReplacementDictionary`](../characterreplacementdictionary) में मौजूद Unicode कोड पॉइंट्स की संख्या प्राप्त करता है। |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | डिक्शनरी का प्रकार प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | निर्दिष्ट अक्षर प्रतिस्थापनों के संग्रह को इस [`CharacterReplacementDictionary`](../characterreplacementdictionary) के उदाहरण में जोड़ता है। |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | निर्दिष्ट अक्षर प्रतिस्थापनों के संग्रह को इस [`CharacterReplacementDictionary`](../characterreplacementdictionary) के उदाहरण में जोड़ता है। |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | निर्दिष्ट अक्षर प्रतिस्थापनों के संग्रह को इस [`CharacterReplacementDictionary`](../characterreplacementdictionary) के उदाहरण में जोड़ता है। |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | निर्दिष्ट Unicode कोड पॉइंट प्रतिस्थापनों के संग्रह को इस [`CharacterReplacementDictionary`](../characterreplacementdictionary) के उदाहरण में जोड़ता है। |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | एक [`CharacterReplacementDictionary`](../characterreplacementdictionary) ऑब्जेक्ट से सभी अक्षर प्रतिस्थापन हटाता है। |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | निर्धारित करता है कि एक [`CharacterReplacementDictionary`](../characterreplacementdictionary) ऑब्जेक्ट में निर्दिष्ट Unicode कोड पॉइंट के लिए प्रतिस्थापन है या नहीं। |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | डिक्शनरी को निर्दिष्ट नाम वाली फ़ाइल में निर्यात करता है। |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | एक इटेरेटर लौटाता है जो संग्रह के माध्यम से इटरिट करता है। |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | निर्दिष्ट यूनिकोड कोड पॉइंट के लिए एक प्रतिस्थापन प्राप्त करता है। |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | निर्दिष्ट फ़ाइल से एक डिक्शनरी आयात करता है। |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | इस उदाहरण से निर्दिष्ट कैरेक्टर प्रतिस्थापनों के संग्रह को हटाता है [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | इस उदाहरण से निर्दिष्ट कैरेक्टर प्रतिस्थापनों के संग्रह को हटाता है [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | इस उदाहरण से निर्दिष्ट यूनिकोड कोड पॉइंट प्रतिस्थापनों के संग्रह को हटाता है [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | इस उदाहरण से निर्दिष्ट यूनिकोड कोड पॉइंट प्रतिस्थापनों के संग्रह को हटाता है [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### टिप्पणियाँ

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### संबंधित देखें

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
