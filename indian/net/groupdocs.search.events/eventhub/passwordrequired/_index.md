---
title: PasswordRequired
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: तब हत है जब कस दस्तवेज़ क खलने के लए पसवर्ड क आवश्यकत हत है
type: docs
weight: 60
url: /hi/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

तब होता है जब किसी दस्तावेज़ को खोलने के लिए पासवर्ड की आवश्यकता होती है।

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### उदाहरण

उदाहरण दर्शाता है कि कैसे घटना का उपयोग करना है।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// इंडेक्स बनाना
Index index = new Index(indexFolder);

// घटना की सदस्यता लेना
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण
index.Add(documentsFolder);
```

### यह सभी देखें

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* नाम स्थान [GroupDocs.Search.Events](../../eventhub)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->