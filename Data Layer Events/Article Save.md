# Article Save

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "article_save",
  "detailed_event": "Article Save",
    "article": {
        "articleAffiliateOrPartner": "<articleAffiliateOrPartner>",
        "articleAuthor": "<articleAuthor>",
        "articleCategory": "<articleCategory>",
        "articleIsLocal": "<articleIsLocal>",
        "articlePageType": "<articlePageType>",
        "articleParagraphCount": <articleParagraphCount>,
        "articleProgramsAndBlogs": "<articleProgramsAndBlogs>",
        "articlePublishDate": <articlePublishDate>,
        "articleSeries": "<articleSeries>",
        "articleTagOrKeyword": "<articleTagOrKeyword>",
        "articleTitle": "<articleTitle>",
        "articleWordCount": <articleWordCount>,
        "publish_month_year": "<publish_month_year>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|article.articleAffiliateOrPartner|string|Content Affiliate||||||||
|article.articleAuthor|string|The author of the article being viewed||||||||
|article.articleCategory|string|Content Categories||||||||
|article.articleIsLocal|string|Indicates whether article is "Local"||||||||
|article.articlePageType|string|Article Page Type||||||||
|article.articleParagraphCount|integer|The number of paragraphs associated with the article being viewed||||||||
|article.articleProgramsAndBlogs|string|Program||||||||
|article.articlePublishDate|number|The date that the article was published||||||||
|article.articleSeries|string|Series||||||||
|article.articleTagOrKeyword|string|content tags or keywords||||||||
|article.articleTitle|string|The title of the article being viewed||||||||
|article.articleWordCount|integer|The word count of the article being viewed||||||||
|article.publish_month_year|string|The month and year that the article was published \(07\_2023\) 

Not yet existing||||||||




