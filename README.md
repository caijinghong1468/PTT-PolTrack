# ML_Proj
This is a machine learning project aimed at determining an author’s political spectrum on the PTT political page.
## Environment
---
|**Environment**|**Version**|
|:----:|:--------:|
|**python**|**3.7.9**|
---
## Install
---
|**Package**|**Intall**|**Version**|
|:----:|:--------:|:--------:|
|**re**|**pip install regex**|**2.2.1**|
|**lxml**|**pip install lxml**|**4.6.2**|
|**pandas**|**pip install pandas**|**2.2.2**|
|**requests**|**pip install requests**|**2.25.1**|
|**beautifulsoup4**|**pip install beautifulsoup4**|**4.9.3**|

---

## Web crawler
In `webcrawler.ipynb`, a `Python` implementation is used to gather posts from the PTT political page.

The dataset contains 1327 records.  

Feature:
- Extract content elements from posts.
- Filter post content, retaining only `Chinese` characters and `numbers`.
- Use `Jieba` to remove `stopwords`.
## Label
Six labels are used to classify the author’s political spectrum:


<img src="/img/label.png" alt=" "  width=200px height=240px/>


## Feature
Use `TF-IDF` (term frequency–inverse document frequency）as feature representation.

