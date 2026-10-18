---
title: "SpellingCorrectorOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk korektor ejaan."
type: docs
weight: 36
url: /id/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

Menyediakan opsi untuk korektor ejaan.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Mendapatkan nilai yang menunjukkan apakah korektor ejaan diaktifkan. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Mengatur nilai yang menunjukkan apakah korektor ejaan diaktifkan. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | Mendapatkan jumlah maksimum kesalahan. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | Mengatur jumlah maksimum kesalahan. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | Mendapatkan nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | Mengatur nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | Mendapatkan kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | Mengatur kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | Mendapatkan nilai yang menunjukkan apakah algoritma harus menganggap pertukaran dua karakter berdekatan sebagai satu kesalahan. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | Mengatur nilai yang menunjukkan apakah algoritma harus menganggap pertukaran dua karakter berdekatan sebagai satu kesalahan. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


Mendapatkan nilai yang menunjukkan apakah korektor ejaan diaktifkan. Nilai default adalah false.


**Returns:**
boolean - Nilai yang menunjukkan apakah korektor ejaan diaktifkan.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


Mengatur nilai yang menunjukkan apakah korektor ejaan diaktifkan. Nilai default adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah korektor ejaan diaktifkan. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


Mendapatkan jumlah maksimum kesalahan. Nilai default adalah 2.


**Returns:**
int - Jumlah maksimum kesalahan.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


Mengatur jumlah maksimum kesalahan. Nilai default adalah  2 .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum kesalahan. |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


Mendapatkan nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. Nilai default adalah  false .


**Returns:**
boolean -  true  jika hanya hasil terbaik yang akan dikembalikan; jika tidak  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


Mengatur nilai yang menunjukkan apakah hanya hasil terbaik yang akan dikembalikan. Nilai default adalah  false .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | true  jika hanya hasil terbaik yang akan dikembalikan; jika tidak  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


Mendapatkan kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. Nilai default adalah  0 .


**Returns:**
byte - Kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


Mengatur kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. Nilai default adalah  0 .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | byte | Kelebihan maksimum dari jumlah minimum kesalahan yang ditemukan. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


Mendapatkan nilai yang menunjukkan apakah algoritma harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. Nilai default adalah  true .


**Returns:**
boolean -  true  jika algoritma koreksi ejaan mempertimbangkan pertukaran; jika tidak  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


Mengatur nilai yang menunjukkan apakah algoritma harus mempertimbangkan pertukaran dua karakter berdekatan sebagai satu kesalahan. Nilai default adalah  true .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | true  jika algoritma koreksi ejaan mempertimbangkan pertukaran; jika tidak  false . |
|

