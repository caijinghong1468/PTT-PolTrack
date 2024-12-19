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
|**matplotlib**|**pip install matplotlib**|**24.3.1**|
|**scikit-learn**|**pip install scikit-learn**|**24.3.1**|
|**beautifulsoup4**|**pip install beautifulsoup4**|**4.9.3**|

---
## Research Motivation 
```
   有感於臺灣近年來國民黨（藍）與民進黨（綠）間競爭越來越白熱化，加以今年選舉中民眾黨又成為國會的關鍵少數，近三十年來的藍綠廝殺
中出現新的競爭者，給予臺灣政治版圖帶來新的樣貌，卻也帶來新的爭論。  

   近期又爆發民眾黨（白）黨黨主席柯文哲的京華城案以及中央勞動部的公務員輕生案，民眾對於各黨間的討論更為熱烈。

   部分支持藍綠白黨派的民眾會在PTT黑特政治版發表文章，而由於發文者不一定會明確表示自身的政治傾向，因此我們透過文章中的關鍵字詞  
來判斷各文章的政治傾向。
```
## Issue
```
   政黨可藉由文章的觀點來區分敵我方，了解人民當前對自身的正負面評價。  

   從正面來看，執政黨可藉此檢視、調整政策以符合人民的需求；在野黨則可在了解人民的需求下監督執政黨是否落實，或在下次選舉前提出相  
關政策，以獲得人民支持，贏得選舉。    

   而從負面的角度來看，政黨間競爭時可能會透過「買網軍」的方式來攻擊、抹黑敵對政黨，此時便可透過這個模型來判斷。如出現大量類似攻
擊某政黨的言論，該政黨便可藉此應對並反擊。
```
## Purpoes
```
   在偵測每篇文章政治傾向後，綜合看整體留言趨勢，了解網路上的風向，政黨便可藉此購買網軍。執政黨可以透過網軍來壓迫反對的聲音，鞏  
固自身地位，主導輿論風向，進而獲得下午選舉的連任資格；同樣的，在野黨也可利用這個方式來打擊執政黨，塑造有利於自身形象的言論，進而  
獲得人民的支持。
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
Four labels are used to classify the author’s political spectrum:

<img src="/img/label.png" alt=" "  width=240px height=240px/>


## Feature

Use `TF-IDF` (term frequency–inverse document frequency）and `BOW` as feature representation.

## Model


## Analysis

## Conclusion
