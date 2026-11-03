---
title: Features Overview
linkTitle: "Features overview"
second_title: GroupDocs.Search for Python via .NET API References
description: "GroupDocs.Search for Python via .NET creates, updates, merges and optimizes full-text indexes, and searches them with many search types: boolean, phrase, wildcard, regular expression, fuzzy, synonym, homophone, faceted, date and numeric range search, with highlighting, events and Python callbacks."
type: docs
url: /python-net/guides/features-overview/
is_root: false
weight: 40
---


GroupDocs.Search for Python via .NET indexes and searches documents of a wide range of [supported document formats](https://docs.groupdocs.com/search/python-net/supported-document-formats/). Every task follows the same workflow: create or open an [`Index`](/search/python-net/groupdocs.search/index/), `add()` documents to it, then `search()` it and read or highlight the results. The index lives in a folder of its own and is opened again on the next run, so documents are indexed once and searched many times. For details on a feature, follow the links to the [Developer Guide](https://docs.groupdocs.com/search/python-net/developer-guide/).

## Creating and opening indexes

Create an index on disk or in memory, open it again on the next run, load an index into memory completely or save it to another folder, and keep several indexes in a repository that searches them all at once. Settings chosen at creation decide what an index keeps: a normal, compact or metadata-only index, with or without the text of the documents, stored at a choice of compression. An index created by a previous version of the library can be updated to the current format. See [Index lifecycle](https://docs.groupdocs.com/search/python-net/index-lifecycle/), [Search index location](https://docs.groupdocs.com/search/python-net/search-index-location/), [Search index settings](https://docs.groupdocs.com/search/python-net/search-index-settings/), [Search index repository](https://docs.groupdocs.com/search/python-net/search-index-repository/), and [Index format and compatibility](https://docs.groupdocs.com/search/python-net/index-format-and-compatibility/).

## Indexing documents

Index files, folders, streams and structures, including the documents inside ZIP archives and email attachments. Supply the passwords of protected documents, filter which documents are indexed, add fields of your own, assign attributes that can be changed without reindexing, and choose stop words, blended characters and character replacements. Text can be extracted separately from indexing, or in a separate process, and custom text extractors index formats the library does not know. See [Indexing from different sources](https://docs.groupdocs.com/search/python-net/indexing-from-different-sources/), [Indexing options](https://docs.groupdocs.com/search/python-net/indexing-options/), [Indexing password protected documents](https://docs.groupdocs.com/search/python-net/indexing-password-protected-documents/), [Document filtering during indexing](https://docs.groupdocs.com/search/python-net/document-filtering-during-indexing/), [Indexing additional fields](https://docs.groupdocs.com/search/python-net/indexing-additional-fields/), [Document attributes](https://docs.groupdocs.com/search/python-net/document-attributes/), [Character types](https://docs.groupdocs.com/search/python-net/character-types/), [Separate data extraction](https://docs.groupdocs.com/search/python-net/separate-data-extraction/), and [Custom text extractors](/search/python-net/guides/custom-text-extractors/).

## Keeping an index up to date

Update an index to take changed, deleted and added documents into account, merge several indexes into one, and optimize an index to speed up search and to remove deleted documents physically. Delete documents by path or by key, tell the index about renamed documents so they are not reindexed, and check an index's integrity and restore a damaged one. Index changes are atomic, and index data is protected by checksums. See [Update index](https://docs.groupdocs.com/search/python-net/update-index/), [Merge indexes](https://docs.groupdocs.com/search/python-net/merge-indexes/), [Optimize index](https://docs.groupdocs.com/search/python-net/optimize-index/), [Delete indexed documents](https://docs.groupdocs.com/search/python-net/delete-indexed-documents/), [Document renaming](https://docs.groupdocs.com/search/python-net/document-renaming/), and [Checking index integrity](https://docs.groupdocs.com/search/python-net/checking-index-integrity/).

## Search types

Search for words, phrases and patterns with simple, boolean, wildcard, phrase (with wildcards) and regular-expression queries, and narrow a search to a field with faceted search. Date-range and numeric-range search find dates and numbers in the text, and queries can also target file names, document types, metadata fields and the creation and modification dates of files. Different search types combine in one query, written as text or built as objects. See [Build search query](/search/python-net/guides/build-search-query/), [Boolean search](/search/python-net/guides/boolean-search/), [Phrase search](/search/python-net/guides/phrase-search/), [Wildcard search](/search/python-net/guides/wildcard-search/), [Regular expression search](/search/python-net/guides/regular-expression-search/), [Faceted search](/search/python-net/guides/faceted-search/), [Date range search](https://docs.groupdocs.com/search/python-net/date-range-search/), [Numeric range search](https://docs.groupdocs.com/search/python-net/numeric-range-search/), [Queries in text and object form](https://docs.groupdocs.com/search/python-net/queries-in-text-and-object-form/), and the [Query language specification](https://docs.groupdocs.com/search/python-net/query-language-specification/).

## Finding what was meant

Fuzzy search finds words with typos and OCR noise, with a configurable similarity. Synonym, homophone and word-form search widen a query, case-sensitive search narrows it, aliases stand for longer queries, and spell checking and keyboard layout correction repair the query itself. See [Fuzzy search](/search/python-net/guides/fuzzy-search/), [Synonym search](https://docs.groupdocs.com/search/python-net/synonym-search/), [Homophone search](https://docs.groupdocs.com/search/python-net/homophone-search/), [Search for different word forms](https://docs.groupdocs.com/search/python-net/search-for-different-word-forms/), [Case sensitive search](https://docs.groupdocs.com/search/python-net/case-sensitive-search/), [Using aliases](https://docs.groupdocs.com/search/python-net/using-aliases/), [Spell checking](https://docs.groupdocs.com/search/python-net/spell-checking/), and [Keyboard layout correction](https://docs.groupdocs.com/search/python-net/keyboard-layout-correction/).

## Search results and highlighting

A search result lists the found documents with their occurrences, relevance and found fields, and can be filtered by document attributes and other conditions. Highlight the found words in the text of a whole document or in short fragments, as HTML or plain text, read the text of any indexed document, and get reports of past searches. A large result can be read in chunks. See [Work with search results](/search/python-net/guides/work-with-search-results/), [Document filtering in search result](https://docs.groupdocs.com/search/python-net/document-filtering-in-search-result/), [Highlighting search results](/search/python-net/guides/highlighting-search-results/), [Getting indexed documents](https://docs.groupdocs.com/search/python-net/getting-indexed-documents/), [Search reports](https://docs.groupdocs.com/search/python-net/search-reports/), and [Search by chunks](https://docs.groupdocs.com/search/python-net/search-by-chunks/).

## Dictionaries

Each index keeps the dictionaries its search uses - synonyms, homophones, stop words, aliases, the alphabet, character replacements, the spelling corrector and document passwords - and each can be read, changed, exported and imported from Python. See [Managing Dictionaries](https://docs.groupdocs.com/search/python-net/managing-dictionaries/).

## Images and OCR

Calculate and index image hashes for reverse image search, which finds the documents that contain a picture like a given one. The text of images and scans is indexed through an OCR engine you connect. See [Reverse image search](https://docs.groupdocs.com/search/python-net/reverse-image-search/) and [OCR support](https://docs.groupdocs.com/search/python-net/ocr-support/).

## Events and Python callbacks

Index events report what an index does and let a handler take part: follow indexing progress, skip a document, or supply a password as a document needs it, with `index.events.file_indexing += handler`. Text extractors, OCR connectors, loggers and word form providers are plain Python classes or functions that the engine calls. See [Search index events](/search/python-net/guides/search-index-events/), [Logging](https://docs.groupdocs.com/search/python-net/logging/), [Indexing reports](https://docs.groupdocs.com/search/python-net/indexing-reports/), and [Word forms provider](https://docs.groupdocs.com/search/python-net/word-forms-provider/).

## Performance and concurrency

Searches are thread-safe and run while documents are indexed, updated, deleted, merged or optimized; one search can also use several threads. See [Search thread safety](https://docs.groupdocs.com/search/python-net/search-thread-safety/) and [Search options](https://docs.groupdocs.com/search/python-net/search-options/).

## Scaling

A search network distributes the documents over shards on several nodes and balances indexing and search across them. See [Scaling](https://docs.groupdocs.com/search/python-net/scaling/).

## On-premise

GroupDocs.Search for Python via .NET runs entirely on your own infrastructure - your documents never leave your environment. The package is a self-contained wheel that bundles everything it needs, so no Microsoft Office, OpenOffice, or separate runtime has to be installed. See [System Requirements](https://docs.groupdocs.com/search/python-net/system-requirements/) for the supported platforms and native dependencies.
