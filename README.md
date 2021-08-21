<h1 align="center"> Google Summer of Code 2021 </h1>
<p align="center"><i>with</i> </p>
<h2 align="center"><a href="https://summerofcode.withgoogle.com/organizations/4724093699489792/">Cuneiform Digital Library Initiative (CDLI)</a></h2>

![GSoC with CDLI](assets/banner.png)

<h2 align="center"><i>Project Report on "<a href="https://summerofcode.withgoogle.com/projects/#5200278048997376">Discovery Search And Advanced Search Features</a>" </i> </h2>

## About the project

The project mainly focuses on enhancing the Search and Advanced search features in the CDLI framework and adding new features to it using [Elasticsearch](https://www.elastic.co/elasticsearch/) and [CakePHP](https://cakephp.org/).

### Objectives and Deliverables

| \# | Objectives                    | Associated Deliverables         | issue(s) | Pull Requests |    Status |
| --- | ----------------------------- | -------------------------------------------- | -------- | -------- | ---- |
| 1 |  Add “Ids” and “Keywords” search fields to both simple and advanced search | Users will be able to search for specific keywords, Id/Numbers artifacts | [#314](https://gitlab.com/cdli/framework/-/issues/314) | [!317](https://gitlab.com/cdli/framework/-/merge_requests/317), [!307](https://gitlab.com/cdli/framework/-/merge_requests/307) |:heavy_check_mark:|
| 2 | Implementation of fuzzy queries | Fuzzy queries would yield search results in all search fields|[#593](https://gitlab.com/cdli/framework/-/issues/593) | [!317](https://gitlab.com/cdli/framework/-/merge_requests/317) |:heavy_check_mark: |
| 3 | Port request to Elasticsearch from cURL to HttpClient | Replaced cURL implementation with HTTP Client|[#350](https://gitlab.com/cdli/framework/-/issues/350)| [!338](https://gitlab.com/cdli/framework/-/merge_requests/338) | :heavy_check_mark: |
| 4 | Highlight transliteration sign values in ATF display |The sign values will be highlighted in the full and compact search results page|[#347](https://gitlab.com/cdli/framework/-/issues/347)| [!354](https://gitlab.com/cdli/framework/-/merge_requests/354) | :heavy_check_mark: |
| 5 | Enable search inscription with sign value permutation |When a user will enable this search feature and search for sign values, all possible sign values with matching sign names of the query will be returned| [#596](https://gitlab.com/cdli/framework/-/issues/596) | [!375](https://gitlab.com/cdli/framework/-/merge_requests/375) |:heavy_check_mark: |
| 6 | Search settings integration | Users will be able to save specific configuration of search settings and search results will be displayed accordingly. |[#540](https://gitlab.com/cdli/framework/-/issues/540) | [!332](https://gitlab.com/cdli/framework/-/merge_requests/332) | :heavy_check_mark: |
| 7 | Input flexibility enhancements |Users will have the flexibility to search with both UTF-8 and ASCII characters |[#597](https://gitlab.com/cdli/framework/-/issues/597)|[!375](https://gitlab.com/cdli/framework/-/merge_requests/375) |:heavy_check_mark: |
| 8 | Filter search results by RTI Image, Transliterations , 3D Data | Users can apply filters such as RTI Image, Transliterations, 3D Data and get search results | [#136](https://gitlab.com/cdli/framework/-/issues/136) | [!369](https://gitlab.com/cdli/framework/-/merge_requests/369) |:heavy_check_mark: |

## Preview of objectives

### 1. Keywords search
  - *Final outcome:*\
      Keywords search field can internally query all the fields of the database and return results accordingly. 
<center>

| Keyword's search |
| :---:	|
| <img src="assets/gifs/keywords.gif" width="800" height="450"> |
| Search in keywords search field |

</center>

### 2. Fuzzy Id's search
 - *Final outcome:*
  
<center>

| Fuzzy Id's search |
| :---:	|
| <img src="assets/gifs/fuzzy-ids.gif" width="800" height="450"> |
| Search yields results even for improper input format "A1169" for Museum Id "OIM A01169" in Id's search |

</center>

### 3. Highlight inscriptions
The text in inscription field of search result was processed
<center>

| Highlight inscriptions |
| :---:	|
| <img src="assets/gifs/highlight-inscriptions.gif" width="800" height="450"> |
| Highlights the inscription input in search results |

</center>

### 4. Sign Value permutation

<center>

| Sign Value permutation |
| :---:	|
| <img src="assets/gifs/sign-permutation.gif" width="800" height="450"> |
| All possible sign-readings of input sign-values can be searched. |

</center>

### 5. Search Settings

<center>

| Search Settings |
| :---:	|
| <img src="assets/gifs/search-settings.gif" width="800" height="450"> |
| Save and update search settings |

</center>

### 6. Input flexibility enhancements

<center>

| Input flexibility enhancements |
| :---:	|
| <img src="assets/gifs/input-flexibility.gif" width="800" height="450"> |
| flexibility to search with both UTF-8 and ASCII characters |

</center>

### 7. Images and Transliteration Filter

<center>

| Images and Transliteration Filter |
| :---:	|
| <img src="assets/gifs/images-filter.gif" width="800" height="450"> |
| Search results can be filtered w.r.t to Images and Transliteration |

</center>


