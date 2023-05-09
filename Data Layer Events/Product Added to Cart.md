# Product Added to Cart

### 

## Event Firing Instructions

<p>Fires on Application Submission. Note that application submission will have 2 events fire (Product Added to Cart and Course Application Complete).</p>

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "add_to_cart",
  "detailed_event": "Product Added to Cart",
    "ecommerce": {
        "currency": "USD",
        "items": [
            {
                "index": 0,
                "item_brand": "<item_brand>",
                "item_category": "Course",
                "item_category2": "MyHBX Platform",
                "item_id": "<item_id>",
                "item_list_id": "",
                "item_list_name": "",
                "item_name": "<item_name>",
                "item_variant": "<item_variant>",
                "price": <price>,
                "quantity": 1
            }
        ],
        "value": <value>
    }
});
```


## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format. Static value (unless users can use currencies other than USD, then pull dynamically). |USD|||||||
|ecommerce.items[n].index|number|The index/position of the item in a list. Static value since we can only add 1 product at a time. |0|||||||
|ecommerce.items[n].item_brand|string|Based on who owns the course (e.g. Harvard Online or HBS Online). Dynamic value.|Harvard Online or HBS Online|||||||
|ecommerce.items[n].item_category|string|Item Category. Static value. |Course|||||||
|ecommerce.items[n].item_category2|string|The second category of an item. Static value.|MyHBX Platform|||||||
|ecommerce.items[n].item_id|string|Item ID. Uses the course code. Dynamic value. |NEGO|||||||
|ecommerce.items[n].item_list_id|string|Left blank for future use.||||||||
|ecommerce.items[n].item_list_name|string|Left blank for future use.||||||||
|ecommerce.items[n].item_name|string|Item Name. Uses the course name. Dynamic value.|Negotiation Mastery|||||||
|ecommerce.items[n].price|number|Cost of course. Dynamic value.|1750|||||||
|ecommerce.items[n].item_variant|string|Value for Program Dates (e.g. April 4, 2023). Dynamic value.|April 4, 2023|||||||
|ecommerce.items[n].quantity|integer|Item quantity. Static value, will always be 1. |1|||||||
|ecommerce.value|number|Cost of course. Dynamic value. |1750|||||||


