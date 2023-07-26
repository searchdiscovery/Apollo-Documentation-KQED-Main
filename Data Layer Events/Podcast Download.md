# Podcast Download

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "podcast_download",
  "detailed_event": "Podcast Download",
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




