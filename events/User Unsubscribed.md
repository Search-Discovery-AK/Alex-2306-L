# User Unsubscribed

### 

## Javascript Code
```js
window.appEventData2306L = window.appEventData2306L || [];
appEventData2306L.push({
  "event": "User Unsubscribed",
    "subscription": {
        "subscriptionType": "<subscriptionType>",
        "unsubscribeMethod": "<unsubscribeMethod>"
    },
    "user": {
        "profileAttributesList": "<profileAttributesList>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|profileAttributesList|string|A twice delimited string of key / value pairs.  Use ~ between key and value.  Use | between pairs|homeStore~234|loyaltyTier~gold|memberSince~2002|||||||
|subscriptionType|string|Describes the type of subscription. |news, updates, sales, events|||||||
|unsubscribeMethod|string|Describes the method used to unsubscribe.|footer field, registration opt in, order placed, notification preferences, ESP feed|||||||
