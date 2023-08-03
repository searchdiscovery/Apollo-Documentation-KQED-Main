# Podcast Follow

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "podcast_follow",
  "detailed_event": "Podcast Follow",
    "event_data": {
        "episode_name": "<episode_name>",
        "podcast_platform": "<podcast_platform>",
        "series_name": "<series_name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.episode_name|string|The name of the podcast or livestream episode||||||||
|event_data.podcast_platform|string|Podcast platform name - Apple, Google, NPR One, Stitcher, Spotify, RSS||||||||
|event_data.series_name|string|The name of the podcast or livestream series||||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">"episode_name"</span>:&nbsp;<em>"California Needs Renewable Energy. Could We Harness the Power of the Ocean?"</em></p>
<p><span class="hljs-string">"series_name"</span>:&nbsp;<em>"Bay Curious"</em></p>
<p>"podcast_platform":&nbsp;<em>"Apple Podcasts"</em></p>
