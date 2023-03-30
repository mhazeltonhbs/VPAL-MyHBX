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
        "coupon": "<coupon>",
        "currency": "<currency>",
        "items": [
            {
                "coupon": "<coupon>",
                "currency": "<currency>",
                "discount": <discount>,
                "item_brand": "<item_brand>",
                "item_category": "<item_category>",
                "item_id": "<item_id>",
                "item_list_name": "<item_list_name>",
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
|ecommerce.coupon|string|Order-level coupon code used for a purchase.|summer\_fun|||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.items[n].coupon|string|Item-level coupon code used for a purchase.|SUMMER\_FUN|||||||
|ecommerce.items[n].currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|ecommerce.items[n].discount|number|Monetary value of discount associated with a purchase.|2.22|||||||
|ecommerce.items[n].item_brand|string|Item brand|Gucci|||||||
|ecommerce.items[n].item_category|string|Item Category \(context-specific\). item\_category2 through item\_category5 can also be used if the item has many categories.|pants|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_list_name|string|The human-readable name of the item list the item showed up in \(if sent with a view\_item\_list event\). If one is not available, populate with numerical index of which list this is on the page \(1-indexed\). For filter\_by\_group component, use that value.|filter\_by\_group, recommended\_products, recently\_viewed\_products|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].price|number|The monetary price of the item, in units of the specified currency parameter.|9.99|||||||
|ecommerce.items[n].quantity|integer|Item quantity.|1|||||||
|ecommerce.payment_method|string|The chosen method of payment.|credit card, gift card, paypal, apple pay|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




