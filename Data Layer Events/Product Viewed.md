# Product Viewed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "view_item",
  "detailed_event": "Product Viewed",
    "ecommerce": {
        "currency": "<currency>",
        "items": [
            {
                "item_category": "<item_category>",
                "item_category2": "<item_category2>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "price": <price>
            }
        ],
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|ecommerce.items[n].item_category|string|Item Category \(context-specific\). item\_category2 through item\_category5 can also be used if the item has many categories.|pants|||||||
|ecommerce.items[n].item_category2|string|The second category of an item.||||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].price|number|The monetary price of the item, in units of the specified currency parameter.|9.99|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||

## Attached Notes

<p><span class="hljs-string">"item_category"</span>: <span class="hljs-string">"&lt;item_category&gt;": </span></p>
<p><span class="hljs-string">corresponds to top level breadcrumb category, such as wine or wine entertaining</span></p>
<p><span class="hljs-string">"item_category2"</span>: <span class="hljs-string">"&lt;item_category2&gt;"</span>,</p>
<p><span class="hljs-string">corresponds to second level breadcrumb category, such as white wine or glassware</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
