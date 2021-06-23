# Order Placed

### 

## Javascript Code
```js
window.appEventData2306L = window.appEventData2306L || [];
appEventData2306L.push({
  "event": "Order Placed",
    "transaction": {
        "item": [
            {
                "price": {
                    "basePrice": "<basePrice>",
                    "markdownPrice": "<markdownPrice>",
                    "sellingPrice": "<sellingPrice>"
                },
                "productInfo": {
                    "brand": "<brand>",
                    "productID": "<productID>"
                },
                "quantity": "<quantity>",
                "shippingCost": "<shippingCost>",
                "shippingVoucherDiscount": "<shippingVoucherDiscount>",
                "voucherDiscount": {
                    "orderLevelDiscountAmount": "<orderLevelDiscountAmount>",
                    "productLevelDiscountAmount": "<productLevelDiscountAmount>"
                }
            }
        ],
        "productIDList": "<productIDList>",
        "purchaseID": "<purchaseID>",
        "skuList": "<skuList>",
        "total": {
            "currency": "<currency>"
        }
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|basePrice|string|String representation of MSRP of a product. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|currency|string|Currency of the transaction. ISO 4217 (3 character alpha), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|markdownPrice|string|String representation of the price offered. Often called 'hard mark' price. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|orderLevelDiscountAmount|string|String representation of an order level discount applied to an item in a transaction. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productIDList|string|A delimited list of product IDs in the transaction.|1234|7878|9039, abc12|deh213, abc12|||||||
|productLevelDiscountAmount|string|String representation of product level discount for a transaction. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|purchaseID|string|Unique identifier of the purchase. Max Length 20. Used as Unique ID of the purchase or deduplication.|ABC-132456789, DEF-132456789, 0987654567|^[a-zA-Z0-9]{6,20}$|6|20||||
|quantity|integer|Integer number of products being acted upon (added to a cart, removed from wishlist, purchased, reserved)|1, 2, 3, 4, 5||||1|||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|shippingCost|string|The shipping costs for all items within the shippingGroup of the transaction.|15.05, 2, 0.22, 2.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|shippingVoucherDiscount|string|String representation of an discount applied against shipping costs for a shipping group. Positive. Up to two decimal places for cents. No currency symbol.|5, 20, 10.22, 19.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|skuList|string| A delimited list of skus in the transaction.|sku123|sku465, 67890|87576|74674, 87654|||||||
