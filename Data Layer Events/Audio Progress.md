# Audio Progress
Should fire when the user reaches a quartile (i.e. listened to 25%, 50% and 75% of the audio)
### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "audio_progress",
  "detailed_event": "Audio Progress",
    "event_data": {
        "episode_name": "<episode_name>",
        "media_duration": <media_duration>,
        "media_position": "<media_position>",
        "media_quartile": <media_quartile>,
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
|event_data.media_position|string|The length of the media at the time that the user has paused or hit a milestone||||||||
|event_data.media_quartile|number|The quartile that the user has reached while listening to audio or livestream||||||||
|event_data.media_type|string|Indicates which type of audio the user listened to -article audio or podcast|article audio OR podcast|||||||
|event_data.series_name|string|The name of the podcast or livestream series||||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">"episode_name"</span>: <em>"California Needs Renewable Energy. Could We Harness the Power of the Ocean?"</em></p>
<p>"media_position": <em>5:40</em></p>
<p><span class="hljs-string">"media_duration"</span>: <em>21:30</em></p>
<p><em>"media_quartile": 50</em></p>
<p><span class="hljs-string">"media_type"</span>: <em>"podcast"</em></p>
<p><span class="hljs-string">"series_name"</span>: <em>"Bay Curious"</em></p>
