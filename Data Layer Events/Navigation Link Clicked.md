# Navigation Link Clicked

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "click",
  "detailed_event": "Navigation Link Clicked",
    "event_data": {
        "identifier": "<identifier>",
        "link_url": "<link_url>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.identifier|string|Captures the name or ID of the navigation links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.link_url|string|Captures the site destination of the navigation links used.|https:\/\/www.example.com|||||||

## Attached Notes

<p>Send this event when users click on:</p>
<p>&nbsp;</p>
<ol>
<li>Gift Cards</li>
<li>Wine Club</li>
<li>Product of the Month CTA on the main SHOP Nav</li>
<li>Wine of the Month CTA on the main SHOP Nav</li>
</ol>
<p>&nbsp;</p>
<p>event_data.identifier should have these values</p>
<ol>
<li>gift cards</li>
<li>wine club</li>
<li>product of the month</li>
<li>wine of the month</li>
</ol>
