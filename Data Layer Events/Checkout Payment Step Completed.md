# Checkout Payment Step Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "add_payment_info",
  "detailed_event": "Checkout Payment Step Completed",
    "ecommerce": {
        "count_checkout_payment_step_completions": "<count_checkout_payment_step_completions>",
        "currency": "<currency>",
        "items": [
            {
                "item_category": "<item_category>",
                "item_category2": "<item_category2>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "price": <price>,
                "quantity": <quantity>
            }
        ],
        "payment_method": "<payment_method>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.count_checkout_payment_step_completions|number|Captures the specific chat service line used. \(i.e., the agent\)||||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|ecommerce.items[n].item_category|string|Item Category \(context-specific\). item\_category2 through item\_category5 can also be used if the item has many categories.|pants|||||||
|ecommerce.items[n].item_category2|string|The second category of an item.||||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].price|number|The monetary price of the item, in units of the specified currency parameter.|9.99|||||||
|ecommerce.items[n].quantity|integer|Item quantity.|1|||||||
|ecommerce.payment_method|string|The chosen method of payment.|credit card, gift card, paypal, apple pay|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||

## Attached Notes

<p>Fire this event upon completion of the payment step after user has entered payment info and accepted terms &amp; conditions</p>
<p><a href="https://www.screencast.com/t/4neaArcw0q">https://www.screencast.com/t/4neaArcw0q</a></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
