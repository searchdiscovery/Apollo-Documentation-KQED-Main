# Audio Complete

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "audio_complete",
  "detailed_event": "Audio Complete",
    "event_data": {
        "episode_name": "<episode_name>",
        "media_duration": <media_duration>,
        "media_type": "<media_type>",
        "series_name": "<series_name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.episode_name|string|The name of the podcast or livestream episode||||||||
|event_data.media_duration|integer|The total length of the media that is being listened to||||||||
|event_data.media_type|string|Indicates which type of audio the user listened to -article audio or podcast|article audio OR podcast|||||||
|event_data.series_name|string|The name of the podcast or livestream series||||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:</span></strong></p>
<p><span class="hljs-string">"episode_name"</span>: <em>"California Needs Renewable Energy. Could We Harness the Power of the Ocean?"</em></p>
<p><span class="hljs-string">"media_duration"</span>: <em>21:30</em></p>
<p><span class="hljs-string">"media_type"</span>: <em>"podcast"</em></p>
<p><span class="hljs-string">"series_name"</span>: <em>"Bay Curious"</em></p>
