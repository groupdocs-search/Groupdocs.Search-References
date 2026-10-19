---
title: "SearchQuery"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Представляет поисковый запрос в виде объекта."
type: docs
weight: 1580
url: /ru/net/groupdocs.search/searchquery/
---
## SearchQuery class

Представляет поисковый запрос в виде объекта.

```csharp
public abstract class SearchQuery
```

## Properties

| Name | Описание |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Получает количество дочерних запросов. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Получает имя поля. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Получает первый дочерний запрос. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Получает или задаёт параметры поиска этого поискового запроса. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Получает второй дочерний запрос. |

## Methods

| Name | Описание |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Создаёт комбинированный запрос, который найдёт только документы, найденные для каждого исходного запроса. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Создаёт комбинированный запрос, который найдёт только документы, найденные для каждого исходного запроса. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Создает запрос диапазона дат. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Добавляет поле к указанному запросу. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Создает инвертированный запрос, который найдет остальные документы в индексе, в отличие от тех, которые будут найдены оригинальным запросом. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Создает запрос числового диапазона. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Создает комбинированный запрос, который найдет все документы, найденные хотя бы одним из оригинальных запросов. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Создает комбинированный запрос, который найдет все документы, найденные хотя бы одним из оригинальных запросов. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Создает запрос поиска фразы. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Создает запрос регулярного выражения. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Создает запрос регулярного выражения. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Создает подстановочный шаблон для поиска фразы. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Создает подстановочный шаблон для поиска фразы. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Создает запрос шаблона слова. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Создает простой запрос слова. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Получает дочерний запрос по индексу. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Возвращает строку, представляющую текущий экземпляр [`SearchQuery`](../searchquery). |

### Примечания

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Примеры

Пример демонстрирует типичное использование класса.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Создание подзапроса поиска диапазона дат
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Создание подзапроса подстановки с количеством пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Создание объекта параметров поиска с увеличенной емкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### См. также

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
