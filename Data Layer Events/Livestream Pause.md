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
        "media_type": "<media_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.media_type|string|Indicates which type of audio the user listened to -article audio or podcast|article audio OR podcast|||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">media_type</span>:&nbsp;<em>"hls"</em></p>
<p>&nbsp;</p>
