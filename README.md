# ml_proj
It's a machine learning project of determining an author‘s political spectrum on ptt political page 
## Web crawler
In `webcrawler.ipynb`, it's implemented to gather the posts on ptt political page using `Python`.  

The dataset contains 2000 records.  

Feature:
- Get the `content` elements of posts.
- Filter the content of posts leaving `Chinese` and `Number`.
- Use Jieba to remove the stopwords
## Label
Use six labels to decide the author‘s political spectrum: 

![](/img/label.png)

## Feature
Use `TF-IDF` (term frequency–inverse document frequency）as feature.
