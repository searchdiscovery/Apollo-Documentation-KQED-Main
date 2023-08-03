# Event Register Click

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "event_register_click",
  "detailed_event": "Event Register Click",
    "event_data": {
        "event_id": <event_id>,
        "event_title": "<event_title>",
        "event_type": "<event_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.event_id|integer|The id of the in-person or online event||||||||
|event_data.event_title|string|The title of the in-person or online event||||||||
|event_data.event_type|string|The type of event - in-person or online||||||||

## Attached Notes

<p><strong><span class="hljs-string">Examples:&nbsp;</span></strong></p>
<p><span class="hljs-string">"event_id"</span>: "3338"</p>
<p><span class="hljs-string">"event_title"</span>: "Caf&eacute; Ohlone Popup Dinner"</p>
<p><span class="hljs-string">"event_type"</span>: "In-Person"</p>
