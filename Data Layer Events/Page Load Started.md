# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "article": {
        "articleAffiliateOrPartner": "<articleAffiliateOrPartner>",
        "articleAuthor": "<articleAuthor>",
        "articleHasAudio": <articleHasAudio>,
        "articleHasGallery": <articleHasGallery>,
        "articleHasVideo": <articleHasVideo>,
        "articleIsLocal": "<articleIsLocal>",
        "articleParagraphCount": <articleParagraphCount>,
        "articleProgramsAndBlogs": "<articleProgramsAndBlogs>",
        "articlePublishDate": <articlePublishDate>,
        "articleSeries": "<articleSeries>",
        "articleTagOrKeyword": "<articleTagOrKeyword>",
        "articleTitle": "<articleTitle>",
        "articleWordCount": <articleWordCount>,
        "article_position_on_page": <article_position_on_page>,
        "number_articles_on_page": <number_articles_on_page>,
        "page_initial_url": "<page_initial_url>",
        "publish_month_year": "<publish_month_year>"
    },
    "event_data": {
        "login_state": <login_state>
    },
    "page_data": {
        "content_group": "<content_group>",
        "country": "<country>",
        "language": "<language>",
        "page_location": "<page_location>",
        "site_section": "<site_section>"
    },
    "user_data": {
        "account_creation_date": <account_creation_date>,
        "account_status": "<account_status>",
        "account_verified_date": <account_verified_date>,
        "days_since_creation": <days_since_creation>,
        "days_since_verified": <days_since_verified>,
        "member_status": "<member_status>",
        "newsletters_subscribed": "<newsletters_subscribed>",
        "signup_source": "<signup_source>",
        "user_id": "<user_id>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|article.articleAffiliateOrPartner|string|Content Affiliate||||||||
|article.articleAuthor|string|The author of the article being viewed||||||||
|article.articleHasAudio|boolean|Boolean - does the article have an audio element?||||||||
|article.articleHasGallery|boolean|Boolean - does the article have an image gallery?||||||||
|article.articleHasVideo|boolean|Boolean - does the article have a video element?||||||||
|article.articleIsLocal|string|Indicates whether article is "Local"||||||||
|article.articleParagraphCount|integer|The number of paragraphs associated with the article being viewed||||||||
|article.articleProgramsAndBlogs|string|Program||||||||
|article.articlePublishDate|number|The date that the article was published||||||||
|article.articleSeries|string|Series||||||||
|article.articleTagOrKeyword|string|content tags or keywords||||||||
|article.articleTitle|string|The title of the article being viewed||||||||
|article.articleWordCount|integer|The word count of the article being viewed||||||||
|article.article_position_on_page|integer|Indicates the numerical order that the article is on the page

Not yet existing||||||||
|article.number_articles_on_page|integer|The total number of articles possible on the page

Not yet existing||||||||
|article.page_initial_url|string|The initial URL of an article page before it changes from dynamically loaded content

Not yet existing||||||||
|article.publish_month_year|string|The month and year that the article was published \(07\_2023\) 

Not yet existing||||||||
|event_data.login_state|boolean|Boolean indicating logged in currently or not||||||||
|page_data.content_group|string|The content group\/site section that the page resides in. Often associated with the first section in the URL path. 

Examples: https:\/\/www.kqed.org\/science = "science" 
https:\/\/www.kqed.org\/podcasts = "podcasts"

Not yet existing||||||||
|page_data.country|string|The country associated with the current page.|US, CA, FR, UK|||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.|en-us, en-gb, ch-cn, fr-ca, fr-fr|||||||
|page_data.page_location|string|The URL of the page currently being viewed. This value will include the full, unaltered URL of the page\/screen the user is currently viewing, including query parameters, fragments, etc., for example https:\/\/www.example.com\/home?user=true&audience=test\#aboutus.|https:\/\/www.example.com\/home?user=true&audience=test\#aboutus|||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|user_data.account_creation_date|integer|The day the user initially created their web account, despite verification date|05162020|||||||
|user_data.account_status|string|The status of the users account - verified or not verified||||||||
|user_data.account_verified_date|number|The date that the user has verified their account via the link back to the site in their email||||||||
|user_data.days_since_creation|integer|The number of days since the user initially created their web account, despite verification date||||||||
|user_data.days_since_verified|integer|The number of days since the user has verified their account via the link back to the site in their email||||||||
|user_data.member_status|string|Notes whether this user is a member \(i.e. donor\)||||||||
|user_data.newsletters_subscribed|string|Comma delimited list of all the newsletters that the user has subscribed to||||||||
|user_data.signup_source|string|The method that the user created the account - via account or newsletter||||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||

## Attached Notes

<p>This dataLayer push should occur on new page loads and when the url and article changes via continuous scroll.</p>
<p>The article object already exists on article and podcast pages. On non article pages this object is not required.<br /><br />There are a few additional parameters included here in article{} particularly with continuous scroll in mind. As users scroll down and back up an article page and new articles come into view and the url changes in the address bar, this event should fire and the parameters should be updated with the correct values to reflect the article currently in view.<br /><br />within page_data, country, language and page_location are not required but are included in all requirements by default.</p>
