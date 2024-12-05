# ml_proj
It's a machine learning project of determining an author‘s political spectrum on ptt political page 
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
In `webcrawler.ipynb`, it's implemented to gather the posts on ptt political page using `Python`.  

The dataset contains 2000 records.  

Feature:
- Get the elements of contents on posts.
- Filter the content of posts leaving `Chinese` and `Number`.
- Use `Jieba` to remove the `stopwords`.
## Label
Use six labels to decide the author‘s political spectrum: 


<img src="/img/label.png" alt=" "  width=200px height=240px/>


## Feature
Use `TF-IDF` (term frequency–inverse document frequency）as feature.

