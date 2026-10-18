---
title: "SearchOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk operasi pencarian."
type: docs
weight: 34
url: /id/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Menyediakan opsi untuk operasi pencarian.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Menginisialisasi sebuah instance baru dari kelas SearchOptions. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Menginisialisasi sebuah instance baru dari kelas SearchOptions. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Mendapatkan flag penggunaan sinonim dalam pencarian. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Mengatur flag penggunaan sinonim dalam pencarian. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Mendapatkan flag penggunaan homofon dalam pencarian. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Mengatur flag penggunaan homofon dalam pencarian. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Mendapatkan flag penggunaan bentuk kata berbeda dalam pencarian. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Mengatur flag penggunaan bentuk kata berbeda dalam pencarian. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Mendapatkan flag untuk mengambil atribut yang terkait dengan dokumen yang ditemukan. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Mengatur flag untuk mengambil atribut yang terkait dengan dokumen yang ditemukan. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Menampilkan opsi pencarian fuzzy. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Menampilkan opsi korektor ejaan. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Menampilkan opsi korektor tata letak keyboard. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Menampilkan flag pencarian yang sensitif huruf. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Mengatur flag pencarian yang sensitif huruf. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Menampilkan jumlah total maksimum kemunculan semua istilah dalam kueri pencarian. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Mengatur jumlah total maksimum kemunculan semua istilah dalam kueri pencarian. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Menampilkan jumlah maksimum kemunculan setiap istilah dalam kueri pencarian. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Mengatur jumlah maksimum kemunculan setiap istilah dalam kueri pencarian. |
|
|  | [getDateFormats()](#getDateFormats--) | Menampilkan koleksi format tanggal untuk pencarian rentang tanggal. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Menampilkan flag pencarian berdasarkan potongan. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Mengatur flag pencarian berdasarkan potongan. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Mendapatkan filter dokumen pencarian. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Mengatur filter dokumen pencarian. |
|
|  | [getCancellation()](#getCancellation--) | Mendapatkan objek pembatalan operasi. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Mengatur objek pembatalan operasi. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Menginisialisasi sebuah instance baru dari kelas SearchOptions.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Menginisialisasi sebuah instance baru dari kelas SearchOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Menampilkan flag penggunaan sinonim dalam pencarian. Nilai default adalah false.


**Returns:**
boolean - Flag penggunaan sinonim dalam pencarian.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Mengatur flag penggunaan sinonim dalam pencarian. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Flag penggunaan sinonim dalam pencarian. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Menampilkan flag penggunaan homofon dalam pencarian. Nilai default adalah false.


**Returns:**
boolean - Flag penggunaan homofon dalam pencarian.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Mengatur flag penggunaan homofon dalam pencarian. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Flag penggunaan homofon dalam pencarian. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Menampilkan flag penggunaan bentuk kata berbeda dalam pencarian. Nilai default adalah false.


**Returns:**
boolean - Flag penggunaan bentuk kata berbeda dalam pencarian.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Mengatur flag penggunaan bentuk kata berbeda dalam pencarian. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Bendera untuk menggunakan bentuk kata yang berbeda dalam pencarian. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Mendapatkan bendera untuk mengambil atribut yang terkait dengan dokumen yang ditemukan. Nilai default adalah false.


**Returns:**
boolean - Bendera untuk mengambil atribut yang terkait dengan dokumen yang ditemukan.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Mengatur bendera untuk mengambil atribut yang terkait dengan dokumen yang ditemukan. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Bendera untuk mengambil atribut yang terkait dengan dokumen yang ditemukan. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Menampilkan opsi pencarian fuzzy.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Menampilkan opsi korektor ejaan.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Menampilkan opsi korektor tata letak keyboard.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Mendapatkan bendera untuk pencarian sensitif huruf besar/kecil. Nilai default adalah false.


**Returns:**
boolean - Bendera untuk pencarian sensitif huruf besar/kecil.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Mengatur bendera untuk pencarian sensitif huruf besar/kecil. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Bendera untuk pencarian sensitif huruf besar/kecil. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Mendapatkan jumlah total maksimum kemunculan semua istilah dalam kueri pencarian. Nilai default adalah 500000.


**Returns:**
int - Jumlah total maksimum kemunculan.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Mengatur jumlah total maksimum kemunculan semua istilah dalam kueri pencarian. Nilai default adalah 500000.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah total maksimum kemunculan. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Mendapatkan jumlah maksimum kemunculan setiap istilah dalam kueri pencarian. Nilai default adalah 100000.


**Returns:**
int - Jumlah maksimum kemunculan setiap istilah dalam kueri pencarian.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Mengatur jumlah maksimum kemunculan setiap istilah dalam kueri pencarian. Nilai default adalah 100000.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum kemunculan setiap istilah dalam kueri pencarian. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Mendapatkan koleksi format tanggal untuk pencarian rentang tanggal. Format tanggal default adalah 'dd.MM.yyyy', 'MM/dd/yyyy', dan 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Contoh ini menunjukkan cara mengatur format tanggal untuk pencarian.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Menghapus format tanggal default
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Membuat pola format tanggal 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Cari di indeks
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Mendapatkan bendera untuk pencarian per bagian. Nilai default adalah false.


**Returns:**
boolean - Bendera untuk pencarian per bagian.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Mengatur bendera untuk pencarian per bagian. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Bendera untuk pencarian per bagian. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Mendapatkan filter dokumen pencarian. SearchDocumentFilter bekerja dengan logika inklusi. Gunakan kelas SearchDocumentFilter untuk membuat instance filter dokumen pencarian. Nilai default adalah null, yang berarti semua dokumen yang ditemukan akan dikembalikan.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Contoh ini menunjukkan cara mengatur filter dokumen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen
index.add(documentsFolder);
// Membuat filter dokumen pencarian yang melewatkan dokumen dengan ekstensi '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Membuat filter ekstensi file
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Membalikkan filter ekstensi file
options.setSearchDocumentFilter(invertedFilter);
// Cari dalam indeks
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Mengatur filter dokumen pencarian. SearchDocumentFilter bekerja pada logika inklusi. Gunakan kelas SearchDocumentFilter untuk membuat instance filter dokumen pencarian. Nilai default adalah null, yang berarti semua dokumen yang ditemukan akan dikembalikan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Filter dokumen pencarian. |


Contoh ini menunjukkan cara mengatur filter dokumen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen
index.add(documentsFolder);
// Membuat filter dokumen pencarian yang melewatkan dokumen dengan ekstensi '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Membuat filter ekstensi file
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Membalikkan filter ekstensi file
options.setSearchDocumentFilter(invertedFilter);
// Cari dalam indeks
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Mendapatkan objek pembatalan operasi. Nilai defaultnya adalah null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Mengatur objek pembatalan operasi. Nilai defaultnya adalah null.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objek pembatalan operasi. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
