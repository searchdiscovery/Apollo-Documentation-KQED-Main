# Livestream Pause

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "livestream_pause",
  "detailed_event": "Livestream Pause",
    "event_data": {
        "episode_name": "<episode_name>",
        "media_duration": <media_duration>,
        "media_position": "<media_position>",
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
|event_data.series_name|string|The name of the podcast or livestream series||||||||




