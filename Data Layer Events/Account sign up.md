# Account sign up

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "account_signup",
  "detailed_event": "Account sign up",
    "event_data": {
        "login_state": <login_state>
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
|event_data.login_state|boolean|Indicates whether a user is logged in - should return true or false||||||||
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

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">login_state</span>:&nbsp;<em>"logged in" or "not logged in"</em></p>
<p><span class="hljs-string">account_creation_date</span>: "08_01_2023"</p>
<p><span class="hljs-string">account_status</span>: "verified" or "unverified"</p>
<p><span class="hljs-string">account_verified_date</span>:&nbsp;<em>"08_01_2023"</em></p>
<p><span class="hljs-string">days_since_creation</span>:&nbsp;<em>9</em></p>
<p><span class="hljs-string">days_since_verified</span>:&nbsp;<em>7</em></p>
<p><span class="hljs-string">member_status</span>:&nbsp;<em>"member" or "not a member"</em></p>
<p><span class="hljs-string">newsletters_subscribed</span>:&nbsp;<em>News Daily, Science, Kid-Friendly</em></p>
<p><span class="hljs-string">signup_source</span>:&nbsp;<em>"account signup" or "newsletter signup"</em></p>
