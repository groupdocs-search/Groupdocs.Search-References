---
title: "追加"
second_title: "GroupDocs.Search for .NET API リファレンス"
description: "インデックス作成操作を実行します。絶対パスまたは相対パスでファイルまたはフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。"
type: docs
weight: 80
url: /ja/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

インデックス作成操作を実行します。絶対パスまたは相対パスでファイルまたはフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。

```csharp
public void Add(string path)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | String | インデックス対象のファイルまたはフォルダーへのパスです。 |

### 例

この例は、ドキュメントをインデックスに追加する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### 関連項目

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

インデックス作成操作を実行します。絶対パスまたは相対パスでファイルまたはフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。

```csharp
public void Add(string path, IndexingOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | String | インデックス対象のファイルまたはフォルダーへのパスです。 |
| オプション | IndexingOptions | インデックス作成オプションです。 |

### 例

この例は、特定のインデックス作成オプションを使用してドキュメントをインデックスに追加する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### 関連項目

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

インデックス作成操作を実行します。絶対パスまたは相対パスでファイルやフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。

```csharp
public void Add(string[] paths)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | String[] | インデックス対象のファイルやフォルダーへのパスです。 |

### 例

この例は、ドキュメントをインデックスに追加する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### 関連項目

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

インデックス作成操作を実行します。絶対パスまたは相対パスでファイルやフォルダーを追加します。すべてのサブフォルダーのドキュメントがインデックスされます。

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | String[] | インデックス対象のファイルやフォルダーへのパスです。 |
| オプション | IndexingOptions | インデックス作成オプションです。 |

### 例

この例は、特定のインデックス作成オプションを使用してドキュメントをインデックスに追加する方法を示しています。

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### 関連項目

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

インデックス作成操作を実行します。ファイルシステム、ストリーム、または構造からドキュメントを追加します。

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| documents | Document[] | ファイルシステム、ストリーム、または構造からのドキュメントです。 |
| オプション | IndexingOptions | インデックス作成オプションです。 |

### 関連項目

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

インデックス作成操作を実行します。抽出されたデータをインデックスに追加します。

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| data | ExtractedData[] | 抽出されたデータです。 |
| オプション | IndexingOptions | インデックス作成オプションです。 |

### 関連項目

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
