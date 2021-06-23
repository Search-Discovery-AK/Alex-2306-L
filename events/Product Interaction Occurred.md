# Product Interaction Occurred

### 

## Javascript Code
```js
window.appEventData2306L = window.appEventData2306L || [];
appEventData2306L.push({
  "event": "Product Interaction Occurred",
    "product": [
        {
            "price": {
                "priceTier": "<priceTier>",
                "sellingPrice": "<sellingPrice>"
            },
            "productInfo": {
                "brand": "<brand>",
                "businessUnit": "<businessUnit>",
                "name": "<name>",
                "productID": "<productID>",
                "productLine": "<productLine>",
                "trademarkedTechnology": "<trademarkedTechnology>"
            }
        }
    ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|businessUnit|string|The business unit associated with each product.|Apparel, Shoes, Home|||||||
|priceTier|string|Describes the general pricing tier of a product. (Good, Better, Best)|Good, Better, Best, Bronze, Silver, Gold|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|sellingPrice|string|String representation of the price paid after coupons or discounts. Positive. Up to two decimal places for cents. No currency symbol.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|trademarkedTechnology|string|Describes trademarks and/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||
