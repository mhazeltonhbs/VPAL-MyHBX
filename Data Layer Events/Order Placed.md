# Order Placed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "purchase",
  "detailed_event": "Order Placed",
    "ecommerce": {
        "coupon": "<coupon>",
        "currency": "<currency>",
        "fulfillment_method": "<fulfillment_method>",
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
        "number_of_payment_methods": <number_of_payment_methods>,
        "order_level_discount": "<order_level_discount>",
        "payment_method": "<payment_method>",
        "revenue_band": "<revenue_band>",
        "tax": <tax>,
        "tax_amount_collected": "<tax_amount_collected>",
        "transaction_id": "<transaction_id>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.coupon|string|Order-level coupon code used for a purchase.|summer\_fun|||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.fulfillment_method|string|Captures the shipping fullfilment method associated with a product.|Shipped, Emailed, Pick Up In Store, Will Call|||||||
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
|ecommerce.number_of_payment_methods|integer|Collects the number of payment methods used for an order at order confirmaton||||||||
|ecommerce.order_level_discount|string|Amount of money discounted for the entire order.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.payment_method|string|Captures the payment methods used for a transaction \(i.e. credit card, Visa, MasterCard, Amex, Paypal, purchase order, etc\).|Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|ecommerce.revenue_band|string|Captures the revenue dollar amount of the order for use in bucketing orders into specific revenue bands \(i.e. $0-$50, $51-$100\).|125.05, 432.21, 90.22, 12.05|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.tax|number|Tax cost associated with a transaction.|1.11|||||||
|ecommerce.tax_amount_collected|string|Captures the amount of tax paid on the order|5.05, 20, 10.22, 9.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




