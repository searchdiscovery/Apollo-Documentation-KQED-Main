# Livestream Progress
Should fire every 5 minutes that the livestream is listened to
### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "livestream_progress",
  "detailed_event": "Livestream Progress",
    "event_data": {
        "livestream_interval": <livestream_interval>,
        "media_type": "<media_type>",
        "minutes_listened": <minutes_listened>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.livestream_interval|integer|Notes the interval that the event is being fired at \(i.e. 5, 10\)|5 \(representing 5 minute intervals\)|||||||
|event_data.media_type|string|Indicates which type of audio the user listened to -article audio or podcast|article audio OR podcast|||||||
|event_data.minutes_listened|integer|The number of minutes since the last livestream\_progress event fired. Ex. if livestream\_progress is set to fire every 5 minutes, this value would be '5'|If livestream\_progress is set to fire every 5 minutes, this value would be '5'|||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">"livestream_interval"</span>: 5</p>
<p><span class="hljs-string">"media_type"</span>: "hls"</p>
<p><span class="hljs-string">"minutes_listened"</span>: 5</p>
