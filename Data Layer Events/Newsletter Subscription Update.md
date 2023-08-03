# Newsletter Subscription Update

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "newsletter_subscription_update",
  "detailed_event": "Newsletter Subscription Update",
    "user_data": {
        "newsletters_subscribed": "<newsletters_subscribed>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|user_data.newsletters_subscribed|string|Comma delimited list of all the newsletters that the user has subscribed to||||||||

## Attached Notes

<p><strong>Examples:&nbsp;</strong></p>
<p><span class="hljs-string">newsletters_subscribed</span>:&nbsp;<em>News Daily, Science, Kid-Friendly</em></p>
<p>&nbsp;</p>
