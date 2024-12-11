# ML_PROJ
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
|**jieba**|**pip install jieba**|**0.42.1**|
|**pandas**|**pip install pandas**|**2.2.2**|
|**requests**|**pip install requests**|**2.25.1**|
|**beautifulsoup4**|**pip install beautifulsoup4**|**4.9.3**|

---
## Research Motivation 


## Issue
```
1.以PEST分析來看，
P(政治)
企業需了解政策走向及相關利益相關方的政治立場，進而調整應對策略。
E(經濟)
消費者信任與品牌價值：品牌在多元化市場中，需避免觸碰政治敏感地帶。
S(社會)
社交媒體上的激進或極端內容可能威脅公共秩序，或有帶風向的可能。
T(技術)
AI模型容易因網路上客觀性的數據偏差而產生不當的政治傾向分析，可能引發爭議。

（濃縮版）
企業需根據政策趨勢與利益相關方立場調整策略，避免觸及政治敏感議題以維護品牌信任。
在社會層面，需警惕社交媒體上的極端內容可能影響公共秩序與輿論方向；
技術層面則需注意AI因數據偏差引發政治傾向爭議，確保分析的客觀性與公正性。

2.媒體釋讀:
可以看自己看得文章立場是不是很相似，
可以確保自己是不是在同溫層

3.風向判斷:
政黨可以知道現在網路上風向是怎麼樣。
如果有大量負評語好評，可以推測哪個政黨有在用網軍，去加以應對。
```
## References
[PPT HatePolitics](https://www.ptt.cc/bbs/HatePolitics/index.html)	

## Web crawler
In `webcrawler.ipynb`, a `Python` implementation is used to gather posts from the PTT political page.

The dataset contains 1327 records.  

Feature:
- Extract content elements from posts.
- Filter post content, retaining only `Chinese` characters and `numbers`.
- Use `Jieba` for removing `stopwords`  and incorporating a `custom dictionary` to tailor the segmentation process in article
## Label
Six labels are used to classify the author’s political spectrum:

<img src="/img/label.png" alt=" "  width=200px height=240px/>


## Feature
Use `TF-IDF` (term frequency–inverse document frequency）as feature representation.


## Model


## Analysis

## Conclusion
